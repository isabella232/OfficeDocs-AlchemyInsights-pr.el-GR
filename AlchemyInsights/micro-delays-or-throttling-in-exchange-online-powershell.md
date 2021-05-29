---
title: Μικροκαθυστερήσεις ή περιορισμός αριθμού αιτήσεων στο Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702126"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="c0401-102">Μικροκαθυστερήσεις ή περιορισμός αριθμού αιτήσεων στο Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0401-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="c0401-103">Μπορεί να δείτε προειδοποιήσεις “Εφαρμόστηκαν μικροκαθυστερήσεις” ή καθυστερήσεις κατά την εκτέλεση δεσμών ενεργειών και cmdlet στο Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c0401-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="c0401-104">Ακολουθούν μερικές προτάσεις για να επιλύσετε αυτό το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="c0401-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="c0401-105">Εκτελέστε τα διαγνωστικά μας για να χαλαρώσετε τις πολιτικές περιορισμού του PowerShell του μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="c0401-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="c0401-106">Αυτή η λύση θα λύσει το πρόβλημα για τους περισσότερους.</span><span class="sxs-lookup"><span data-stu-id="c0401-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="c0401-107">Εάν το πρόβλημα εξακολουθεί να μην επιλυθεί, [χρησιμοποιήστε τη λειτουργική μονάδα Exchange Online v2 PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)η οποία περιλαμβάνει CMDlet που βασίζονται σε REST API και είναι πολύ πιο αποτελεσματικά.</span><span class="sxs-lookup"><span data-stu-id="c0401-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="c0401-108">Αυτό μπορεί να αποτελεί μια εξαιρετική λύση για πολλές εντολές CMDlet Get που χρησιμοποιούνται συχνά.</span><span class="sxs-lookup"><span data-stu-id="c0401-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="c0401-109">Εάν θέλετε να χρησιμοποιήσετε CMDlet που δεν καλύπτονται στη λειτουργική μονάδα v2, ανατρέξτε στο θέμα Εκτέλεση [cmdlet του PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)για μεγάλο αριθμό χρηστών στο Office 365, το οποίο μιλά για τον τρόπο με τον οποίο μπορείτε να περιηγηθείτε στα όρια περιορισμού του PowerShell στο Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c0401-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
