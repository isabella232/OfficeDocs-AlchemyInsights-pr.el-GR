---
title: Πρόβλημα με μεμονωμένο χρήστη
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429713"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="e3620-102">Πρόβλημα με μεμονωμένο χρήστη</span><span class="sxs-lookup"><span data-stu-id="e3620-102">Problem with single user</span></span>

- <span data-ttu-id="e3620-103">Ενδέχεται να μην έχει γίνει προμήθεια του χρήστη, επειδή η υπηρεσία δεν έχει ακόμα την ευκαιρία να αξιολογήσει τον χρήστη.</span><span class="sxs-lookup"><span data-stu-id="e3620-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="e3620-104">Εξετάστε τις οδηγίες για το χρόνο που χρειάζεται για την παροχή, καθώς και τη γραμμή προόδου στη σελίδα ρύθμισης παραμέτρων παροχής.</span><span class="sxs-lookup"><span data-stu-id="e3620-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="e3620-105">Εάν η σταθερή κατάσταση που καθορίζεται στην ενότητα πρόσθετων λεπτομερειών είναι πριν από την ημερομηνία δημιουργίας/ενημέρωσης/διαγραφής του χρήστη, αυτό σημαίνει ότι δεν έχουμε αξιολογήσει ακόμη το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="e3620-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="e3620-106">Σε αυτό το σενάριο, το καλύτερο που μπορείτε να κάνετε είναι να περιμένετε να ολοκληρωθεί η υπηρεσία παροχής.</span><span class="sxs-lookup"><span data-stu-id="e3620-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="e3620-107">Σημειώστε ότι η υπηρεσία μας γνωρίζει μόνο αλλαγές σε ένα χρήστη στο σύστημα προέλευσης (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="e3620-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="e3620-108">Πρέπει να υπάρχει μια έγκυρη αλλαγή στο σύστημα προέλευσης για το Azure AD για να εντοπίσει την αλλαγή και να τη ρέει στην υπηρεσία καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e3620-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="e3620-109">Παροχή υπηρεσίας που αξιολογείται από το χρήστη και καθορίζεται ότι δεν θα πρέπει να γίνει παροχή:</span><span class="sxs-lookup"><span data-stu-id="e3620-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="e3620-110">Εάν έχετε ορίσει ένα φίλτρο με βάση το εύρος του χαρακτηριστικού, βεβαιωθείτε ότι ο χρήστης πληροί τα κριτήρια που έχετε καθορίσει.</span><span class="sxs-lookup"><span data-stu-id="e3620-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="e3620-111">Εάν οι χρήστες υπάρχουν ήδη στο σύστημα προορισμού και στην κατάσταση του χρήστη στην αντιστοίχιση προέλευσης και προορισμού, δεν θα λάβουμε περαιτέρω μέτρα.</span><span class="sxs-lookup"><span data-stu-id="e3620-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="e3620-112">Η υπηρεσία παροχής επιχείρησε να παροχή του χρήστη και απέτυχε.</span><span class="sxs-lookup"><span data-stu-id="e3620-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="e3620-113">Για αυτά τα σενάρια, εξετάστε την καρτέλα αντιμετώπισης προβλημάτων και προτάσεων στα αρχεία καταγραφής προμήθειας:</span><span class="sxs-lookup"><span data-stu-id="e3620-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="e3620-114">Ένα απαιτούμενο χαρακτηριστικό του χρήστη μπορεί να λείπει από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης ή το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e3620-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="e3620-115">Για παράδειγμα, οι κανόνες γενιάς userPrincipalName ή sAMAccountName δεν δημιουργούν τη σωστή τιμή.</span><span class="sxs-lookup"><span data-stu-id="e3620-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="e3620-116">Το χαρακτηριστικό που ταιριάζει (συνήθως employeeId) δεν επιλύει ένα μοναδικό χρήστη στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης ή στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e3620-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="e3620-117">Για παράδειγμα, υπάρχουν δύο χρήστες με το ίδιο employeeId στο AD και η υπηρεσία επιστρέφει έναν κωδικό σφάλματος που υποδεικνύει διπλότυπες καταχωρήσεις προορισμού για την ίδια καταχώρηση προέλευσης.</span><span class="sxs-lookup"><span data-stu-id="e3620-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="e3620-118">Για να εξετάσετε αρχεία καταγραφής για μεμονωμένο χρήστη και ομάδες, [ανατρέξτε στο θέμα "Αναθεώρηση των αρχείων καταγραφής προμήθειας για ένα πρόβλημα με έναν συγκεκριμένο χρήστη".](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="e3620-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
