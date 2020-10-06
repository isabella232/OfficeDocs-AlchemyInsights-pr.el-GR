---
title: Παρακολούθηση της πρόσβασης υπό όρους
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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366428"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="6fa20-102">Παρακολούθηση της πρόσβασης υπό όρους για το Exchange</span><span class="sxs-lookup"><span data-stu-id="6fa20-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="6fa20-103">Οι χρήστες που στοχεύουν στην πρόσβαση υπό όρους θα λαμβάνουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου ειδοποίησης, εάν δεν ικανοποιούν τις απαιτήσεις πρόσβασης της εταιρείας σας.</span><span class="sxs-lookup"><span data-stu-id="6fa20-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6fa20-104">Για να επιλύσετε αυτό το πλαίσιο, συνιστούμε μία ή περισσότερες από τις ακόλουθες λύσεις:</span><span class="sxs-lookup"><span data-stu-id="6fa20-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="6fa20-105">Εάν τεκμαίρεται ότι η συσκευή είναι εγγεγραμμένη, ενημερώστε το χρήστη για να μεταβείτε στην εφαρμογή εταιρεία πύλης και βεβαιωθείτε ότι εμφανίζεται στην πύλη της εταιρείας.</span><span class="sxs-lookup"><span data-stu-id="6fa20-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6fa20-106">Εάν δεν το κάνει, ο χρήστης θα πρέπει να εγγραφεί στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="6fa20-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="6fa20-107">Στην πύλη Azure, μεταβείτε στη συμβατότητα συσκευής Intune >.</span><span class="sxs-lookup"><span data-stu-id="6fa20-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="6fa20-108">Στην περιοχή παρακολούθηση, κάντε κλικ στην επιλογή συμμόρφωση συσκευής.</span><span class="sxs-lookup"><span data-stu-id="6fa20-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="6fa20-109">Προβάλετε την αναφορά συμμόρφωσης της συσκευής σας για να επαληθεύσετε ότι η συσκευή του χρήστη έχει επισημανθεί ως συμβατή.</span><span class="sxs-lookup"><span data-stu-id="6fa20-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="6fa20-110">Στην πύλη Azure, μεταβείτε στη συμβατότητα συσκευής Intune >.</span><span class="sxs-lookup"><span data-stu-id="6fa20-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="6fa20-111">Στην περιοχή Διαχείριση, κάντε κλικ στην επιλογή πολιτικές.</span><span class="sxs-lookup"><span data-stu-id="6fa20-111">Under Manage, click Policies.</span></span> <span data-ttu-id="6fa20-112">Στη λίστα των πολιτικών συμμόρφωσης, επαληθεύστε ότι ένα προφίλ έχει εκχωρηθεί στη συσκευή του χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="6fa20-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6fa20-113">Εάν δεν έχει εκχωρηθεί κανένα προφίλ, τότε το Intune δεν θα έχει τη δυνατότητα να επιβεβαιώσει την κατάσταση συμμόρφωσης της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="6fa20-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="6fa20-114">Επεξεργασία της εκχώρησης πρόσβασης υπό όρους του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="6fa20-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="6fa20-115">Στην πύλη Azure, μεταβείτε στις **Intune**  >  **πολιτικές πρόσβασης υπό όρους**του Intune  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="6fa20-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="6fa20-116">Επιλέξτε μια πολιτική από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="6fa20-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="6fa20-117">Κάντε κλικ στην επιλογή χρήστες και ομάδες.</span><span class="sxs-lookup"><span data-stu-id="6fa20-117">Click Users and groups.</span></span>
4. <span data-ttu-id="6fa20-118">Για να στοχεύσετε μια συγκεκριμένη πολιτική σε κάποιον, προσθέστε τον στη λίστα συμπερίληψη.</span><span class="sxs-lookup"><span data-stu-id="6fa20-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="6fa20-119">Για να εξασφαλίσετε ότι ένα άτομο παραλείπεται από την πολιτική, προσθέστε το στη λίστα εξαίρεσης.</span><span class="sxs-lookup"><span data-stu-id="6fa20-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="6fa20-120">Χρήσιμες συνδέσεις:</span><span class="sxs-lookup"><span data-stu-id="6fa20-120">Helpful links:</span></span>

[<span data-ttu-id="6fa20-121">Επισκόπηση συμμόρφωσης συσκευής</span><span class="sxs-lookup"><span data-stu-id="6fa20-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="6fa20-122">Αντιμετώπιση προβλημάτων CA</span><span class="sxs-lookup"><span data-stu-id="6fa20-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="6fa20-123">Πολιτική αντιμετώπισης προβλημάτων</span><span class="sxs-lookup"><span data-stu-id="6fa20-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="6fa20-124">Παρακολούθηση της συμμόρφωσης συσκευής Intune</span><span class="sxs-lookup"><span data-stu-id="6fa20-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="6fa20-125">Σημείωση: αυτά τα βήματα είναι χρήσιμα μόνο για την αντιμετώπιση προβλημάτων της δυνατότητας πρόσβασης υπό όρους της δυνατότητας Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6fa20-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="6fa20-126">Είναι επίσης δυνατή η καραντίνα μιας συσκευής που αποκλείει την πρόσβαση στο ηλεκτρονικό ταχυδρομείο της με την πολιτική του Exchange.</span><span class="sxs-lookup"><span data-stu-id="6fa20-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="6fa20-127">Μπορείτε να βρείτε περισσότερες πληροφορίες σχετικά με τη διαχείριση συσκευών του Exchange [εδώ](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="6fa20-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
