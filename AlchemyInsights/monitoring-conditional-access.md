---
title: Παρακολούθηση υπό όρους πρόσβασης
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291554"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="b1eea-102">Παρακολούθηση υπό όρους πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="b1eea-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="b1eea-p101">Οι χρήστες ως προορισμός με πρόσβαση υπό όρους θα λαμβάνουν ενός μηνύματος ηλεκτρονικού ταχυδρομείου ειδοποίησης, εφόσον δεν πληρούν τις απαιτήσεις πρόσβασης της εταιρείας σας. Για να επιλύσετε, συνιστούμε μία ή περισσότερες από τις παρακάτω λύσεις:</span><span class="sxs-lookup"><span data-stu-id="b1eea-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="b1eea-p102">Εάν η συσκευή θεωρείται ότι συμμετέχουν, να συμβουλεύσετε το χρήστη για να μεταβείτε στην εφαρμογή πύλη εταιρείας και βεβαιωθείτε ότι εμφανίζεται στην πύλη εταιρείας. Σε αντίθετη περίπτωση, ο χρήστης πρέπει να εγγραφεί στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="b1eea-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="b1eea-p103">Στην πύλη Azure Μετάβαση σε **Intune \> συμμόρφωση της συσκευής**. Κάτω από **την οθόνη** , κάντε κλικ στο κουμπί **συμμόρφωση της συσκευής**. Προβολή της έκθεση συμμόρφωσης συσκευή για να βεβαιωθείτε ότι η συσκευή του χρήστη έχει σημανθεί ως συμβατή με.</span><span class="sxs-lookup"><span data-stu-id="b1eea-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="b1eea-p104">Στην πύλη Azure Μετάβαση σε **Intune \> συμμόρφωση της συσκευής**. Στην περιοχή **Διαχείριση**, κάντε κλικ στο κουμπί " **πολιτικές**". Στη λίστα των πολιτικών συμμόρφωσης, βεβαιωθείτε ότι στη συσκευή του χρήστη αντιστοιχίζεται ένα προφίλ. Εάν έχει εκχωρηθεί σε κανένα προφίλ, Intune δεν θα είναι σε θέση να επιβεβαιώσετε την κατάσταση συμμόρφωσης της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="b1eea-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="b1eea-114">Επεξεργασία ανάθεσης υπό όρους πρόσβασης του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="b1eea-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="b1eea-115">Στην πύλη Azure Μετάβαση σε **Intune \> υπό όρους πρόσβασης \> πολιτικές**</span><span class="sxs-lookup"><span data-stu-id="b1eea-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="b1eea-116">Επιλέξτε μια πολιτική από τη λίστα</span><span class="sxs-lookup"><span data-stu-id="b1eea-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="b1eea-117">Κάντε κλικ στην επιλογή **χρήστες και ομάδες**</span><span class="sxs-lookup"><span data-stu-id="b1eea-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="b1eea-p105">Για να στοχεύσετε μια συγκεκριμένη πολιτική σε κάποιον, μπορείτε να τις προσθέσετε στη λίστα **συμπερίληψης** . Για να εξασφαλίσετε ότι ένα άτομο παραλείπεται από την πολιτική, μπορείτε να τις προσθέσετε στη λίστα **εξαίρεση** .</span><span class="sxs-lookup"><span data-stu-id="b1eea-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="b1eea-120">Περισσότερες πληροφορίες: [Τρόπος συσκευές οθόνης υπό όρους πρόσβασης](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="b1eea-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

