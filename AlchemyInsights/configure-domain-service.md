---
title: Ρύθμιση παραμέτρων υπηρεσίας τομέα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885223"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Δεν είναι δυνατή η ενεργοποίηση του AAD-DS ή η ανάπτυξη αποτυγχάνει

Για να επιλύσετε το ζήτημα της υπηρεσίας τομέα AD Azure (AAD-DS) που δεν έχει ενεργοποιηθεί ή δεν είναι δυνατό να αναπτυχθεί, εκτελέστε τα παρακάτω βήματα:

1. Εάν χρησιμοποιείτε ένα ήδη υπάρχον εικονικό δίκτυο, ανατρέξτε στο NSG για κανόνες που εμποδίζουν τις θύρες που απαιτούνται για το συγχρονισμό στο AAD-DS στην πύλη https://aka.ms/aadds-networking .
2. Ανατρέξτε στο θέμα εάν το μήνυμα σφάλματος απαντάται σε αυτόν τον οδηγό αντιμετώπισης προβλημάτων που είναι διαθέσιμος στο  https://aka.ms/aadds-troubleshoot-enable .
3. Δοκιμάστε να αναπτύξετε τις υπηρεσίες τομέα AD Azure σε ένα νέο εικονικό δίκτυο.
4. Ακολουθήστε τον οδηγό "γρήγορα αποτελέσματα" σχετικά με τον τρόπο ανάπτυξης του AAD-DS: [δημιουργία και ρύθμιση παραμέτρων των υπηρεσιών τομέα AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Εάν αντιμετωπίζετε προβλήματα με την ανάπτυξη των υπηρεσιών τομέα AD Azure, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων των υπηρεσιών τομέα AD Azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) για την επίλυση συνηθισμένων σφαλμάτων, για να σας βοηθήσουν να εργαστείτε ξανά. 

**Δεν είναι δυνατή η απενεργοποίηση του AAD-DS**

Το AAD-DS δεν μπορεί να διακοπεί προσωρινά. Εάν θέλετε να διακόψετε τη χρήση του διαχειριζόμενου τομέα σας, πρέπει να διαγραφεί.
Για να διαγράψετε τον διαχειριζόμενο τομέα σας, ανατρέξτε στο θέμα [Διαγραφή υπηρεσίας τομέα AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



