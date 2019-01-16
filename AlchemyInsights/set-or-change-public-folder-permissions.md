---
title: Ορίσετε ή να αλλάξετε τα δικαιώματα σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d537f1446318f1507f52297e547789fdf246b322
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290840"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="0eab2-102">Τα δικαιώματα και οι δημόσιοι φάκελοι</span><span class="sxs-lookup"><span data-stu-id="0eab2-102">Permissions and Public Folders</span></span>

<span data-ttu-id="0eab2-103">Μπορείτε να αλλάξετε τα δικαιώματα σε δημόσιους φακέλους σας με το Outlook, στο Κέντρο διαχείρισης Exchange (ΕΚΟ) ή PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0eab2-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="0eab2-104">Για οδηγίες Outlook, [κάντε κλικ εδώ](https://support.office.com/article/https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="0eab2-104">For Outlook instructions, [click here](https://support.office.com/article/https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="0eab2-p101">Για ΕΚΟ, ανατρέξτε σε [αυτό το άρθρο](https://support.office.com/article/https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) για οδηγίες. Μπορείτε να κάνετε κλικ [εδώ](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) για να μεταβείτε σε ΕΚΟ.</span><span class="sxs-lookup"><span data-stu-id="0eab2-p101">For EAC, refer to [this article](https://support.office.com/article/https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="0eab2-p102">Για Powershell, ανατρέξτε σε [αυτό το άρθρο](https://support.office.com/article/https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) για οδηγίες σχετικά με την προσθήκη PublicFolderClientPermission commandlet. Εάν χρειάζεστε οδηγίες για να συνδεθείτε με το Exchange Powershell, κάντε κλικ [εδώ](https://support.office.com/article/https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="0eab2-p102">For Powershell, refer to [this article](https://support.office.com/article/https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://support.office.com/article/https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="0eab2-p103">Εάν οι **εξωτερικοί χρήστες δεν μπορεί να στείλει μηνύματα ηλεκτρονικού ταχυδρομείου σε έναν δημόσιο φάκελο με δυνατότητα αλληλογραφίας**, η αιτία μπορεί να είναι ότι ο δημόσιος φάκελος δεν διαθέτει δικαιώματα απαιτούνται για παράδοση εξωτερικό μήνυμα ηλεκτρονικού ταχυδρομείου. Μπορείτε να διορθώσετε αυτό το πρόβλημα χρησιμοποιώντας τις οδηγίες του Outlook [εδώ](https://support.office.com/article/https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)ή τις οδηγίες PowerShell [εδώ](https://support.office.com/article/https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="0eab2-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://support.office.com/article/https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.office.com/article/https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

