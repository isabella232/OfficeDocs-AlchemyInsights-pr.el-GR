---
title: Αντιμετώπιση προβλημάτων πρόσβασης επιτρέπονται μηνύματα για OneDrive για επαγγελματικές τοποθεσίες
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232526"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="5ef38-102">Αντιμετώπιση προβλημάτων πρόσβασης επιτρέπονται μηνύματα για OneDrive για επαγγελματικές τοποθεσίες</span><span class="sxs-lookup"><span data-stu-id="5ef38-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="5ef38-103">Αυτό το ζήτημα προκύπτει πιο συχνά όταν ο χρήστης έχει διαγραφεί και να δημιουργηθεί εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="5ef38-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="5ef38-104">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό Αναγνωριστικό Passport).</span><span class="sxs-lookup"><span data-stu-id="5ef38-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="5ef38-105">Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή τους OneDrive, ο χρήστης έχει μια εσφαλμένη PUID.</span><span class="sxs-lookup"><span data-stu-id="5ef38-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="5ef38-106">Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμού καταλόγου με μια υπηρεσία καταλόγου Active Directory οργανική μονάδα (OU).</span><span class="sxs-lookup"><span data-stu-id="5ef38-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="5ef38-107">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint, και στη συνέχεια θα μετακινηθεί σε μια διαφορετική OU και resynced με το SharePoint, αυτά ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="5ef38-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="5ef38-108">Για να επιλύσετε αυτό το ζήτημα θα πρέπει να επαναφέρετε το αρχικό UPN ακολουθώντας τα βήματα στο άρθρο,[επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="5ef38-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="5ef38-109">Εάν δεν μπορείτε να επαναφέρετε το αρχικό χρήστη θα πρέπει να καταργήσετε το παλιό χρήστη από την τοποθεσία OneDrive χρησιμοποιώντας αυτά τα βήματα, [καταργήσετε ένα χρήστη από τη λίστα πληροφοριών χρήστη]().</span><span class="sxs-lookup"><span data-stu-id="5ef38-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="5ef38-110">Αφού το κάνετε αυτό, μπορείτε να επαληθεύσετε ο χρήστης διαθέτει δικαιώματα διαχείρισης στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για την [Προσθήκη admin του για OneDrive του χρήστη](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="5ef38-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="5ef38-111">Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο, [Κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="5ef38-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
