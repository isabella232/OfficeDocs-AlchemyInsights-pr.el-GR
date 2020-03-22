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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891749"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="e3d5f-102">Το Outlook δεν είναι δυνατό να συνδεθεί με δημόσιους φακέλους</span><span class="sxs-lookup"><span data-stu-id="e3d5f-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="e3d5f-103">Εάν η πρόσβαση σε δημόσιους φακέλους δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="e3d5f-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="e3d5f-104">Συνδεθείτε με το EXO PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στο λογαριασμό χρήστη προβλήματος, ώστε να ταιριάζει με την παράμετρο σε ένα λογαριασμό χρήστη που λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="e3d5f-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="e3d5f-105">Παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="e3d5f-105">Example:</span></span>

<span data-ttu-id="e3d5f-106">Λειτουργικός χρήστης του γραμματοκιβωτίου get | ft προεπιλεγμένοδημόσιο φάκελογραμματοκιβώτιο, αποτελεσματικόδημόσιο φάκελογραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="e3d5f-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="e3d5f-107">Set-Γραμματοκιβώτιο ProblemUser -Προεπιλεγμένη τιμήδημόσιου φακέλουΓραμματοκιβώτιο \<από την προηγούμενη εντολή></span><span class="sxs-lookup"><span data-stu-id="e3d5f-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="e3d5f-108">Περιμένετε τουλάχιστον μία ώρα για να εφαρμοστεί η αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="e3d5f-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="e3d5f-109">Εάν το ζήτημα παραμένει, ακολουθήστε [αυτήν τη διαδικασία](https://aka.ms/pfcte) για να αντιμετωπίσετε ζητήματα πρόσβασης σε δημόσιους φακέλους χρησιμοποιώντας το Outlook.</span><span class="sxs-lookup"><span data-stu-id="e3d5f-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>