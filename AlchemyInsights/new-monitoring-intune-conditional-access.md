---
title: Παρακολούθηση της πρόσβασης υπό όρους Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427427"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="43979-102">Παρακολούθηση της πρόσβασης υπό όρους Intune</span><span class="sxs-lookup"><span data-stu-id="43979-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="43979-103">Οι στοχευμένοι χρήστες με πρόσβαση υπό όρους θα λάβουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου ειδοποίησης εάν δεν πληρούν τις απαιτήσεις πρόσβασης του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="43979-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="43979-104">Για να επιλύσετε το ζήτημα, συνιστάται να χρησιμοποιήσετε μία ή περισσότερες από τις παρακάτω λύσεις:</span><span class="sxs-lookup"><span data-stu-id="43979-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="43979-105">Εάν η συσκευή θεωρείται ότι είναι εγγεγραμμένη, συμβουλέψτε το χρήστη να μεταβεί στην εφαρμογή Εταιρική πύλη και να βεβαιωθεί ότι εμφανίζεται στην Εταιρική πύλη.</span><span class="sxs-lookup"><span data-stu-id="43979-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="43979-106">Εάν δεν το κάνει, ο χρήστης πρέπει να εγγράψει τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="43979-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="43979-107">Στην πύλη Azure, μεταβείτε στη **συμμόρφωση συσκευής Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="43979-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="43979-108">Για να προβάλετε την αναφορά συμμόρφωσης συσκευής για να επαληθεύσετε ότι η συσκευή του χρήστη έχει επισημανθεί ως συμβατή, στην περιοχή **"Παρακολούθηση",** κάντε κλικ στην επιλογή **"Συμμόρφωση συσκευής".**</span><span class="sxs-lookup"><span data-stu-id="43979-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="43979-109">Στην πύλη Azure, μεταβείτε στη **συμμόρφωση συσκευής Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="43979-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="43979-110">Στην περιοχή **"Διαχείριση", κάντε** κλικ στην επιλογή **"Πολιτικές".**</span><span class="sxs-lookup"><span data-stu-id="43979-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="43979-111">Στη λίστα με τις πολιτικές συμμόρφωσης, βεβαιωθείτε ότι έχει εκχωρηθεί ένα προφίλ στη συσκευή του χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="43979-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="43979-112">Εάν δεν έχει εκχωρηθεί προφίλ, τότε το Intune δεν θα μπορεί να επιβεβαιώσει την κατάσταση συμμόρφωσης της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="43979-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="43979-113">Επεξεργαστείτε την εκχώρηση πρόσβασης υπό όρους του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="43979-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="43979-114">Στην πύλη Azure, μεταβείτε στις Πολιτικές πρόσβασης υπό όρους **του Intune,** επιλέξτε μια πολιτική από τη λίστα και  >    >  κάντε κλικ στην επιλογή "Χρήστες **και ομάδες".**</span><span class="sxs-lookup"><span data-stu-id="43979-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="43979-115">Για να στοχεύσετε μια συγκεκριμένη πολιτική σε κάποιον, προσθέστε τον στη λίστα **"Συμπερίληψη".**</span><span class="sxs-lookup"><span data-stu-id="43979-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="43979-116">Για να εξασφαλίσετε ότι ένα άτομο παραλείπεται από την πολιτική, προσθέστε το στη λίστα **εξαιρέσεων.**</span><span class="sxs-lookup"><span data-stu-id="43979-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="43979-117">**Χρήσιμες συνδέσεις:**</span><span class="sxs-lookup"><span data-stu-id="43979-117">**Helpful links:**</span></span>

- [<span data-ttu-id="43979-118">Επισκόπηση συμμόρφωσης συσκευής</span><span class="sxs-lookup"><span data-stu-id="43979-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="43979-119">Αντιμετώπιση προβλημάτων CA</span><span class="sxs-lookup"><span data-stu-id="43979-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="43979-120">Πολιτική αντιμετώπισης προβλημάτων</span><span class="sxs-lookup"><span data-stu-id="43979-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="43979-121">Παρακολούθηση συμμόρφωσης συσκευής Intune</span><span class="sxs-lookup"><span data-stu-id="43979-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="43979-122">Αυτά τα βήματα είναι χρήσιμα μόνο για την αντιμετώπιση προβλημάτων της δυνατότητας πρόσβασης υπό όρους της υπηρεσίας καταλόγου Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="43979-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="43979-123">Είναι επίσης δυνατή η καραντίνα μιας συσκευής που αποκλείει την πρόσβαση στο ηλεκτρονικό ταχυδρομείο της με την πολιτική του Exchange.</span><span class="sxs-lookup"><span data-stu-id="43979-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="43979-124">Περισσότερες πληροφορίες σχετικά με τη διαχείριση συσκευών του Exchange μπορείτε να [**βρείτε εδώ.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="43979-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
