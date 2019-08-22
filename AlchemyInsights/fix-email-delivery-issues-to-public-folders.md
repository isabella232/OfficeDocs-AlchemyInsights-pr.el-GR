---
title: Επιδιορθώστε προβλήματα παράδοσης ηλεκτρονικού ταχυδρομείου για δημόσιους φακέλους με δυνατότητα αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525104"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="4cd07-102">Επιδιορθώστε προβλήματα παράδοσης ηλεκτρονικού ταχυδρομείου για δημόσιους φακέλους με δυνατότητα αλληλογραφίας</span><span class="sxs-lookup"><span data-stu-id="4cd07-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="4cd07-103">Εάν εξωτερικοί αποστολείς δεν είναι δυνατό να στείλετε μηνύματα στους δημόσιους φακέλους σας με δυνατότητα αλληλογραφίας και τους αποστολείς να εμφανιστεί το μήνυμα λάθους: **δεν ήταν δυνατή η εύρεση (550 5.4.1)**, επιβεβαιώστε τον τομέα ηλεκτρονικού ταχυδρομείου για τον δημόσιο φάκελο που έχει ρυθμιστεί ως μια εσωτερική αναμετάδοσης τομέα αντί για ένα επιτακτική τομέα:</span><span class="sxs-lookup"><span data-stu-id="4cd07-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="4cd07-104">Ανοίξτε το [Κέντρο διαχείρισης Exchange (ΕΚΟ)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="4cd07-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="4cd07-105">Μεταβείτε στην **ροή αλληλογραφίας** \> **δεκτά τομέων**, επιλέξτε τον τομέα που έγινε αποδεκτή και, στη συνέχεια, κάντε κλικ στο κουμπί **Επεξεργασία**.</span><span class="sxs-lookup"><span data-stu-id="4cd07-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="4cd07-106">Στις ιδιότητες σελίδας που ανοίγει, εάν έχει οριστεί ο τύπος τομέα **Authoritative**, αλλάξτε την τιμή σε **εσωτερικό αναμετάδοσης** και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="4cd07-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="4cd07-107">Εάν εξωτερικοί αποστολείς, λαμβάνετε το σφάλμα που **δεν έχετε δικαίωμα (550 5.7.13)**, εκτελέστε την ακόλουθη εντολή στο [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) για να δείτε τα δικαιώματα για τους ανώνυμους χρήστες στο δημόσιο φάκελο:</span><span class="sxs-lookup"><span data-stu-id="4cd07-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="4cd07-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Για παράδειγμα, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="4cd07-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="4cd07-109">Για να επιτρέπεται στους εξωτερικούς χρήστες να στείλετε μήνυμα ηλεκτρονικού ταχυδρομείου σε αυτόν τον δημόσιο φάκελο, προσθέστε την πρόσβαση CreateItems δεξιά ο ανώνυμος χρήστης.</span><span class="sxs-lookup"><span data-stu-id="4cd07-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="4cd07-110">Για παράδειγμα, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="4cd07-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
