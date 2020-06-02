---
title: Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται η πρόσβαση
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505379"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="a555c-102">Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται πρόσβασης στο Κέντρο διαχείρισης του Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="a555c-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="a555c-103">Εάν λαμβάνετε ένα μήνυμα που δεν επιτρέπεται από την πρόσβαση κατά την προσπάθεια αναζήτησης σε ένα Κέντρο διαχείρισης του Sharepoint/OneDrive, βεβαιωθείτε ότι [εκχωρείτε μια άδεια χρήσης στο χρήστη](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="a555c-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="a555c-104">Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει επίσης να βεβαιωθείτε ότι του [έχει ανατεθεί ένας ρόλος διαχειριστή](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) που μπορεί να έχει πρόσβαση στα κέντρα διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="a555c-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="a555c-105">Αυτό το ζήτημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγράφεται και δημιουργείται ξανά με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="a555c-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a555c-106">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="a555c-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a555c-107">Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή το OneDrive, ο χρήστης έχει εσφαλμένο PUID.</span><span class="sxs-lookup"><span data-stu-id="a555c-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a555c-108">Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμό καταλόγου με μια οργανωτική μονάδα της υπηρεσίας καταλόγου Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="a555c-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a555c-109">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινούνται σε διαφορετική οργανική μονάδα και επανασυγχρονίζονται με το SharePoint, ενδέχεται να αντιμετωπίσουν αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="a555c-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a555c-110">Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, [Επαναφορά ενός χρήστη στο Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="a555c-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="a555c-111">Σημείωση: Εάν ένα κέντρο διαχείρισης του OneDrive ή του SharePoint δεν είναι διαθέσιμο σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="a555c-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="a555c-112">[Ελέγξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a555c-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


