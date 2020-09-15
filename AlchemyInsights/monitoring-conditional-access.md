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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702903"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a9a40-102">Παρακολούθηση της πρόσβασης υπό όρους για το Exchange</span><span class="sxs-lookup"><span data-stu-id="a9a40-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a9a40-103">Οι χρήστες που στοχεύουν στην πρόσβαση υπό όρους θα λαμβάνουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου ειδοποίησης, εάν δεν ικανοποιούν τις απαιτήσεις πρόσβασης της εταιρείας σας.</span><span class="sxs-lookup"><span data-stu-id="a9a40-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a9a40-104">Για να επιλύσετε αυτό το πλαίσιο, συνιστούμε μία ή περισσότερες από τις ακόλουθες λύσεις:</span><span class="sxs-lookup"><span data-stu-id="a9a40-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a9a40-105">Εάν τεκμαίρεται ότι η συσκευή είναι εγγεγραμμένη, ενημερώστε το χρήστη για να μεταβείτε στην εφαρμογή εταιρεία πύλης και βεβαιωθείτε ότι εμφανίζεται στην πύλη της εταιρείας.</span><span class="sxs-lookup"><span data-stu-id="a9a40-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a9a40-106">Εάν δεν το κάνει, ο χρήστης θα πρέπει να εγγραφεί στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="a9a40-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a9a40-107">Στην πύλη Azure, μεταβείτε στη \*\* \> συμμόρφωση συσκευής του Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="a9a40-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a9a40-108">Στην περιοχή **Παρακολούθηση** , κάντε κλικ στην επιλογή **συμμόρφωση συσκευής**.</span><span class="sxs-lookup"><span data-stu-id="a9a40-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="a9a40-109">Προβάλετε την αναφορά συμμόρφωσης της συσκευής σας για να επαληθεύσετε ότι η συσκευή του χρήστη έχει επισημανθεί ως συμβατή.</span><span class="sxs-lookup"><span data-stu-id="a9a40-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a9a40-110">Στην πύλη Azure, μεταβείτε στη \*\* \> συμμόρφωση συσκευής του Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="a9a40-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a9a40-111">Στην περιοχή **Διαχείριση**, κάντε κλικ στην επιλογή **πολιτικές**.</span><span class="sxs-lookup"><span data-stu-id="a9a40-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="a9a40-112">Στη λίστα των πολιτικών συμμόρφωσης, επαληθεύστε ότι ένα προφίλ έχει εκχωρηθεί στη συσκευή του χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="a9a40-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a9a40-113">Εάν δεν έχει εκχωρηθεί κανένα προφίλ, τότε το Intune δεν θα έχει τη δυνατότητα να επιβεβαιώσει την κατάσταση συμμόρφωσης της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="a9a40-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a9a40-114">Επεξεργασία της εκχώρησης πρόσβασης υπό όρους του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="a9a40-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a9a40-115">Στην πύλη Azure, μεταβείτε στις \*\* \> \> πολιτικές πρόσβασης υπό όρους του Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="a9a40-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a9a40-116">Επιλογή μιας πολιτικής από τη λίστα</span><span class="sxs-lookup"><span data-stu-id="a9a40-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a9a40-117">Κάντε κλικ στην επιλογή **χρήστες και ομάδες**</span><span class="sxs-lookup"><span data-stu-id="a9a40-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a9a40-118">Για να στοχεύσετε μια συγκεκριμένη πολιτική σε κάποιον, προσθέστε τον στη λίστα **Συμπερίληψη** .</span><span class="sxs-lookup"><span data-stu-id="a9a40-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="a9a40-119">Για να εξασφαλίσετε ότι ένα άτομο παραλείπεται από την πολιτική, προσθέστε το στη λίστα **εξαίρεσης** .</span><span class="sxs-lookup"><span data-stu-id="a9a40-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a9a40-120">Διαβάστε περισσότερα: [Πώς να παρακολουθείτε τις συσκευές πρόσβασης υπό όρους](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a9a40-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

