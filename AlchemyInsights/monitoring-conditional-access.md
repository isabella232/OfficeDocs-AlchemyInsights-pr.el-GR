---
title: Παρακολούθηση πρόσβασης υπό όρους
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708674"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="97136-102">Παρακολούθηση της πρόσβασης υπό όρους για το Exchange</span><span class="sxs-lookup"><span data-stu-id="97136-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="97136-103">Οι στοχευμένοι χρήστες με πρόσβαση υπό όρους θα λάβουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου ειδοποίησης εάν δεν πληρούν τις απαιτήσεις πρόσβασης του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="97136-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="97136-104">Για να επιλύσετε το ζήτημα, συνιστάται να χρησιμοποιήσετε μία ή περισσότερες από τις παρακάτω λύσεις:</span><span class="sxs-lookup"><span data-stu-id="97136-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="97136-105">Εάν η συσκευή θεωρείται ότι είναι εγγεγραμμένη, συμβουλέψτε το χρήστη να μεταβεί στην εφαρμογή Εταιρική πύλη και να βεβαιωθεί ότι εμφανίζεται στην Εταιρική πύλη.</span><span class="sxs-lookup"><span data-stu-id="97136-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="97136-106">Εάν δεν το κάνει, ο χρήστης θα πρέπει να εγγράψει τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="97136-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="97136-107">Στην πύλη Azure, μεταβείτε στο Intune και > συμμόρφωση συσκευής.</span><span class="sxs-lookup"><span data-stu-id="97136-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="97136-108">Στην περιοχή "Παρακολούθηση", κάντε κλικ στην επιλογή "Συμμόρφωση συσκευής".</span><span class="sxs-lookup"><span data-stu-id="97136-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="97136-109">Προβάλετε την αναφορά συμμόρφωσης συσκευής, για να επαληθεύσετε ότι η συσκευή του χρήστη έχει επισημανθεί ως συμβατή.</span><span class="sxs-lookup"><span data-stu-id="97136-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="97136-110">Στην πύλη Azure, μεταβείτε στο Intune και > συμμόρφωση συσκευής.</span><span class="sxs-lookup"><span data-stu-id="97136-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="97136-111">Στην περιοχή "Διαχείριση", κάντε κλικ στην επιλογή "Πολιτικές".</span><span class="sxs-lookup"><span data-stu-id="97136-111">Under Manage, click Policies.</span></span> <span data-ttu-id="97136-112">Στη λίστα με τις πολιτικές συμμόρφωσης, βεβαιωθείτε ότι έχει εκχωρηθεί ένα προφίλ στη συσκευή του χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="97136-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="97136-113">Εάν δεν έχει εκχωρηθεί προφίλ, τότε το Intune δεν θα μπορεί να επιβεβαιώσει την κατάσταση συμμόρφωσης της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="97136-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="97136-114">Επεξεργαστείτε την εκχώρηση πρόσβασης υπό όρους του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="97136-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="97136-115">Στην πύλη Azure, μεταβείτε στις Πολιτικές πρόσβασης υπό όρους **του Intune.**  >    >  </span><span class="sxs-lookup"><span data-stu-id="97136-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="97136-116">Επιλέξτε μια πολιτική από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="97136-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="97136-117">Κάντε κλικ στην επιλογή "Χρήστες και ομάδες".</span><span class="sxs-lookup"><span data-stu-id="97136-117">Click Users and groups.</span></span>
4. <span data-ttu-id="97136-118">Για να στοχεύσετε μια συγκεκριμένη πολιτική σε κάποιον, προσθέστε τον στη λίστα "Συμπερίληψη".</span><span class="sxs-lookup"><span data-stu-id="97136-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="97136-119">Για να εξασφαλίσετε ότι ένα άτομο παραλείπεται από την πολιτική, προσθέστε το στη λίστα εξαιρέσεων.</span><span class="sxs-lookup"><span data-stu-id="97136-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="97136-120">Χρήσιμες συνδέσεις:</span><span class="sxs-lookup"><span data-stu-id="97136-120">Helpful links:</span></span>

[<span data-ttu-id="97136-121">Επισκόπηση συμμόρφωσης συσκευής</span><span class="sxs-lookup"><span data-stu-id="97136-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="97136-122">Αντιμετώπιση προβλημάτων CA</span><span class="sxs-lookup"><span data-stu-id="97136-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="97136-123">Πολιτική αντιμετώπισης προβλημάτων</span><span class="sxs-lookup"><span data-stu-id="97136-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="97136-124">Παρακολούθηση της συμμόρφωσης της συσκευής Intune</span><span class="sxs-lookup"><span data-stu-id="97136-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="97136-125">Σημείωση: αυτά τα βήματα είναι χρήσιμα μόνο για την αντιμετώπιση προβλημάτων της δυνατότητας πρόσβασης υπό όρους της υπηρεσίας καταλόγου Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="97136-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="97136-126">Είναι επίσης δυνατή η καραντίνα μιας συσκευής που αποκλείει την πρόσβαση στο ηλεκτρονικό ταχυδρομείο της με την πολιτική του Exchange.</span><span class="sxs-lookup"><span data-stu-id="97136-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="97136-127">Μπορείτε να βρείτε περισσότερες πληροφορίες σχετικά με τη διαχείριση συσκευών του Exchange [εδώ]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="97136-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
