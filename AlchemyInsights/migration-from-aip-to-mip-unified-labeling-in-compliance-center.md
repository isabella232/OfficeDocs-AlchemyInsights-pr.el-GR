---
title: Μετεγκατάσταση από AIP σε ΠΕΠ/ενοποιημένη επισήμανση στο κέντρο συμμόρφωσης
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674326"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="073ac-102">Μετεγκατάσταση από AIP σε ΠΕΠ/ενοποιημένη επισήμανση στο κέντρο συμμόρφωσης</span><span class="sxs-lookup"><span data-stu-id="073ac-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="073ac-103">Για να κάνετε μετεγκατάσταση από ετικέτες AIP σε ενοποιημένη σήμανση στο κέντρο ασφάλειας και συμμόρφωσης, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="073ac-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="073ac-104">**Ενεργοποίηση προστασίας από την πύλη Azure**</span><span class="sxs-lookup"><span data-stu-id="073ac-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="073ac-105">Εάν δεν το έχετε κάνει ήδη, ανοίξτε ένα νέο παράθυρο του προγράμματος περιήγησης και [Πραγματοποιήστε είσοδο στην πύλη Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="073ac-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="073ac-106">Μεταβείτε στη λεπίδα **προστασίας πληροφοριών Azure** .</span><span class="sxs-lookup"><span data-stu-id="073ac-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="073ac-107">Για παράδειγμα, στο μενού Hub, κάντε κλικ στην επιλογή **όλες οι υπηρεσίες** και αρχίστε να πληκτρολογείτε **πληροφορίες** στο πλαίσιο φίλτρο.</span><span class="sxs-lookup"><span data-stu-id="073ac-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="073ac-108">Επιλέξτε **προστασία πληροφοριών Azure**.</span><span class="sxs-lookup"><span data-stu-id="073ac-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="073ac-109">Εάν δεν έχετε αποκτήσει πρόσβαση στο δίσκο προστασίας πληροφοριών Azure πριν, ανατρέξτε στα [πρόσθετα βήματα](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) εφάπαξ για να προσθέσετε αυτήν τη λεπίδα στην πύλη.</span><span class="sxs-lookup"><span data-stu-id="073ac-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="073ac-110">Για να ανοίξετε το Blade προστασία πληροφοριών Azure, πρέπει να έχετε ένα [πρόγραμμα προστασίας πληροφοριών Azure Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ή ένα πρόγραμμα του Office 365 που περιλαμβάνει τη διαχείριση δικαιωμάτων.</span><span class="sxs-lookup"><span data-stu-id="073ac-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="073ac-111">Εάν έχετε μία από αυτές τις συνδρομές, αλλά δείτε ένα μήνυμα ότι δεν είναι δυνατή η εύρεση μιας έγκυρης συνδρομής, [επικοινωνήστε με την υποστήριξη της Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ή χρησιμοποιήστε τα τυπικά κανάλια υποστήριξής σας.</span><span class="sxs-lookup"><span data-stu-id="073ac-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="073ac-112">Εντοπίστε τις επιλογές **διαχείρισης** μενού και επιλέξτε **Ενεργοποίηση προστασίας**.</span><span class="sxs-lookup"><span data-stu-id="073ac-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="073ac-113">Κάντε κλικ στην επιλογή **Ενεργοποίηση**και, στη συνέχεια, επιβεβαιώστε την ενέργειά σας.</span><span class="sxs-lookup"><span data-stu-id="073ac-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="073ac-114">Όταν ολοκληρωθεί η ενεργοποίηση, η γραμμή πληροφοριών εμφανίζει την **Ενεργοποίηση ολοκληρώθηκε με επιτυχία**.</span><span class="sxs-lookup"><span data-stu-id="073ac-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="073ac-115">**Μετεγκατάσταση ετικετών προστασίας πληροφοριών του Azure στο κέντρο συμμόρφωσης & ασφαλείας του Office 365**</span><span class="sxs-lookup"><span data-stu-id="073ac-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="073ac-116">Βεβαιωθείτε ότι έχετε συνδεθεί ως χρήστης με δικαιώματα καθολικού διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="073ac-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="073ac-117">Μεταβείτε στη λεπίδα **προστασίας πληροφοριών Azure** .</span><span class="sxs-lookup"><span data-stu-id="073ac-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="073ac-118">Από την επιλογή " **Διαχείριση** μενού", επιλέξτε " **ενοποιημένη επισήμανση**".</span><span class="sxs-lookup"><span data-stu-id="073ac-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="073ac-119">Στη λάμα **προστασίας πληροφοριών Azure-ενοποιημένη ετικέτα** , κάντε κλικ στην επιλογή **Ενεργοποίηση** και ακολουθήστε τις οδηγίες στο Internet.</span><span class="sxs-lookup"><span data-stu-id="073ac-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="073ac-120">**Σημείωση**: Βεβαιωθείτε ότι έχετε τα κατάλληλα δικαιώματα για να ενεργοποιήσετε τη μετεγκατάσταση του κέντρου συμμόρφωσης & ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="073ac-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="073ac-121">Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω άρθρα:</span><span class="sxs-lookup"><span data-stu-id="073ac-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="073ac-122">Πρέπει να είστε καθολικός διαχειριστής για να ρυθμίσετε τις παραμέτρους της προστασίας πληροφοριών του Azure ή μπορώ να αναθέτω σε άλλους διαχειριστές;</span><span class="sxs-lookup"><span data-stu-id="073ac-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="073ac-123">Σημαντικές πληροφορίες σχετικά με τους ρόλους διαχείρισης μετά τη μετεγκατάσταση στο κέντρο συμμόρφωσης & ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="073ac-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="073ac-124">Για περισσότερες πληροφορίες σχετικά με το AIP για την ενοποιημένη επισήμανση της μετεγκατάστασης στο κέντρο ασφάλειας και συμμόρφωσης, ανατρέξτε στο θέμα [μετεγκατάσταση ετικετών](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="073ac-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
