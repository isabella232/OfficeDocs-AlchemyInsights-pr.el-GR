---
title: Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291188"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="7a40a-102">Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="7a40a-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="7a40a-103">Για να αντιμετωπίσετε ζητήματα όπου δεν υπάρχουν κωδικοί πρόσβασης είναι συγχρονισμένη με σύνδεση AD Azure έκδοση 1.1.614.0 ή νεότερη έκδοση:</span><span class="sxs-lookup"><span data-stu-id="7a40a-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="7a40a-104">Ανοίξτε μια νέα περίοδο λειτουργίας του Windows PowerShell στο διακομιστή σας σύνδεση AD Azure με την επιλογή " **Εκτέλεση ως διαχειριστής** ".</span><span class="sxs-lookup"><span data-stu-id="7a40a-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="7a40a-105">Εκτέλεση **σύνολο-της πολιτικής εκτέλεσης του RemoteSigned** ή **σύνολο-της πολιτικής εκτέλεσης του χωρίς περιορισμούς**.</span><span class="sxs-lookup"><span data-stu-id="7a40a-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="7a40a-106">Ξεκινήστε τον Οδηγό Azure AD σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="7a40a-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="7a40a-107">Μεταβείτε το \*\* πρόσθετες εργασίες \*\* σελίδα, επιλέξτε \*\* αντιμετώπιση \*\*, και κάντε κλικ στο κουμπί **Επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="7a40a-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="7a40a-108">Στη σελίδα "Αντιμετώπιση προβλημάτων", κάντε κλικ στο μενού **εκκίνησης για να ξεκινήσετε την αντιμετώπιση προβλημάτων** σε PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7a40a-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="7a40a-109">Το κύριο μενού, επιλέξτε **Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης**.</span><span class="sxs-lookup"><span data-stu-id="7a40a-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="7a40a-110">Στο υπο-μενού, επιλέξτε **Συγχρονισμός κωδικού πρόσβασης δεν λειτουργεί καθόλου**.</span><span class="sxs-lookup"><span data-stu-id="7a40a-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="7a40a-111">**Κατανόηση των αποτελεσμάτων της αντιμετώπισης προβλημάτων εργασίας**</span><span class="sxs-lookup"><span data-stu-id="7a40a-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="7a40a-112">Αντιμετώπιση προβλημάτων εργασίας εκτελούν τους ακόλουθους ελέγχους:</span><span class="sxs-lookup"><span data-stu-id="7a40a-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="7a40a-113">Επικυρώνει ότι είναι ενεργοποιημένη η δυνατότητα συγχρονισμού του κωδικού πρόσβασης για σας μισθωτών Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7a40a-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="7a40a-114">Επικυρώνει ότι ο διακομιστής σύνδεση AD Azure δεν είναι στην υλοποίηση της λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="7a40a-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="7a40a-115">Για κάθε υπάρχουσα εσωτερικής εγκατάστασης υπηρεσίας καταλόγου Active Directory connector (που αντιστοιχεί σε ένα υπάρχον σύμπλεγμα δομών της υπηρεσίας καταλόγου Active Directory):</span><span class="sxs-lookup"><span data-stu-id="7a40a-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="7a40a-116">Επικυρώνει ότι είναι ενεργοποιημένη η δυνατότητα συγχρονισμού του κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="7a40a-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="7a40a-117">Πραγματοποιεί αναζήτηση για συμβάντα παλμού συγχρονισμού κωδικού πρόσβασης στα αρχεία καταγραφής συμβάντων εφαρμογών των Windows.</span><span class="sxs-lookup"><span data-stu-id="7a40a-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="7a40a-118">Για κάθε τομέα της υπηρεσίας καταλόγου Active Directory στην περιοχή της σύνδεσης της υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης:</span><span class="sxs-lookup"><span data-stu-id="7a40a-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="7a40a-119">Επικυρώνει ότι ο τομέας είναι προσπελάσιμες από το διακομιστή Azure AD σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="7a40a-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="7a40a-120">Επικυρώνει ότι τους λογαριασμούς υπηρεσιών τομέα Active Directory (AD DS) που χρησιμοποιούνται από την υπηρεσία σύνδεσης υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης έχει το σωστό όνομα χρήστη, κωδικό πρόσβασης και δικαιώματα που απαιτούνται για το συγχρονισμό κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="7a40a-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="7a40a-121">Για περισσότερη βοήθεια αντιμετώπισης προβλημάτων συγχρονισμού κωδικού πρόσβασης, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων κωδικού πρόσβασης συγχρονισμού με σύνδεση AD Azure συγχρονισμού](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="7a40a-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

