---
title: Παραχωρήσετε στους χρήστες πρόσβαση στο SharePoint και OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736648"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="c3c04-102">Παραχωρήσετε στους χρήστες πρόσβαση στο SharePoint και OneDrive</span><span class="sxs-lookup"><span data-stu-id="c3c04-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="c3c04-103">Αυτό το ζήτημα προκύπτει πιο συχνά όταν ο χρήστης έχει διαγραφεί και να δημιουργηθεί εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="c3c04-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c3c04-104">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό Αναγνωριστικό Passport).</span><span class="sxs-lookup"><span data-stu-id="c3c04-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c3c04-105">Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή τους OneDrive, ο χρήστης έχει μια εσφαλμένη PUID.</span><span class="sxs-lookup"><span data-stu-id="c3c04-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c3c04-106">Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμού καταλόγου με μια υπηρεσία καταλόγου Active Directory οργανική μονάδα (OU).</span><span class="sxs-lookup"><span data-stu-id="c3c04-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c3c04-107">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint, και στη συνέχεια θα μετακινηθεί σε μια διαφορετική OU και resynced με το SharePoint, αυτά ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="c3c04-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="c3c04-108">Για να επιλύσετε αυτό το ζήτημα θα πρέπει να επαναφέρετε το αρχικό UPN ακολουθώντας τα βήματα στο άρθρο,[επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c3c04-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="c3c04-109">Αφού το κάνετε αυτό, μπορείτε να επαληθεύσετε ο χρήστης διαθέτει δικαιώματα διαχείρισης στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για την [Προσθήκη admin του για OneDrive του χρήστη](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="c3c04-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="c3c04-110">Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο, [Κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="c3c04-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
