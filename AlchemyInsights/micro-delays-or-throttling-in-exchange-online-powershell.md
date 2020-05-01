---
title: Μικροκαθυστερήσεις ή περιορισμός αριθμού αιτήσεων στο Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947913"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="977e4-102">Μικροκαθυστερήσεις ή περιορισμός αριθμού αιτήσεων στο Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="977e4-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="977e4-103">Μπορεί να δείτε προειδοποιήσεις “Εφαρμόστηκαν μικροκαθυστερήσεις” ή καθυστερήσεις κατά την εκτέλεση δεσμών ενεργειών και cmdlet στο Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="977e4-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="977e4-104">Εδώ θα βρείτε δύο προτάσεις που σχετίζονται με αυτό:</span><span class="sxs-lookup"><span data-stu-id="977e4-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="977e4-105">Δοκιμάστε να χρησιμοποιήσετε τη [Λειτουργική μονάδα Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), η οποία περιλαμβάνει CMDlet που βασίζονται στο REST API και έχουν σημαντικά καλύτερες επιδόσεις.</span><span class="sxs-lookup"><span data-stu-id="977e4-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="977e4-106">Αυτό μπορεί να αποτελεί μια εξαιρετική λύση για πολλές εντολές CMDlet Get που χρησιμοποιούνται συχνά.</span><span class="sxs-lookup"><span data-stu-id="977e4-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="977e4-107">Εάν θέλετε να χρησιμοποιήσετε CMDlet που δεν καλύπτονται ακόμη από τη λειτουργική μονάδα v2, ανατρέξτε στο θέμα [Εκτέλεση cmdlet του PowerShell για μεγάλο αριθμό χρηστών στο Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), το οποίο αναφέρεται στο πώς μπορείτε να παρακάμψετε τα αναμενόμενα όρια περιορισμού αριθμού αιτήσεων του PowerShell στο Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="977e4-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
