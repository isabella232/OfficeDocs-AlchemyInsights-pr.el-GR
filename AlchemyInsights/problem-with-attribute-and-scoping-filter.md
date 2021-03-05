---
title: Πρόβλημα με το χαρακτηριστικό και το φίλτρο αναζήτησης
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481366"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="762d2-102">Πρόβλημα με το χαρακτηριστικό και το φίλτρο αναζήτησης</span><span class="sxs-lookup"><span data-stu-id="762d2-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="762d2-103">**Πρόβλημα με αντικρουόμενες τιμές UPN**</span><span class="sxs-lookup"><span data-stu-id="762d2-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="762d2-104">Η εργάσιμη ημέρα σε AD User Provisioning Workday to AD User Provisioning εμφανίζει το μήνυμα σφάλματος **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.**</span><span class="sxs-lookup"><span data-stu-id="762d2-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="762d2-105">Η λειτουργία απέτυχε, επειδή η τιμή UPN που παρέχεται για την προσθήκη/τροποποίηση δεν είναι μοναδική σε όλο το δάσος.</span><span class="sxs-lookup"><span data-stu-id="762d2-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="762d2-106">Λεπτομέρειες σφάλματος: **CONSTRAINT_ATT_TYPE - userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="762d2-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="762d2-107">Η **τιμή userPrincipalName** που προσπαθεί να ορίσει η γραμμή σύνδεσης Workday κατά τη δημιουργία του λογαριασμού χρήστη AD υπάρχει ήδη στον τομέα AD προορισμού.</span><span class="sxs-lookup"><span data-stu-id="762d2-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="762d2-108">Αυτό σημαίνει ότι είτε (1) ο χρήστης υπάρχει ήδη και ο έλεγχος αναγνωριστικού που ταιριάζει απέτυχε για το χρήστη είτε (2) ο κανόνας δημιουργίας UPN δημιούργησε μια τιμή σε διένεξη.</span><span class="sxs-lookup"><span data-stu-id="762d2-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="762d2-109">Ακολουθούν τα προτεινόμενα βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="762d2-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="762d2-110">Εάν ο χρήστης υπάρχει ήδη και ο έλεγχος αναγνωριστικού που ταιριάζει απέτυχε να συνδέσει το λογαριασμό Εργάσιμη ημέρα με το λογαριασμό της υπηρεσίας καταλόγου Active Directory, ελέγξτε εάν το χαρακτηριστικό αναγνωριστικού που ταιριάζει (συνήθως **αναγνωριστικό** υπαλλήλου) τόσο στην εργάσιμη ημέρα όσο και στο AD έχει ακριβή αντιστοιχία.</span><span class="sxs-lookup"><span data-stu-id="762d2-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="762d2-111">Εάν δεν υπάρχει αντιστοιχία, αυτό είναι ένα πρόβλημα με τα δεδομένα που πρέπει να διορθωθεί.</span><span class="sxs-lookup"><span data-stu-id="762d2-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="762d2-112">Για παράδειγμα, εάν το αναγνωριστικό υπαλλήλου στο Workday είναι 001052 και στο AD είναι 1052, ο μηχανισμός προμήθειας δεν θα συνδέσει τους δύο λογαριασμούς και θα προσπαθήσει να δημιουργήσει ένα χρήστη που υπάρχει ήδη.</span><span class="sxs-lookup"><span data-stu-id="762d2-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="762d2-113">Η λύση σε αυτή την περίπτωση είναι να αλλάξετε την τιμή **"EmployeeID"** στο AD ώστε να περιλαμβάνει τα αρχικά μηδενικά ώστε να είναι 001052.</span><span class="sxs-lookup"><span data-stu-id="762d2-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="762d2-114">Εάν η παράσταση δημιουργίας UPN δεν δημιουργεί μια μοναδική τιμή, εξετάστε το ενδεχόμενο να χρησιμοποιήσετε τη συνάρτηση απο-δημιουργίας **SelectUniqueValue** για να δημιουργείτε μια μοναδική τιμή κάθε φορά.</span><span class="sxs-lookup"><span data-stu-id="762d2-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="762d2-115">**Η εργάσιμη ημέρα σε προμήθεια χρήστη AD δεν έχει ορίσει τιμή χαρακτηριστικού διαχειριστή για το λογαριασμό χρήστη AD**</span><span class="sxs-lookup"><span data-stu-id="762d2-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="762d2-116">Η εργασία "Εργασία σε παροχή χρήστη AD" δεν καθορίζει την τιμή χαρακτηριστικού **διαχειριστή** για τους λογαριασμούς χρηστών AD.</span><span class="sxs-lookup"><span data-stu-id="762d2-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="762d2-117">Υπάρχουν δύο πιθανά σενάρια όταν παρουσιάζεται αυτή η συμπεριφορά:</span><span class="sxs-lookup"><span data-stu-id="762d2-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="762d2-118">Ο διευθυντής σε Εργάσιμη ημέρα δεν μπορεί να επιλυθεί σε έναν αντίστοιχο λογαριασμό χρήστη AD, επειδή ο διευθυντής δεν έχει εμβέλεια.</span><span class="sxs-lookup"><span data-stu-id="762d2-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="762d2-119">Σε ένα **σενάριο πολλών τομέων AD,** η διαχείριση της εργάσιμης ημέρας δεν υπάρχει στον ίδιο τομέα με το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="762d2-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="762d2-120">Δοκιμάστε τα παρακάτω βήματα για να επιλύσετε το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="762d2-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="762d2-121">Εάν έχετε ορίσει φίλτρα εμβέλειας, ελέγξτε πρώτα εάν ο διευθυντής έχει εμβέλεια και ότι ικανοποιεί τον όρο εμβέλειας.</span><span class="sxs-lookup"><span data-stu-id="762d2-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="762d2-122">Εάν ο διευθυντής δεν ικανοποιεί το φίλτρο εμβέλειας, αλλάξτε το φίλτρο, ώστε ο διευθυντής να έχει επίσης πεδίο εφαρμογής της λειτουργίας παροχής.</span><span class="sxs-lookup"><span data-stu-id="762d2-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="762d2-123">Εάν έχετε πολλούς τομείς AD, τότε η σύνδεση έχει έναν γνωστό περιορισμό αδυναμίας επίλυσης αναφορών μεταξύ τομέων.</span><span class="sxs-lookup"><span data-stu-id="762d2-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="762d2-124">Για περισσότερες λεπτομέρειες σχετικά με τη ρύθμιση παραμέτρων της εργάσιμης ημέρας για την αυτοματοποιημένη παροχή, ανατρέξτε στο πρόγραμμα εκμάθησης: Ρύθμιση [παραμέτρων εργάσιμης ημέρας για αυτόματη προμήθεια από χρήστες.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="762d2-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













