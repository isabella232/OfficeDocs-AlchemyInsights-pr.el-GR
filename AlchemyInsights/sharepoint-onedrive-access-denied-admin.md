---
title: Αντιμετώπιση προβλημάτων σε μηνύματα που δεν επιτρέπονται
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767662"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="b4b76-102">Αντιμετώπιση προβλημάτων με τα μηνύματα που δεν επιτρέπεται στην Access στο κέντρο διαχείρισης του SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="b4b76-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="b4b76-103">Εάν λαμβάνετε ένα μήνυμα απόρριψης πρόσβασης όταν προσπαθείτε να μεταβείτε σε ένα κέντρο διαχείρισης του SharePoint/OneDrive, βεβαιωθείτε ότι [εκχωρείτε μια άδεια χρήσης στο χρήστη](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="b4b76-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="b4b76-104">Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει επίσης να βεβαιωθείτε ότι του έχει [ανατεθεί ρόλος διαχειριστή](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ο οποίος μπορεί να αποκτήσει πρόσβαση στα κέντρα διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="b4b76-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="b4b76-105">Αυτό το πρόβλημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγραφεί και δημιουργηθεί εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="b4b76-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b4b76-106">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="b4b76-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b4b76-107">Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή στο OneDrive, ο χρήστης έχει εσφαλμένο PUID.</span><span class="sxs-lookup"><span data-stu-id="b4b76-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b4b76-108">Ένα δεύτερο σενάριο περιλαμβάνει τον συγχρονισμό καταλόγων με μια οργανική μονάδα της υπηρεσίας καταλόγου Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="b4b76-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b4b76-109">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική οργανική μονάδα και επανασυγχρονιστούν με το SharePoint, ενδέχεται να αντιμετωπίσουν αυτό το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="b4b76-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b4b76-110">Για να επιλύσετε αυτό το πρόβλημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, να [επαναφέρετε ένα χρήστη στο Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="b4b76-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="b4b76-111">Σημείωση: Εάν ένα κέντρο διαχείρισης του OneDrive ή του SharePoint δεν είναι διαθέσιμο σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, μπορεί να υπάρχει κάποιο πρόβλημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="b4b76-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="b4b76-112">[Επιλέξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b4b76-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


