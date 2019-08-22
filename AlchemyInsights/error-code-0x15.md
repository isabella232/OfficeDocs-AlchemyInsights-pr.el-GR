---
title: Κωδικός σφάλματος 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526995"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="cd701-103">Παρουσιάστηκε σφάλμα κατά την ενεργοποίηση Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας</span><span class="sxs-lookup"><span data-stu-id="cd701-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="cd701-104">Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου.</span><span class="sxs-lookup"><span data-stu-id="cd701-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="cd701-105">**Κλειδί μητρώου**</span><span class="sxs-lookup"><span data-stu-id="cd701-105">**Registry key**</span></span>|<span data-ttu-id="cd701-106">**Τύπος**</span><span class="sxs-lookup"><span data-stu-id="cd701-106">**Type**</span></span>|<span data-ttu-id="cd701-107">**Τιμή**</span><span class="sxs-lookup"><span data-stu-id="cd701-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cd701-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="cd701-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="cd701-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="cd701-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="cd701-110">1</span><span class="sxs-lookup"><span data-stu-id="cd701-110">1</span></span>  <br/> |

<span data-ttu-id="cd701-111">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="cd701-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="cd701-112">ADAL είναι ενεργοποιημένη από προεπιλογή στο Office 365 ProPlus και Office 2016.</span><span class="sxs-lookup"><span data-stu-id="cd701-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="cd701-113">Υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ήταν προηγουμένως με το όνομα των υπηρεσιών Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="cd701-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  