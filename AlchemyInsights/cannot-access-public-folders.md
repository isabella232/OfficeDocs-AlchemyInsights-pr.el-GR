---
title: Δεν είναι δυνατή η πρόσβαση σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341403"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="807c2-102">Το Outlook δεν μπορεί να συνδεθεί με δημόσιους φακέλους</span><span class="sxs-lookup"><span data-stu-id="807c2-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="807c2-103">Εάν η πρόσβαση στο δημόσιο φάκελο δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="807c2-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="807c2-104">Συνδεθείτε στο έξω PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στο λογαριασμό χρήστη του προβλήματος ώστε να ταιριάζει με την παράμετρο σε έναν λογαριασμό χρήστη που λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="807c2-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="807c2-105">Παράδειγμα</span><span class="sxs-lookup"><span data-stu-id="807c2-105">Example:</span></span>

<span data-ttu-id="807c2-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="807c2-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="807c2-107">Ορίστε-γραμματοκιβώτιο ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="807c2-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="807c2-108">Περιμένετε τουλάχιστον μία ώρα για να ισχύσει η αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="807c2-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="807c2-109">Εάν το πρόβλημα παραμένει, ακολουθήστε [αυτή τη διαδικασία](https://aka.ms/pfcte) για την αντιμετώπιση προβλημάτων πρόσβασης δημόσιου φακέλου με χρήση του Outlook.</span><span class="sxs-lookup"><span data-stu-id="807c2-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="807c2-110">**Για να ελέγξετε ποιοι χρήστες μπορούν να έχουν πρόσβαση σε δημόσιους φακέλους με χρήση του Outlook**:</span><span class="sxs-lookup"><span data-stu-id="807c2-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="807c2-111">Χρήση του συνόλου-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE ή $FALSE</span><span class="sxs-lookup"><span data-stu-id="807c2-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="807c2-112">$true: να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους στο Outlook</span><span class="sxs-lookup"><span data-stu-id="807c2-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="807c2-113">$false: αποτροπή πρόσβασης χρηστών σε δημόσιους φακέλους στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="807c2-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="807c2-114">Αυτή είναι η προεπιλεγμένη τιμή.</span><span class="sxs-lookup"><span data-stu-id="807c2-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="807c2-115">Ορίστε-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="807c2-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="807c2-116">**Σημείωση** Αυτή η διαδικασία μπορεί να ελέγχει τις συνδέσεις μόνο με το Outlook για υπολογιστές-πελάτες των Windows.</span><span class="sxs-lookup"><span data-stu-id="807c2-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="807c2-117">Ένας χρήστης μπορεί να συνεχίσει την πρόσβαση σε δημόσιους φακέλους με χρήση του OWA ή του Outlook για Mac.</span><span class="sxs-lookup"><span data-stu-id="807c2-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="807c2-118">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα ανακοίνωση υποστήριξης για ελεγχόμενες συνδέσεις σε δημόσιους φακέλους στο Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="807c2-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>