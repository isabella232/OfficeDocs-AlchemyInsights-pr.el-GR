---
title: Ρύθμιση παραμέτρων της υπηρεσίας παροχής
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482868"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="c35e7-102">Ρύθμιση παραμέτρων της υπηρεσίας παροχής</span><span class="sxs-lookup"><span data-stu-id="c35e7-102">Configuring the Provision service</span></span>

<span data-ttu-id="c35e7-103">Για να λειτουργήσει η αυτοματοποιημένη παροχή χρηστών, το Azure AD απαιτεί έγκυρα διαπιστευτήρια που του επιτρέπουν να συνδέεται στο API των υπηρεσιών Web Workday.</span><span class="sxs-lookup"><span data-stu-id="c35e7-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="c35e7-104">Επιπλέον, το κουμπί "Δοκιμή σύνδεσης" στην εφαρμογή "Εργάσιμη ημέρα σε παροχή χρήστη AD" επικυρώνει επίσης εάν είναι σε θέση να συνδεθεί με τον παράγοντα παροχής του Azure AD Connect που σχετίζεται με τον τομέα AD.</span><span class="sxs-lookup"><span data-stu-id="c35e7-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="c35e7-105">Εάν η πύλη Azure επιστρέφει σφάλμα κατά την αποθήκευση των διαπιστευτηρίων, ακολουθήστε τα παρακάτω προτεινόμενα βήματα:</span><span class="sxs-lookup"><span data-stu-id="c35e7-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="c35e7-106">Επιβεβαιώστε ότι έχετε ρυθμίσει τις παραμέτρους του λογαριασμού χρήστη συστήματος ενοποίησης Workday, όπως αναφέρεται στην ενότητα εκμάθησης "Ρύθμιση παραμέτρων χρήστη [συστήματος ενοποίησης" στις Εργάσιμες ημέρες.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="c35e7-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="c35e7-107">Επιβεβαιώστε ότι η Υπηρεσία παράγοντα παροχής του Azure AD Connect λειτουργεί και λειτουργεί στο διακομιστή Windows εσωτερικής εγκατάστασης χρησιμοποιώντας την Κονσόλα διαχείρισης υπηρεσιών.</span><span class="sxs-lookup"><span data-stu-id="c35e7-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="c35e7-108">Μπορείτε επίσης να ελέγξετε την κατάσταση του παράγοντα στην πύλη Azure, κάνοντας κλικ στο κουμπί "Προβολή παραγόντων εσωτερικής εγκατάστασης".</span><span class="sxs-lookup"><span data-stu-id="c35e7-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="c35e7-109">Βεβαιωθείτε ότι εισάγετε την τιμή για το πεδίο "Workday Username" χρησιμοποιώντας τη username@workday-όνομα-μισθωτή.</span><span class="sxs-lookup"><span data-stu-id="c35e7-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="c35e7-110">Εάν το όνομα του μισθωτή-εργάσιμης ημέρας λείπει, ο έλεγχος ταυτότητας της εργάσιμης ημέρας αποτυγχάνει.</span><span class="sxs-lookup"><span data-stu-id="c35e7-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="c35e7-111">Εάν ρυθμίζετε τις παραμέτρους της ενοποίησης με τον μισθωτή υλοποίησης του Workday, σημειώστε τις προγραμματισμένες ώρες εκτός λειτουργίας του μισθωτή εργάσιμης ημέρας.</span><span class="sxs-lookup"><span data-stu-id="c35e7-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="c35e7-112">Η Εργάσιμη ημέρα έχει προγραμματίσει χρόνο εκτός λειτουργίας για τους μισθωτές υλοποίησης τα Σαββατοκύριακα (συνήθως από το από το απόγευμα της Παρασκευής έως το Σάββατο πρωί) και οι αποτυχίες συνδεσιμότητας κατά τη διάρκεια αυτού του παραθύρου εκτός λειτουργίας είναι ένα γνωστό θέμα που επιλύεται αυτόματα μόλις οι μισθωτές υλοποίησης επιστρέψουν σε σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="c35e7-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="c35e7-113">Σε σπάνιες περιπτώσεις, μπορεί επίσης να δείτε αυτό το σφάλμα εάν ο κωδικός πρόσβασης του χρήστη συστήματος ενοποίησης άλλαξε λόγω ανανέωσης μισθωτή ή εάν ο λογαριασμός είναι σε κατάσταση κλειδώματος ή λήξης.</span><span class="sxs-lookup"><span data-stu-id="c35e7-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="c35e7-114">Ελέγξτε την κατάσταση του χρήστη του Συστήματος ενοποίησης με το διαχειριστή του Workday.</span><span class="sxs-lookup"><span data-stu-id="c35e7-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="c35e7-115">Για περισσότερες λεπτομέρειες σχετικά με τη ρύθμιση παραμέτρων της εργάσιμης ημέρας για την αυτοματοποιημένη παροχή, ανατρέξτε στο πρόγραμμα εκμάθησης: Ρύθμιση [παραμέτρων εργάσιμης ημέρας για αυτόματη προμήθεια από χρήστες.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="c35e7-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
