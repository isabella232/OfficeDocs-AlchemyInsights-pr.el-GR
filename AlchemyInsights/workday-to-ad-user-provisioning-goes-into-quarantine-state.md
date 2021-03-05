---
title: Οι εργάσιμες ημέρες έως ad user provisioning πηγαίνουν σε κατάσταση καραντίνας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481358"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Οι εργάσιμες ημέρες έως ad user provisioning πηγαίνουν σε κατάσταση καραντίνας

**Οι εργάσιμες ημέρες έως ad user provisioning πηγαίνουν σε κατάσταση καραντίνας και δεν δημιουργούνται χρήστες στο AD**

Η εργασία "Εργάσιμη ημέρα σε παροχή χρήστη AD" έχει τεθεί σε κατάσταση καραντίνας και τα αρχεία καταγραφής ελέγχου εμφανίζουν συμβάντα αποτυχίας εξαγωγής με το μήνυμα **σφάλματος: OperationsError-SvcErr: Παρουσιάστηκε σφάλμα λειτουργίας. Δεν έχει ρυθμιστεί καμία ανώτερη αναφορά για την υπηρεσία καταλόγου. Επομένως, η υπηρεσία καταλόγου δεν είναι σε θέση να εκδώσει συστάσεις σε αντικείμενα εκτός αυτού του δάσους.** Αυτό το σφάλμα εμφανίζεται συνήθως εάν η OU κοντέινερ της υπηρεσίας καταλόγου Active Directory δεν έχει οριστεί σωστά ή εάν υπάρχουν ζητήματα με την αντιστοίχιση παραστάσεων που χρησιμοποιείται για **το parentDistinguishedName.**

Ελέγξτε την προεπιλεγμένη OU για την **παράμετρο New Users** για λάθη κατά τη δημιουργία λάθη. Βεβαιωθείτε ότι η καθορισμένη OU υπάρχει ήδη στο AD σας. Εάν χρησιμοποιείτε το **parentDistinguishedName** στην αντιστοίχιση χαρακτηριστικών, βεβαιωθείτε ότι αυτό πάντα αξιολογείται σε ένα γνωστό κοντέινερ μέσα στον τομέα AD. Ελέγξτε το συμβάν Export στα αρχεία καταγραφής ελέγχου για να δείτε την τιμή που δημιουργήθηκε.

Για περισσότερες λεπτομέρειες σχετικά με τη ρύθμιση παραμέτρων της εργάσιμης ημέρας για την αυτοματοποιημένη παροχή, ανατρέξτε στο πρόγραμμα εκμάθησης: Ρύθμιση [παραμέτρων εργάσιμης ημέρας για αυτόματη προμήθεια από χρήστες.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

