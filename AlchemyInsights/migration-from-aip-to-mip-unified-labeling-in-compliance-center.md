---
title: Μετεγκατάσταση από AIP σε MIP/Ενοποιημένη σήμανση στο Κέντρο συμμόρφωσης
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825371"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="ac352-102">Μετεγκατάσταση από AIP σε MIP/Ενοποιημένη σήμανση στο Κέντρο συμμόρφωσης</span><span class="sxs-lookup"><span data-stu-id="ac352-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="ac352-103">Για να μετεγκαταστήσετε από ετικέτες AIP σε ενοποιημένες ετικέτες στο κέντρο ασφάλειας και συμμόρφωσης, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="ac352-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="ac352-104">**Ενεργοποίηση προστασίας από την πύλη Azure**</span><span class="sxs-lookup"><span data-stu-id="ac352-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="ac352-105">Εάν δεν το έχετε κάνει ήδη, ανοίξτε ένα νέο παράθυρο του προγράμματος περιήγησης [και πραγματοποιήστε είσοδο στην πύλη Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="ac352-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="ac352-106">Μεταβείτε στη **λάμα προστασίας πληροφοριών** Azure.</span><span class="sxs-lookup"><span data-stu-id="ac352-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="ac352-107">Για παράδειγμα, στο μενού διανομέα, κάντε κλικ στην επιλογή "Όλες **οι υπηρεσίες" και** αρχίστε να **πληκτρολογείτε "Πληροφορίες"** στο πλαίσιο "Φίλτρο".</span><span class="sxs-lookup"><span data-stu-id="ac352-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="ac352-108">Επιλέξτε **"Προστασία πληροφοριών Azure".**</span><span class="sxs-lookup"><span data-stu-id="ac352-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="ac352-109">Εάν δεν έχετε αποκτήσει ξανά πρόσβαση στη λάμα προστασίας [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) πληροφοριών Azure, ανατρέξτε στα πρόσθετα βήματα που απαιτούνται για την προσθήκη αυτής της λάμας στην πύλη.</span><span class="sxs-lookup"><span data-stu-id="ac352-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="ac352-110">Για να ανοίξετε τη λάμα προστασίας πληροφοριών Azure, πρέπει να έχετε είτε ένα πρόγραμμα [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) είτε ένα πρόγραμμα του Office 365 που περιλαμβάνει τη Διαχείριση δικαιωμάτων.</span><span class="sxs-lookup"><span data-stu-id="ac352-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="ac352-111">Εάν έχετε μία από αυτές τις συνδρομές, αλλά βλέπετε ένα μήνυμα ότι δεν είναι δυνατή η βρείτε μια έγκυρη συνδρομή, επικοινωνήστε με την Υποστήριξη [της Microsoft ή](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) χρησιμοποιήστε τα τυπικά κανάλια υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="ac352-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="ac352-112">Εντοπίστε **τις επιλογές** μενού "Διαχείριση" και επιλέξτε **"Ενεργοποίηση προστασίας".**</span><span class="sxs-lookup"><span data-stu-id="ac352-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="ac352-113">Κάντε κλικ **στην επιλογή "Ενεργοποίηση"** και, στη συνέχεια, επιβεβαιώστε την ενέργεια.</span><span class="sxs-lookup"><span data-stu-id="ac352-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="ac352-114">Όταν ολοκληρωθεί η ενεργοποίηση, η γραμμή πληροφοριών εμφανίζει ότι η ενεργοποίηση **ολοκληρώθηκε με επιτυχία.**</span><span class="sxs-lookup"><span data-stu-id="ac352-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="ac352-115">**Μετεγκατάσταση ετικετών προστασίας πληροφοριών Azure στο Κέντρο ασφάλειας του Office 365 & Συμμόρφωσης**</span><span class="sxs-lookup"><span data-stu-id="ac352-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="ac352-116">Βεβαιωθείτε ότι έχετε συνδεθεί ως χρήστης με δικαιώματα καθολικού διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="ac352-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="ac352-117">Μεταβείτε στη **λάμα προστασίας πληροφοριών** Azure.</span><span class="sxs-lookup"><span data-stu-id="ac352-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="ac352-118">Από την **επιλογή μενού** "Διαχείριση", επιλέξτε **"Ενοποιημένη σήμανση".**</span><span class="sxs-lookup"><span data-stu-id="ac352-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="ac352-119">Στην Προστασία **πληροφοριών Azure - Ενοποιημένος δίσκος ετικετών,** κάντε κλικ στην επιλογή **"Ενεργοποίηση"** και ακολουθήστε τις οδηγίες στο Internet.</span><span class="sxs-lookup"><span data-stu-id="ac352-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="ac352-120">**Σημείωση:** Βεβαιωθείτε ότι έχετε τα κατάλληλα δικαιώματα πριν από την ενεργοποίηση της μετεγκατάστασης του Κέντρου & ασφάλειας.</span><span class="sxs-lookup"><span data-stu-id="ac352-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="ac352-121">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτά τα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="ac352-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="ac352-122">Πρέπει να είστε καθολικός διαχειριστής για να ρυθμίσετε τις παραμέτρους της Προστασίας πληροφοριών Azure ή μπορώ να αναθέσω σε άλλους διαχειριστές;</span><span class="sxs-lookup"><span data-stu-id="ac352-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="ac352-123">Σημαντικές πληροφορίες σχετικά με τους ρόλους διαχείρισης μετά τη μετεγκατάσταση στο Κέντρο & ασφάλειας.</span><span class="sxs-lookup"><span data-stu-id="ac352-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="ac352-124">Για περισσότερες πληροφορίες σχετικά με τη μετεγκατάσταση AIP σε ενοποιημένη σήμανση στο Κέντρο ασφάλειας και συμμόρφωσης, ανατρέξτε στο θέμα [Μετεγκατάσταση ετικετών.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="ac352-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
