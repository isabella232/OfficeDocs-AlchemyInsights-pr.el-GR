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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098566"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Μικροκαθυστερήσεις ή περιορισμός αριθμού αιτήσεων στο Exchange Online PowerShell

Μπορεί να δείτε προειδοποιήσεις “Εφαρμόστηκαν μικροκαθυστερήσεις” ή καθυστερήσεις κατά την εκτέλεση δεσμών ενεργειών και cmdlet στο Exchange Online. Ακολουθούν μερικές προτάσεις για να επιλύσετε αυτό το πρόβλημα:

- Εκτελέστε τα διαγνωστικά μας για να χαλαρώσετε τις πολιτικές περιορισμού του PowerShell του μισθωτή σας. Αυτή η λύση θα λύσει το πρόβλημα για τους περισσότερους.
- Εάν το πρόβλημα εξακολουθεί να μην επιλυθεί, [χρησιμοποιήστε τη λειτουργική μονάδα Exchange Online v2 PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)η οποία περιλαμβάνει CMDlet που βασίζονται σε REST API και είναι πολύ πιο αποτελεσματικά. Αυτό μπορεί να αποτελεί μια εξαιρετική λύση για πολλές εντολές CMDlet Get που χρησιμοποιούνται συχνά.
- Εάν θέλετε να χρησιμοποιήσετε CMDlet που δεν καλύπτονται στη λειτουργική μονάδα v2, ανατρέξτε στο θέμα Εκτέλεση [cmdlet του PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)για μεγάλο αριθμό χρηστών στο Office 365, το οποίο μιλά για τον τρόπο με τον οποίο μπορείτε να περιηγηθείτε στα όρια περιορισμού του PowerShell στο Exchange Online.
