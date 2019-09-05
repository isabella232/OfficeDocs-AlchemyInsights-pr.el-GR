---
title: Αντιμετώπιση προβλημάτων μηνυμάτων άρνησης πρόσβασης
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751276"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="cea30-102">Αντιμετώπιση προβλημάτων με τα μηνύματα άρνησης πρόσβασης στο κέντρο διαχείρισης του SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="cea30-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="cea30-103">Εάν λαμβάνετε ένα μήνυμα άρνησης πρόσβασης κατά την προσπάθεια αναζήτησης σε ένα κέντρο διαχείρισης του SharePoint/OneDrive, βεβαιωθείτε ότι έχετε [εκχωρήσει μια άδεια χρήσης στο χρήστη](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="cea30-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="cea30-104">Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει επίσης να βεβαιωθείτε ότι τους έχει [ανατεθεί ένας ρόλος διαχειριστή](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) που μπορεί να αποκτήσει πρόσβαση στα κέντρα διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="cea30-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="cea30-105">Αυτό το ζήτημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγράφεται και δημιουργείται ξανά με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="cea30-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="cea30-106">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό αναγνωριστικό διαβατηρίου).</span><span class="sxs-lookup"><span data-stu-id="cea30-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="cea30-107">Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή το OneDrive, ο χρήστης έχει ένα εσφαλμένο PUID.</span><span class="sxs-lookup"><span data-stu-id="cea30-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="cea30-108">Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμό καταλόγων με μια οργανωτική μονάδα Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="cea30-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="cea30-109">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινούνται σε μια διαφορετική οργανική μονάδα και να συγχρονίσετε ξανά με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="cea30-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="cea30-110">Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, [επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="cea30-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="cea30-111">Σημείωση: Εάν ένα OneDrive ή το κέντρο διαχείρισης του SharePoint δεν είναι διαθέσιμο σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="cea30-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="cea30-112">[Ελέγξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="cea30-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


