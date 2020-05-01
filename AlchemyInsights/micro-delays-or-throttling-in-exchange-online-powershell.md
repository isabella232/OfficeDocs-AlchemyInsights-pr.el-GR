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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Μικροκαθυστερήσεις ή περιορισμός αριθμού αιτήσεων στο Exchange Online PowerShell

Μπορεί να δείτε προειδοποιήσεις “Εφαρμόστηκαν μικροκαθυστερήσεις” ή καθυστερήσεις κατά την εκτέλεση δεσμών ενεργειών και cmdlet στο Exchange Online. Εδώ θα βρείτε δύο προτάσεις που σχετίζονται με αυτό:

- Δοκιμάστε να χρησιμοποιήσετε τη [Λειτουργική μονάδα Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), η οποία περιλαμβάνει CMDlet που βασίζονται στο REST API και έχουν σημαντικά καλύτερες επιδόσεις. Αυτό μπορεί να αποτελεί μια εξαιρετική λύση για πολλές εντολές CMDlet Get που χρησιμοποιούνται συχνά.
- Εάν θέλετε να χρησιμοποιήσετε CMDlet που δεν καλύπτονται ακόμη από τη λειτουργική μονάδα v2, ανατρέξτε στο θέμα [Εκτέλεση cmdlet του PowerShell για μεγάλο αριθμό χρηστών στο Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), το οποίο αναφέρεται στο πώς μπορείτε να παρακάμψετε τα αναμενόμενα όρια περιορισμού αριθμού αιτήσεων του PowerShell στο Exchange Online.
