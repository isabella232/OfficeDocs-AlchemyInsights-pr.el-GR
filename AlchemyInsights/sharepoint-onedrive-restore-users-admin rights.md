---
title: Αντιμετώπιση προβλημάτων στα μηνύματα που δεν επιτρέπονται στο OneDrive για επιχειρηματικές τοποθεσίες
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670616"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="a9157-102">Αντιμετώπιση προβλημάτων στα μηνύματα που δεν επιτρέπονται στο OneDrive για επιχειρηματικές τοποθεσίες</span><span class="sxs-lookup"><span data-stu-id="a9157-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="a9157-103">Αυτό το πρόβλημα παρουσιάζεται συχνότερα όταν ένας χρήστης διαγράφεται και δημιουργείται εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="a9157-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a9157-104">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="a9157-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a9157-105">Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή στο OneDrive, ο χρήστης έχει εσφαλμένο PUID.</span><span class="sxs-lookup"><span data-stu-id="a9157-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a9157-106">Ένα δεύτερο σενάριο περιλαμβάνει τον συγχρονισμό καταλόγων με μια οργανική μονάδα της υπηρεσίας καταλόγου Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="a9157-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a9157-107">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική οργανική μονάδα και επανασυγχρονιστούν με το SharePoint, ενδέχεται να αντιμετωπίσουν αυτό το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="a9157-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="a9157-108">Για να επιλύσετε αυτό το πρόβλημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, να [επαναφέρετε ένα χρήστη στο Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="a9157-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="a9157-109">Εάν δεν μπορείτε να επαναφέρετε τον αρχικό χρήστη, θα πρέπει να καταργήσετε τον παλιό χρήστη από την τοποθεσία του OneDrive, χρησιμοποιώντας αυτά τα βήματα, να [καταργήσετε ένα χρήστη από τη λίστα πληροφοριών χρήστη]().</span><span class="sxs-lookup"><span data-stu-id="a9157-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="a9157-110">Αφού ολοκληρωθεί αυτή η ενέργεια, μπορείτε να επαληθεύσετε ότι ο χρήστης έχει δικαιώματα διαχειριστή στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για την [Προσθήκη του διαχειριστή για το OneDrive ενός χρήστη](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="a9157-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="a9157-111">Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο [κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a9157-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
