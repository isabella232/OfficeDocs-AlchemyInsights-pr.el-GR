---
title: Δεν είναι δυνατή η πρόσβαση σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812547"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="a6718-102">Το Outlook δεν μπορεί να συνδεθεί με δημόσιους φακέλους</span><span class="sxs-lookup"><span data-stu-id="a6718-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="a6718-103">Εάν η πρόσβαση στο δημόσιο φάκελο δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="a6718-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="a6718-104">Συνδεθείτε στο έξω PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στο λογαριασμό χρήστη του προβλήματος ώστε να ταιριάζει με την παράμετρο σε έναν λογαριασμό χρήστη που λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="a6718-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="a6718-105">Παράδειγμα</span><span class="sxs-lookup"><span data-stu-id="a6718-105">Example:</span></span>

<span data-ttu-id="a6718-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="a6718-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="a6718-107">Ορίστε-γραμματοκιβώτιο ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="a6718-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="a6718-108">Περιμένετε τουλάχιστον μία ώρα για να ισχύσει η αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="a6718-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="a6718-109">Εάν το πρόβλημα παραμένει, ακολουθήστε [αυτή τη διαδικασία](https://aka.ms/pfcte) για την αντιμετώπιση προβλημάτων πρόσβασης δημόσιου φακέλου με χρήση του Outlook.</span><span class="sxs-lookup"><span data-stu-id="a6718-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="a6718-110">**Για να ελέγξετε ποιοι χρήστες μπορούν να έχουν πρόσβαση σε δημόσιους φακέλους με χρήση του Outlook**:</span><span class="sxs-lookup"><span data-stu-id="a6718-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="a6718-111">Χρήση του συνόλου-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE ή $FALSE</span><span class="sxs-lookup"><span data-stu-id="a6718-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="a6718-112">$true: να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους στο Outlook</span><span class="sxs-lookup"><span data-stu-id="a6718-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="a6718-113">$false: αποτροπή πρόσβασης χρηστών σε δημόσιους φακέλους στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="a6718-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="a6718-114">Αυτή είναι η προεπιλεγμένη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a6718-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="a6718-115">Ορίστε-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="a6718-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="a6718-116">**Σημείωση** Αυτή η διαδικασία μπορεί να ελέγχει τις συνδέσεις μόνο με το Outlook για υπολογιστές-πελάτες των Windows.</span><span class="sxs-lookup"><span data-stu-id="a6718-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="a6718-117">Ένας χρήστης μπορεί να συνεχίσει την πρόσβαση σε δημόσιους φακέλους με χρήση του OWA ή του Outlook για Mac.</span><span class="sxs-lookup"><span data-stu-id="a6718-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="a6718-118">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα ανακοίνωση υποστήριξης για ελεγχόμενες συνδέσεις σε δημόσιους φακέλους στο Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="a6718-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>