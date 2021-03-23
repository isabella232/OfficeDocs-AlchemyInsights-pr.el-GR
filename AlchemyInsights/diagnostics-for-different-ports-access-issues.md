---
title: Διαγνωστικά για προβλήματα πρόσβασης σε διαφορετικές θύρες
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035784"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Διαγνωστικά για προβλήματα πρόσβασης σε διαφορετικές θύρες

Για να επιλύσετε τα διάφορα προβλήματα πρόσβασης σε θύρα, ακολουθήστε τα παρακάτω βήματα:

1. Διακόψτε/διακόψτε την εκχώρηση της εικονικής μηχανής (VM) από την πύλη, επανεκκινήστε την εικονική μηχανή και ελέγξτε ξανά. 
2. Ελέγξτε τις ρυθμίσεις δικτύου της εικονικής μηχανής για να προσδιορίσετε εάν έχετε ομάδες ασφαλείας δικτύου (NSG) που εμποδίζουν την κυκλοφορία. Μπορείτε επίσης να χρησιμοποιήσετε το εργαλείο επαλήθευσης ροής [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) παρακολούθησης δικτύου για να ελέγξετε για NSG που εμποδίζουν την κυκλοφορία, δρομολογήσεις του User-Defined (UDR) που δρομολογούν ξανά την κυκλοφορία σας στην εσωτερική εγκατάσταση ('Προεπιλεγμένη δρομολόγηση' 0.0.0.0/0) ή σε μια συσκευή δικτύου.
Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα αφού δοκιμάσετε τα παραπάνω βήματα, δώστε το όνομα της εικονικής μηχανής και τη θύρα TCP στην οποία προσπαθείτε να στείλετε αλληλογραφία για περαιτέρω διάγνωση.

**Προτεινόμενα έγγραφα**

[Περιορισμοί και συστάσεις για την αποστολή εξερχόμενων μηνυμάτων ηλεκτρονικού ταχυδρομείου μέσω της θύρας 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)