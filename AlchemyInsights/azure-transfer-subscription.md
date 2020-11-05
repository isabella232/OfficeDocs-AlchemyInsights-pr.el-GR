---
title: Μεταφορά κυριότητας χρέωσης Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922075"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="f88d2-102">Μεταφορά κυριότητας χρέωσης Azure</span><span class="sxs-lookup"><span data-stu-id="f88d2-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="f88d2-103">Πραγματοποιήστε είσοδο στην [πύλη Azure](https://portal.azure.com/) ως διαχειριστής του λογαριασμού χρέωσης που έχει τη συνδρομή που θέλετε να μεταφέρετε.</span><span class="sxs-lookup"><span data-stu-id="f88d2-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="f88d2-104">Εάν δεν είστε βέβαιοι εάν είστε και διαχειριστής ή εάν πρέπει να προσδιορίσετε ποιος είναι, ανατρέξτε στο θέμα [Καθορισμός διαχειριστή χρεώσεων λογαριασμού](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="f88d2-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="f88d2-105">Αναζητήστε τη **Διαχείριση κόστους + χρέωση**.</span><span class="sxs-lookup"><span data-stu-id="f88d2-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="f88d2-106">Επιλέξτε **συνδρομές** από το αριστερό τμήμα παραθύρου.</span><span class="sxs-lookup"><span data-stu-id="f88d2-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="f88d2-107">Ανάλογα με την Access, ίσως χρειαστεί να επιλέξετε ένα εύρος χρέωσης και, στη συνέχεια, **συνδρομές** ή **συνδρομές Azure**.</span><span class="sxs-lookup"><span data-stu-id="f88d2-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="f88d2-108">Επιλέξτε **Μεταφορά κυριότητας χρέωσης** για τη συνδρομή που θέλετε να μεταφέρετε</span><span class="sxs-lookup"><span data-stu-id="f88d2-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="f88d2-109">Πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου ενός χρήστη που είναι διαχειριστής χρέωσης του λογαριασμού που θα είναι ο νέος κάτοχος για τη συνδρομή και, στη συνέχεια, επιλέξτε **Αποστολή αίτησης μεταφοράς**</span><span class="sxs-lookup"><span data-stu-id="f88d2-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="f88d2-110">Ο χρήστης λαμβάνει ένα μήνυμα ηλεκτρονικού ταχυδρομείου με οδηγίες για την αναθεώρηση της αίτησής σας για μεταφορά.</span><span class="sxs-lookup"><span data-stu-id="f88d2-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="f88d2-111">Για να εγκρίνει την αίτηση μεταφοράς, ο χρήστης επιλέγει τη σύνδεση στο μήνυμα ηλεκτρονικού ταχυδρομείου και ακολουθεί τις οδηγίες.</span><span class="sxs-lookup"><span data-stu-id="f88d2-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="f88d2-112">**Σημείωση** : Εάν μεταφέρετε την κυριότητα χρέωσης της συνδρομής σας σε ένα λογαριασμό χρήστη σε άλλο μισθωτή AD Azure, όλες οι αναθέσεις [ελέγχου πρόσβασης βάσει ρόλων (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)για τη διαχείριση πόρων στη συνδρομή καταργούνται οριστικά.</span><span class="sxs-lookup"><span data-stu-id="f88d2-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="f88d2-113">Μόνο ο νέος κάτοχος θα έχει πρόσβαση για τη διαχείριση πόρων στη συνδρομή.</span><span class="sxs-lookup"><span data-stu-id="f88d2-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="f88d2-114">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα μεταφορά συνδρομής σε χρήστη σε άλλο ΜΙΣΘΩΤΉ AD Azure](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f88d2-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f88d2-115">**Προτεινόμενα έγγραφα**</span><span class="sxs-lookup"><span data-stu-id="f88d2-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="f88d2-116">Μεταφορά της κυριότητας χρέωσης μιας συνδρομής Azure σε άλλο λογαριασμό</span><span class="sxs-lookup"><span data-stu-id="f88d2-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="f88d2-117">Πληροφορίες σχετικά με τη μεταφορά της κυριότητας χρέωσης για μια συνδρομή Azure</span><span class="sxs-lookup"><span data-stu-id="f88d2-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="f88d2-118">Μεταφορά του Visual Studio, του δικτύου συνεργατών της Microsoft (MPN) και του Pay as you Go dev/Test συνδρομές</span><span class="sxs-lookup"><span data-stu-id="f88d2-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="f88d2-119">Συνήθεις ερωτήσεις για την κυριότητα μεταφοράς</span><span class="sxs-lookup"><span data-stu-id="f88d2-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="f88d2-120">Αντιμετώπιση προβλημάτων μεταβίβασης ιδιοκτησίας</span><span class="sxs-lookup"><span data-stu-id="f88d2-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
