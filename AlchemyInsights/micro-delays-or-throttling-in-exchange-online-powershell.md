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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868534"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Μικροκαθυστερήσεις ή περιορισμός αριθμού αιτήσεων στο Exchange Online PowerShell

Μπορεί να δείτε προειδοποιήσεις “Εφαρμόστηκαν μικροκαθυστερήσεις” ή καθυστερήσεις κατά την εκτέλεση δεσμών ενεργειών και cmdlet στο Exchange Online. Ακολουθούν μερικές προτάσεις για να επιλύσετε αυτό το πρόβλημα:

- Εκτελέστε τα διαγνωστικά μας για να χαλαρώσετε τις πολιτικές περιορισμού του PowerShell του μισθωτή σας. Αυτή η λύση θα λύσει το πρόβλημα για τους περισσότερους.
- Εάν το πρόβλημα εξακολουθεί να μην επιλυθεί, [χρησιμοποιήστε τη λειτουργική μονάδα Exchange Online v2 PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)η οποία περιλαμβάνει CMDlet που βασίζονται σε REST API και είναι πολύ πιο αποτελεσματικά. Αυτό μπορεί να αποτελεί μια εξαιρετική λύση για πολλές εντολές CMDlet Get που χρησιμοποιούνται συχνά.
- Εάν πρέπει να χρησιμοποιήσετε CMDlet που δεν καλύπτονται στη λειτουργική μονάδα v2, ανατρέξτε στο θέμα Εκτέλεση [cmdlet του PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)για μεγάλο αριθμό χρηστών στο Office 365, το οποίο μιλά για τον τρόπο με τον οποίο μπορείτε να περιηγηθείτε στα όρια περιορισμού του PowerShell στο Exchange Online.
