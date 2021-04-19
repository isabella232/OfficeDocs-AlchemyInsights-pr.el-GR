---
title: Έλεγχος της πρόσβασης σε δημόσιους φακέλους με χρήση του Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816740"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="8ec27-102">Έλεγχος της πρόσβασης σε δημόσιους φακέλους με χρήση του Outlook</span><span class="sxs-lookup"><span data-stu-id="8ec27-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="8ec27-103">Για να ελέγξετε ποιοι χρήστες μπορούν να έχουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το Outlook:</span><span class="sxs-lookup"><span data-stu-id="8ec27-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="8ec27-104">Χρήση `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="8ec27-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="8ec27-105">$true: Να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους στο Outlook</span><span class="sxs-lookup"><span data-stu-id="8ec27-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="8ec27-106">$false: Αποτρέψτε την πρόσβαση των χρηστών σε δημόσιους φακέλους στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="8ec27-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="8ec27-107">Αυτή είναι η προεπιλεγμένη τιμή.</span><span class="sxs-lookup"><span data-stu-id="8ec27-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="8ec27-108">Σημείωση: Αυτή η διαδικασία μπορεί να ελέγξει μόνο τις συνδέσεις με υπολογιστές-πελάτες του Outlook για Windows.</span><span class="sxs-lookup"><span data-stu-id="8ec27-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="8ec27-109">Οι χρήστες μπορούν να συνεχίσουν να έχουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το OWA ή το Outlook για Mac.</span><span class="sxs-lookup"><span data-stu-id="8ec27-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="8ec27-110">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Ελεγχόμενες συνδέσεις σε δημόσιους φακέλους στο Outlook](https://aka.ms/controlpf) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="8ec27-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
