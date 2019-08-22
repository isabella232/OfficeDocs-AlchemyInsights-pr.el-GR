---
title: Παρακολούθηση υπό όρους πρόσβασης
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538743"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="2186c-102">Παρακολούθηση υπό όρους πρόσβασης για ανταλλαγή</span><span class="sxs-lookup"><span data-stu-id="2186c-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="2186c-103">Οι χρήστες ως προορισμός με πρόσβαση υπό όρους θα λαμβάνουν ενός μηνύματος ηλεκτρονικού ταχυδρομείου ειδοποίησης, εφόσον δεν πληρούν τις απαιτήσεις πρόσβασης της εταιρείας σας.</span><span class="sxs-lookup"><span data-stu-id="2186c-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="2186c-104">Για να επιλύσετε, συνιστούμε μία ή περισσότερες από τις παρακάτω λύσεις:</span><span class="sxs-lookup"><span data-stu-id="2186c-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="2186c-105">Εάν η συσκευή θεωρείται ότι συμμετέχουν, να συμβουλεύσετε το χρήστη για να μεταβείτε στην εφαρμογή πύλη εταιρείας και βεβαιωθείτε ότι εμφανίζεται στην πύλη εταιρείας.</span><span class="sxs-lookup"><span data-stu-id="2186c-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="2186c-106">Σε αντίθετη περίπτωση, ο χρήστης πρέπει να εγγραφεί στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="2186c-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="2186c-107">Στην πύλη Azure Μετάβαση σε **Intune \> συμμόρφωση της συσκευής**.</span><span class="sxs-lookup"><span data-stu-id="2186c-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2186c-108">Κάτω από **την οθόνη** , κάντε κλικ στο κουμπί **συμμόρφωση της συσκευής**.</span><span class="sxs-lookup"><span data-stu-id="2186c-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="2186c-109">Προβολή της έκθεση συμμόρφωσης συσκευή για να βεβαιωθείτε ότι η συσκευή του χρήστη έχει σημανθεί ως συμβατή με.</span><span class="sxs-lookup"><span data-stu-id="2186c-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="2186c-110">Στην πύλη Azure Μετάβαση σε **Intune \> συμμόρφωση της συσκευής**.</span><span class="sxs-lookup"><span data-stu-id="2186c-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2186c-111">Στην περιοχή **Διαχείριση**, κάντε κλικ στο κουμπί " **πολιτικές**".</span><span class="sxs-lookup"><span data-stu-id="2186c-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="2186c-112">Στη λίστα των πολιτικών συμμόρφωσης, βεβαιωθείτε ότι στη συσκευή του χρήστη αντιστοιχίζεται ένα προφίλ.</span><span class="sxs-lookup"><span data-stu-id="2186c-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="2186c-113">Εάν έχει εκχωρηθεί σε κανένα προφίλ, Intune δεν θα είναι σε θέση να επιβεβαιώσετε την κατάσταση συμμόρφωσης της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="2186c-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="2186c-114">Επεξεργασία ανάθεσης υπό όρους πρόσβασης του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="2186c-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="2186c-115">Στην πύλη Azure Μετάβαση σε **Intune \> υπό όρους πρόσβασης \> πολιτικές**</span><span class="sxs-lookup"><span data-stu-id="2186c-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="2186c-116">Επιλέξτε μια πολιτική από τη λίστα</span><span class="sxs-lookup"><span data-stu-id="2186c-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="2186c-117">Κάντε κλικ στην επιλογή **χρήστες και ομάδες**</span><span class="sxs-lookup"><span data-stu-id="2186c-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="2186c-118">Για να στοχεύσετε μια συγκεκριμένη πολιτική σε κάποιον, μπορείτε να τις προσθέσετε στη λίστα **συμπερίληψης** .</span><span class="sxs-lookup"><span data-stu-id="2186c-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="2186c-119">Για να εξασφαλίσετε ότι ένα άτομο παραλείπεται από την πολιτική, μπορείτε να τις προσθέσετε στη λίστα **εξαίρεση** .</span><span class="sxs-lookup"><span data-stu-id="2186c-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="2186c-120">Περισσότερες πληροφορίες: [Τρόπος συσκευές οθόνης υπό όρους πρόσβασης](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="2186c-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

