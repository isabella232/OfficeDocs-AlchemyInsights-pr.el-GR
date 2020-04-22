---
title: Παρακολούθηση πρόσβασης υπό όρους
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713718"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="23fb0-102">Παρακολούθηση πρόσβασης υπό όρους για exchange</span><span class="sxs-lookup"><span data-stu-id="23fb0-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="23fb0-103">Οι χρήστες που είναι στόχοι με πρόσβαση υπό όρους θα λάβουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου ειδοποίησης, εάν δεν πληρούν τις απαιτήσεις πρόσβασης του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="23fb0-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="23fb0-104">Για να επιλύσετε, συνιστούμε μία ή περισσότερες από τις ακόλουθες λύσεις:</span><span class="sxs-lookup"><span data-stu-id="23fb0-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="23fb0-105">Εάν η συσκευή τεκμαίρεται ότι είναι εγγεγραμμένη, συμβουλέψτε το χρήστη να μεταβεί στην εφαρμογή Εταιρική πύλη και βεβαιωθείτε ότι εμφανίζεται στην Εταιρική Πύλη.</span><span class="sxs-lookup"><span data-stu-id="23fb0-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="23fb0-106">Εάν δεν το κάνει, ο χρήστης θα πρέπει να εγγράψει τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="23fb0-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="23fb0-107">Στην πύλη Azure μεταβείτε \*\*στη συμμόρφωση της συσκευής Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="23fb0-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="23fb0-108">Στην περιοχή **Οθόνη,** κάντε κλικ στην επιλογή **Συμμόρφωση συσκευής**.</span><span class="sxs-lookup"><span data-stu-id="23fb0-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="23fb0-109">Προβάλετε την αναφορά συμμόρφωσης της συσκευής σας για να βεβαιωθείτε ότι η συσκευή του χρήστη έχει επισημανθεί ως συμβατή.</span><span class="sxs-lookup"><span data-stu-id="23fb0-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="23fb0-110">Στην πύλη Azure μεταβείτε \*\*στη συμμόρφωση της συσκευής Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="23fb0-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="23fb0-111">Στην περιοχή **Διαχείριση**, κάντε κλικ στην επιλογή **Πολιτικές**.</span><span class="sxs-lookup"><span data-stu-id="23fb0-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="23fb0-112">Στη λίστα των πολιτικών συμμόρφωσης, βεβαιωθείτε ότι έχει αντιστοιχιστεί ένα προφίλ στη συσκευή του χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="23fb0-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="23fb0-113">Εάν δεν έχει αντιστοιχιστεί προφίλ, τότε το Intune δεν θα είναι σε θέση να επιβεβαιώσει την κατάσταση συμμόρφωσης της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="23fb0-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="23fb0-114">Επεξεργασία της εκχώρησης πρόσβασης υπό όρους του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="23fb0-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="23fb0-115">Στην πύλη Azure, μεταβείτε **στις πολιτικές \> πρόσβασης \> υπό όρους intune**</span><span class="sxs-lookup"><span data-stu-id="23fb0-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="23fb0-116">Επιλογή πολιτικής από τη λίστα</span><span class="sxs-lookup"><span data-stu-id="23fb0-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="23fb0-117">Κάντε κλικ στην επιλογή **Χρήστες και ομάδες**</span><span class="sxs-lookup"><span data-stu-id="23fb0-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="23fb0-118">Για να στοχεύσετε μια συγκεκριμένη πολιτική σε κάποιον, προσθέστε τον στη λίστα **Συμπερίληψη.**</span><span class="sxs-lookup"><span data-stu-id="23fb0-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="23fb0-119">Για να βεβαιωθείτε ότι ένα άτομο παραλείπεται από την πολιτική, προσθέστε το στη λίστα **Εξαίρεση.**</span><span class="sxs-lookup"><span data-stu-id="23fb0-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="23fb0-120">Διαβάστε περισσότερα: [Τρόπος παρακολούθησης συσκευών πρόσβασης υπό όρους](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="23fb0-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

