---
title: Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732510"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="75aa8-102">Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="75aa8-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="75aa8-103">Για να αντιμετωπίσετε ζητήματα όπου δεν συγχρονίζονται κωδικοί πρόσβασης με το Azure AD Connect έκδοση 1.1.614.0 ή νεότερη έκδοση:</span><span class="sxs-lookup"><span data-stu-id="75aa8-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="75aa8-104">Ανοίξτε μια νέα περίοδο λειτουργίας του Windows PowerShell στο διακομιστή Azure AD Connect με την επιλογή **"Εκτέλεση ως διαχειριστής".**</span><span class="sxs-lookup"><span data-stu-id="75aa8-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="75aa8-105">Εκτέλεση **πολιτικής εκτέλεσης συνόλου απομακρυσμένης υπογραφής** ή **πολιτικής εκτέλεσης συνόλου χωρίς περιορισμούς**.</span><span class="sxs-lookup"><span data-stu-id="75aa8-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="75aa8-106">Ξεκινήστε τον "Οδηγό σύνδεσης Azure AD".</span><span class="sxs-lookup"><span data-stu-id="75aa8-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="75aa8-107">Μεταβείτε στη σελίδα **"Πρόσθετες εργασίες",** επιλέξτε **"Αντιμετώπιση προβλημάτων"** και κάντε κλικ στο κουμπί **"Επόμενο"**.</span><span class="sxs-lookup"><span data-stu-id="75aa8-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="75aa8-108">Στη σελίδα Αντιμετώπιση προβλημάτων, κάντε κλικ στην επιλογή Εκκίνηση για να ξεκινήσετε το μενού **αντιμετώπισης προβλημάτων** στο PowerShell.</span><span class="sxs-lookup"><span data-stu-id="75aa8-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="75aa8-109">Στο κύριο μενού, επιλέξτε **Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης**.</span><span class="sxs-lookup"><span data-stu-id="75aa8-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="75aa8-110">Στο υπομενού , επιλέξτε **Συγχρονισμός κωδικού πρόσβασης δεν λειτουργεί καθόλου**.</span><span class="sxs-lookup"><span data-stu-id="75aa8-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="75aa8-111">**Κατανόηση των αποτελεσμάτων της εργασίας αντιμετώπισης προβλημάτων**</span><span class="sxs-lookup"><span data-stu-id="75aa8-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="75aa8-112">Η εργασία αντιμετώπισης προβλημάτων εκτελεί τους ακόλουθους ελέγχους:</span><span class="sxs-lookup"><span data-stu-id="75aa8-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="75aa8-113">Επικυρώνει ότι η δυνατότητα συγχρονισμού κωδικού πρόσβασης είναι ενεργοποιημένη για τον μισθωτή Azure AD.</span><span class="sxs-lookup"><span data-stu-id="75aa8-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="75aa8-114">Επικυρώνει ότι ο διακομιστής Azure AD Connect δεν βρίσκεται σε κατάσταση ανασυγκρότησης.</span><span class="sxs-lookup"><span data-stu-id="75aa8-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="75aa8-115">Για κάθε υπάρχουσα σύνδεση active directory εσωτερικής εγκατάστασης (η οποία αντιστοιχεί σε ένα υπάρχον σύμπλεγμα δομών της υπηρεσίας καταλόγου Active Directory):</span><span class="sxs-lookup"><span data-stu-id="75aa8-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="75aa8-116">Επικυρώνει ότι είναι ενεργοποιημένη η δυνατότητα συγχρονισμού κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="75aa8-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="75aa8-117">Αναζητά συμβάντα παλμών συγχρονισμού κωδικού πρόσβασης στα αρχεία καταγραφής συμβάντων εφαρμογών των Windows.</span><span class="sxs-lookup"><span data-stu-id="75aa8-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="75aa8-118">Για κάθε τομέα της υπηρεσίας καταλόγου Active Directory κάτω από τη σύνδεση active directory εσωτερικής εγκατάστασης:</span><span class="sxs-lookup"><span data-stu-id="75aa8-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="75aa8-119">Επικυρώνει ότι ο τομέας είναι προσβάσιμος από το διακομιστή Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="75aa8-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="75aa8-120">Επικυρώνει ότι οι λογαριασμοί υπηρεσιών τομέα Active Directory (AD DS) που χρησιμοποιούνται από τη σύνδεση active directory εσωτερικής εγκατάστασης έχουν το σωστό όνομα χρήστη, κωδικό πρόσβασης και τα δικαιώματα που απαιτούνται για το συγχρονισμό κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="75aa8-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="75aa8-121">Για περισσότερη βοήθεια για την αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων συγχρονισμού κωδικών πρόσβασης με το συγχρονισμό Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="75aa8-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  