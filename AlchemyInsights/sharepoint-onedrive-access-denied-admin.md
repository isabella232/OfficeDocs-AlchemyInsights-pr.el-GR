---
title: Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503528"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="b2aa1-102">Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση στο Κέντρο διαχείρισης του Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="b2aa1-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="b2aa1-103">Εάν λαμβάνετε ένα μήνυμα απαγόρευσης, κατά την προσπάθειά σας να μεταβείτε σε ένα Κέντρο διαχείρισης Sharepoint/OneDrive πρόσβασης, βεβαιωθείτε ότι μπορείτε να [αναθέσετε μια άδεια χρήσης για το χρήστη](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="b2aa1-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="b2aa1-104">Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει να βρίσκονται [που έχει αντιστοιχιστεί σε έναν ρόλο διαχειριστή](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) που μπορούν να έχουν πρόσβαση στα κέντρα διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="b2aa1-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="b2aa1-105">Αυτό το ζήτημα μπορεί να προκύψει, όταν ο χρήστης έχει διαγραφεί και να δημιουργηθεί εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="b2aa1-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b2aa1-106">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό Αναγνωριστικό Passport).</span><span class="sxs-lookup"><span data-stu-id="b2aa1-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b2aa1-107">Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή τους OneDrive, ο χρήστης έχει μια εσφαλμένη PUID.</span><span class="sxs-lookup"><span data-stu-id="b2aa1-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b2aa1-108">Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμού καταλόγου με μια υπηρεσία καταλόγου Active Directory οργανική μονάδα (OU).</span><span class="sxs-lookup"><span data-stu-id="b2aa1-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b2aa1-109">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint, και στη συνέχεια θα μετακινηθεί σε μια διαφορετική OU και resynced με το SharePoint, αυτά ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="b2aa1-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b2aa1-110">Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN ακολουθώντας τα βήματα στο άρθρο, [επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b2aa1-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="b2aa1-111">Σημείωση: Εάν ένα κέντρο OneDrive ή διαχείρισης του SharePoint δεν είναι διαθέσιμες σε πολλούς χρήστες που προηγουμένως είχαν πρόσβαση, ίσως υπάρχει κάποιο ζήτημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="b2aa1-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="b2aa1-112">[Ελέγξτε τον πίνακα εργαλείων υγείας υπηρεσία](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b2aa1-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


