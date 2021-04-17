---
title: Δεν είναι δυνατή η πρόσβαση σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819512"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="541bd-102">Το Outlook δεν μπορεί να συνδεθεί σε δημόσιους φακέλους</span><span class="sxs-lookup"><span data-stu-id="541bd-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="541bd-103">Εάν η πρόσβαση σε δημόσιους φακέλους δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="541bd-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="541bd-104">Συνδεθείτε στο EXO PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στον λογαριασμό χρήστη προβλήματος, ώστε να ταιριάζει με την παράμετρο σε ένα λογαριασμό χρήστη που εργάζεται.</span><span class="sxs-lookup"><span data-stu-id="541bd-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="541bd-105">Παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="541bd-105">Example:</span></span>

<span data-ttu-id="541bd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="541bd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="541bd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="541bd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="541bd-108">Περιμένετε τουλάχιστον μία ώρα για να ισχύει η αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="541bd-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="541bd-109">Εάν το πρόβλημα παραμένει, ακολουθήστε αυτή τη διαδικασία για [να αντιμετωπίσετε](https://aka.ms/pfcte) προβλήματα πρόσβασης σε δημόσιους φακέλους χρησιμοποιώντας το Outlook.</span><span class="sxs-lookup"><span data-stu-id="541bd-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="541bd-110">**Για να ελέγξετε ποιοι χρήστες μπορούν να έχουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το Outlook:**</span><span class="sxs-lookup"><span data-stu-id="541bd-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="541bd-111">Χρήση Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ή $false</span><span class="sxs-lookup"><span data-stu-id="541bd-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="541bd-112">$true: Να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους στο Outlook</span><span class="sxs-lookup"><span data-stu-id="541bd-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="541bd-113">$false: Αποτρέψτε την πρόσβαση των χρηστών σε δημόσιους φακέλους στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="541bd-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="541bd-114">Αυτή είναι η προεπιλεγμένη τιμή.</span><span class="sxs-lookup"><span data-stu-id="541bd-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="541bd-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="541bd-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="541bd-116">**Σημείωση** Αυτή η διαδικασία μπορεί να ελέγξει τις συνδέσεις μόνο με προγράμματα-πελάτες του Outlook για υπολογιστή με Windows.</span><span class="sxs-lookup"><span data-stu-id="541bd-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="541bd-117">Ένας χρήστης μπορεί να συνεχίσει να έχει πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το OWA ή το Outlook για Mac.</span><span class="sxs-lookup"><span data-stu-id="541bd-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="541bd-118">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Ανακοίνωση υποστήριξης για ελεγχόμενες συνδέσεις σε δημόσιους φακέλους" στο Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="541bd-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>