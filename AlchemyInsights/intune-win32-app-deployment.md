---
title: Ανάπτυξη εφαρμογών Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461796"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="7da35-102">Ανάπτυξη εφαρμογών Intune Win32</span><span class="sxs-lookup"><span data-stu-id="7da35-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="7da35-103">Το Microsoft Intune επιτρέπει τις εφαρμογές Win32, συμπεριλαμβανομένων, ενδεικτικά, του MSI και του. Το EXE θα αναπτυχθεί σε συσκευές με Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7da35-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="7da35-104">Ο μηχανισμός ανάπτυξης που χρησιμοποιείται απαιτεί την επέκταση διαχείρισης Intune (IME) να υπάρχει στη συσκευή προορισμού.</span><span class="sxs-lookup"><span data-stu-id="7da35-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="7da35-105">Το IME θα εγκατασταθεί αυτόματα ως αποτέλεσμα της στόχευσης μιας δέσμης ενεργειών PowerShell ή μιας ανάπτυξης εφαρμογών Win32 σε ένα χρήστη/συσκευή.</span><span class="sxs-lookup"><span data-stu-id="7da35-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="7da35-106">Υπάρχουν επίσης ορισμένα προαπαιτούμενα που πρέπει να πληρούνται προκειμένου να αναπτυχθούν εφαρμογές Win32 που περιλαμβάνουν:</span><span class="sxs-lookup"><span data-stu-id="7da35-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="7da35-107">Υποστηριζόμενες πλατφόρμες: Windows 10 έκδοση 1607 ή νεότερη έκδοση (εκδόσεις Enterprise, Pro και Education).</span><span class="sxs-lookup"><span data-stu-id="7da35-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="7da35-108">Υποστηριζόμενη αρχιτεκτονική: x86 και x64.</span><span class="sxs-lookup"><span data-stu-id="7da35-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="7da35-109">Διαχείριση συσκευών: AAD και αυτόματη εγγραφή (συμπεριλαμβανομένων των υβριδικών τομέων που είναι συνδεδεμένοι και της πολιτικής ομάδας που έχουν εγγραφεί αυτόματα).</span><span class="sxs-lookup"><span data-stu-id="7da35-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="7da35-110">Μορφή πακέτου εφαρμογής:. αρχείο **intunewin**  που εκπονήθηκε από το [εργαλείο προετοιμασίας περιεχομένου του Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="7da35-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="7da35-111">Περιορισμοί</span><span class="sxs-lookup"><span data-stu-id="7da35-111">Limitations:</span></span>
    - <span data-ttu-id="7da35-112">Μέγιστο μέγεθος: 8GB.</span><span class="sxs-lookup"><span data-stu-id="7da35-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="7da35-113">Μη υποστηριζόμενη αρχιτεκτονική: όπλα.</span><span class="sxs-lookup"><span data-stu-id="7da35-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="7da35-114">Εξετάστε το έγγραφο "[Προσθήκη, εκχώρηση και παρακολούθηση μιας εφαρμογής Win32 στο Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" για πληροφορίες σχετικά με αυτά τα βήματα.</span><span class="sxs-lookup"><span data-stu-id="7da35-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="7da35-115">Λεπτομέρειες σχετικά με την αντιμετώπιση προβλημάτων ανάπτυξης εφαρμογών στα Windows, συμπεριλαμβανομένων των εφαρμογών Win32, μπορούν να αναθεωρηθούν στα ακόλουθα έγγραφα</span><span class="sxs-lookup"><span data-stu-id="7da35-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="7da35-116">Αντιμετώπιση προβλημάτων εγκατάστασης εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="7da35-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="7da35-117">Αντιμετώπιση προβλημάτων εφαρμογών Win32</span><span class="sxs-lookup"><span data-stu-id="7da35-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)