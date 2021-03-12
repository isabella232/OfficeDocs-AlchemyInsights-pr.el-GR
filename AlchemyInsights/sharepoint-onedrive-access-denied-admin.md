---
title: Αντιμετώπιση προβλημάτων για μηνύματα που δεν επιτρέπεται να έχουν πρόσβαση
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707954"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="0fcde-102">Αντιμετώπιση προβλημάτων κατά την πρόσβαση σε μηνύματα που δεν επιτρέπεται στο Sharepoint/Κέντρο διαχείρισης του OneDrive</span><span class="sxs-lookup"><span data-stu-id="0fcde-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="0fcde-103">Εάν λαμβάνετε ένα μήνυμα άρνησης πρόσβασης όταν προσπαθείτε να περιηγηθείτε σε ένα Κέντρο διαχείρισης του Sharepoint/OneDrive, βεβαιωθείτε ότι έχετε εκχωρήσει μια άδεια χρήσης [στο χρήστη.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="0fcde-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="0fcde-104">Εάν ο χρήστης έχει μια άδεια χρήσης, [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) θα πρέπει επίσης να βεβαιωθείτε ότι έχει εκχωρηθεί ένας ρόλος διαχειριστή στον οποίο έχει πρόσβαση στα κέντρα διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="0fcde-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="0fcde-105">Αυτό το πρόβλημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγραφεί και δημιουργηθεί εκ νέα με το ίδιο κύριο όνομα χρήστη (UPN).</span><span class="sxs-lookup"><span data-stu-id="0fcde-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="0fcde-106">Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Αναγνωριστικό μοναδικού διαβατηρίου).</span><span class="sxs-lookup"><span data-stu-id="0fcde-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="0fcde-107">Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή στο OneDrive του, ο χρήστης έχει ένα εσφαλμένο PUID.</span><span class="sxs-lookup"><span data-stu-id="0fcde-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="0fcde-108">Ένα δεύτερο σενάριο περιλαμβάνει το συγχρονισμό καταλόγου με μια οργανική μονάδα (OU) της υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0fcde-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="0fcde-109">Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική OU και έχουν επανασυγχρονιστεί με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="0fcde-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="0fcde-110">Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα που αναφέρονται στο άρθρο "Επαναφορά [χρήστη στο Microsoft 365".](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="0fcde-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="0fcde-111">Σημείωση: Εάν ένα Κέντρο διαχείρισης του OneDrive ή του SharePoint δεν είναι διαθέσιμο για πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα προσωρινό ζήτημα υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="0fcde-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="0fcde-112">[Ελέγξτε τον πίνακα εργαλείων της υγείας των υπηρεσιών.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="0fcde-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


