---
title: Αντιμετώπιση προβλημάτων πρόσβασης δεν επιτρέπεται μηνύματα στο OneDrive για επιχειρηματικές τοποθεσίες
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766711"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="4412f-102">Αντιμετώπιση προβλημάτων πρόσβασης δεν επιτρέπεται μηνύματα στο OneDrive για επιχειρηματικές τοποθεσίες</span><span class="sxs-lookup"><span data-stu-id="4412f-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="4412f-103">Αυτό το ζήτημα παρουσιάζεται συχνότερα όταν ένας χρήστης διαγράφεται και δημιουργείται ξανά με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="4412f-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4412f-104">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό αναγνωριστικό διαβατηρίου).</span><span class="sxs-lookup"><span data-stu-id="4412f-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4412f-105">Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή το OneDrive, ο χρήστης έχει ένα εσφαλμένο PUID.</span><span class="sxs-lookup"><span data-stu-id="4412f-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4412f-106">Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμό καταλόγων με μια οργανωτική μονάδα Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="4412f-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4412f-107">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινούνται σε μια διαφορετική οργανική μονάδα και να συγχρονίσετε ξανά με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="4412f-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="4412f-108">Για να επιλύσετε αυτό το ζήτημα, πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, [επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4412f-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="4412f-109">Εάν δεν μπορείτε να επαναφέρετε τον αρχικό χρήστη, θα πρέπει να καταργήσετε τον παλιό χρήστη από την τοποθεσία του OneDrive χρησιμοποιώντας αυτά τα βήματα, [καταργήστε ένα χρήστη από τη λίστα πληροφοριών χρήστη]().</span><span class="sxs-lookup"><span data-stu-id="4412f-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="4412f-110">Μετά από αυτό, μπορείτε να επαληθεύσετε ότι ο χρήστης έχει δικαιώματα διαχειριστή στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για να [προσθέσετε διαχειριστή για το OneDrive ενός χρήστη](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="4412f-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="4412f-111">Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο, [κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4412f-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
