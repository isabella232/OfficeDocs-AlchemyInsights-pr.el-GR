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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030902"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Διαγνωστικά για προβλήματα πρόσβασης σε διαφορετικές θύρες

Για να επιλύσετε τα διάφορα προβλήματα πρόσβασης σε θύρα, ακολουθήστε τα παρακάτω βήματα:

1. Διακόψτε/διακόψτε την εκχώρηση της εικονικής μηχανής (VM) από την πύλη, επανεκκινήστε την εικονική μηχανή και ελέγξτε ξανά. 
2. Ελέγξτε τις ρυθμίσεις δικτύου της εικονικής μηχανής για να προσδιορίσετε εάν έχετε ομάδες ασφαλείας δικτύου (NSG) που εμποδίζουν την κυκλοφορία. Μπορείτε επίσης να χρησιμοποιήσετε το εργαλείο επαλήθευσης ροής [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) παρακολούθησης δικτύου για να ελέγξετε για NSG που εμποδίζουν την κυκλοφορία, δρομολογήσεις του User-Defined (UDR) που δρομολογούν ξανά την κυκλοφορία σας στην εσωτερική εγκατάσταση ('Προεπιλεγμένη δρομολόγηση' 0.0.0.0/0) ή σε μια συσκευή δικτύου.
Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα αφού δοκιμάσετε τα παραπάνω βήματα, δώστε το όνομα της εικονικής μηχανής και τη θύρα TCP στην οποία προσπαθείτε να στείλετε αλληλογραφία για περαιτέρω διάγνωση.

**Προτεινόμενα έγγραφα**

[Περιορισμοί και συστάσεις για την αποστολή εξερχόμενων μηνυμάτων ηλεκτρονικού ταχυδρομείου μέσω της θύρας 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)