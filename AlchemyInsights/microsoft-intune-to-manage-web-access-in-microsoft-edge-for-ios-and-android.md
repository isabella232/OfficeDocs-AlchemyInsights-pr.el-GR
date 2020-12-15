---
title: Χρήση του Microsoft Intune για τη διαχείριση της πρόσβασης στο Web στο Microsoft Edge για iOS και Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49678255"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="c0823-102">Χρήση του Microsoft Intune για τη διαχείριση της πρόσβασης στο Web στο Microsoft Edge για iOS και Android</span><span class="sxs-lookup"><span data-stu-id="c0823-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="c0823-103">Το Microsoft Edge για iOS και Android επιτρέπει στο χρήστη να κάνει αναζήτηση στο Web από πολλά, εντελώς ξεχωριστά προφίλ.</span><span class="sxs-lookup"><span data-stu-id="c0823-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="c0823-104">Οι πιο ευρείες δυνατότητες προστασίας για τα δεδομένα του Microsoft 365 είναι διαθέσιμες κατά την εγγραφή σας στην οικογένεια προγραμμάτων ασφαλείας Enterprise κινητικότητας +, η οποία περιλαμβάνει δυνατότητες του Microsoft Intune και του Azure Active Directory Premium, όπως η πρόσβαση υπό όρους.</span><span class="sxs-lookup"><span data-stu-id="c0823-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="c0823-105">Τουλάχιστον, θα θέλετε να αναπτύξετε μια πολιτική πρόσβασης υπό όρους που (1) επιτρέπει στους χρήστες να συνδέονται από κινητές συσκευές στο Microsoft Edge για iOS και Android και ότι (2) εφαρμόζει μια πολιτική προστασίας εφαρμογών του Microsoft Intune που παρέχει μια προστατευμένη εμπειρία περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="c0823-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="c0823-106">Για να καταλάβετε πώς μπορείτε να χρησιμοποιήσετε την πρόσβαση υπό όρους και τις πολιτικές, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="c0823-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="c0823-107">Εφαρμογή πολιτικών πρόσβασης υπό όρους της υπηρεσίας καταλόγου Active Directory Azure</span><span class="sxs-lookup"><span data-stu-id="c0823-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="c0823-108">Δημιουργία πολιτικών προστασίας εφαρμογών του Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c0823-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="c0823-109">Χρήση μιας καθολικής σύνδεσης για τις εφαρμογές Web του Azure Active Directory – συνδεδεμένων εφαρμογών Web σε προγράμματα περιήγησης που προστατεύονται από πολιτικές</span><span class="sxs-lookup"><span data-stu-id="c0823-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="c0823-110">Χρήση της ρύθμισης παραμέτρων εφαρμογής για τη διαχείριση της εμπειρίας περιήγησης</span><span class="sxs-lookup"><span data-stu-id="c0823-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="c0823-111">Να επιτρέπεται η χρήση μόνο των λογαριασμών εργασίας και σχολείων</span><span class="sxs-lookup"><span data-stu-id="c0823-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="c0823-112">Ανάπτυξη γενικών πολιτικών ρύθμισης παραμέτρων εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="c0823-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="c0823-113">Ανάπτυξη πολιτικών ρύθμισης παραμέτρων εφαρμογών για προστασία δεδομένων</span><span class="sxs-lookup"><span data-stu-id="c0823-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="c0823-114">Χρήση της διαχείρισης απόληξης της Microsoft για την ανάπτυξη πολιτικών ρύθμισης παραμέτρων εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="c0823-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="c0823-115">Για να μάθετε πώς μπορείτε να αποκτήσετε πρόσβαση σε διαχειριζόμενα αρχεία καταγραφής εφαρμογών, ανατρέξτε [στο θέμα χρήση του Microsoft Edge για iOS και Android για πρόσβαση σε διαχειριζόμενα αρχεία καταγραφής εφαρμογών](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="c0823-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
