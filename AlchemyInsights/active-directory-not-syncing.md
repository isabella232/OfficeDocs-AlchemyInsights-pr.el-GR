---
title: Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314204"
---
# <a name="active-directory-not-syncing"></a>Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται

Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "δεν υπάρχει πρόσφατος συγχρονισμός" ή παρατηρήσετε ότι η κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office αναφέρει"Τελευταία συγχρονίζεται πριν από περισσότερες από 3 ημέρες", μπορεί να είναι ότι το AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκή δικαιώματα για την εκτέλεση συγχρονισμού.  

Η επανεγκατάσταση του AADConnect με χρήση των express ρυθμίσεων μπορεί να επιλύσει το πρόβλημα γρήγορα:

1. [Κάντε λήψη της πιο πρόσφατης έκδοσης του AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Το Azure AD Connect πρέπει να είναι εγκατεστημένο στον Windows Server 2012 ή σε νεότερες εκδόσεις. Αυτός ο διακομιστής πρέπει να είναι συνδεδεμένος με τομέα και μπορεί να είναι ελεγκτής τομέα ή διακομιστής-μέλος. Για μια πλήρη λίστα με τις απαιτήσεις Σύνδεση Azure AD και τα προαπαιτούμενα, εξετάστε τις [προϋποθέσεις για το Azure AD Σύνδεση.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσιών AADConnect, ανατρέξτε στο [θέμα Azure AD Σύνδεση: Λογαριασμοί και δικαιώματα.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
