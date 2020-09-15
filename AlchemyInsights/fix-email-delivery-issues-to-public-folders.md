---
title: Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677928"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="13e49-102">Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας</span><span class="sxs-lookup"><span data-stu-id="13e49-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="13e49-103">Εάν οι εξωτερικοί αποστολείς δεν μπορούν να στείλουν μηνύματα στους δημόσιους φακέλους με δυνατότητα αλληλογραφίας και οι αποστολείς λαμβάνουν το σφάλμα: **δεν ήταν δυνατή η εύρεση (550 5.4.1)**, επιβεβαιώστε ότι ο τομέας ηλεκτρονικού ταχυδρομείου για τον δημόσιο φάκελο έχει ρυθμιστεί ως εσωτερικός τομέας αναμετάδοσης αντί για έναν επίσημο τομέα:</span><span class="sxs-lookup"><span data-stu-id="13e49-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="13e49-104">Ανοίξτε το [Κέντρο διαχείρισης του Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="13e49-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="13e49-105">Μεταβείτε στις περιοχές με αποδοχή **ροής αλληλογραφίας** \> **Accepted domains**, επιλέξτε τον τομέα που αποδέχτηκε και, στη συνέχεια, κάντε κλικ στην επιλογή **Επεξεργασία**.</span><span class="sxs-lookup"><span data-stu-id="13e49-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="13e49-106">Στη σελίδα ιδιοτήτων που ανοίγει, εάν ο τύπος τομέα έχει την τιμή " **έγκυρη**", αλλάξτε την τιμή σε **εσωτερική αναμετάδοση** και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="13e49-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="13e49-107">Εάν οι εξωτερικοί αποστολείς λάβουν το σφάλμα **που δεν έχετε δικαιώματα (550 5.7.13)**, εκτελέστε την ακόλουθη εντολή στο [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) για να δείτε τα δικαιώματα για ανώνυμους χρήστες στον δημόσιο φάκελο:</span><span class="sxs-lookup"><span data-stu-id="13e49-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="13e49-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Για παράδειγμα, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="13e49-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="13e49-109">Για να επιτρέψετε στους εξωτερικούς χρήστες να στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου σε αυτόν το δημόσιο φάκελο, προσθέστε το δικαίωμα πρόσβασης του CreateItems στο χρήστη ανώνυμο.</span><span class="sxs-lookup"><span data-stu-id="13e49-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="13e49-110">Για παράδειγμα, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="13e49-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
