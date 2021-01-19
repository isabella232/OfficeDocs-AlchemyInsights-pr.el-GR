---
title: Ελεγκτής τομέα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901023"
---
# <a name="domain-controller"></a>Ελεγκτής τομέα

**Δεν είναι δυνατή η ενεργοποίηση του AAD-DS ή η ανάπτυξη αποτυγχάνει**

Για να επιλύσετε το ζήτημα της υπηρεσίας τομέα AD Azure (AAD-DS) που δεν έχει ενεργοποιηθεί ή δεν είναι δυνατό να αναπτυχθεί, εκτελέστε τα παρακάτω βήματα:

1. Εάν χρησιμοποιείτε ένα ήδη υπάρχον εικονικό δίκτυο, ανατρέξτε στο NSG για κανόνες που εμποδίζουν τις θύρες που απαιτούνται για το συγχρονισμό στο AAD-DS στην πύλη https://aka.ms/aadds-networking .
2. Ανατρέξτε στο θέμα εάν το μήνυμα σφάλματος απαντάται σε αυτόν τον οδηγό αντιμετώπισης προβλημάτων που είναι διαθέσιμος στο  https://aka.ms/aadds-troubleshoot-enable .
3. Δοκιμάστε να αναπτύξετε τις υπηρεσίες τομέα AD Azure σε ένα νέο εικονικό δίκτυο.
4. Ακολουθήστε τον οδηγό "γρήγορα αποτελέσματα" σχετικά με τον τρόπο ανάπτυξης του AAD-DS, το οποίο είναι διαθέσιμο στο [πρόγραμμα εκμάθησης για τη δημιουργία υπηρεσιών τομέα AD Azure](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Εάν αντιμετωπίζετε προβλήματα με την ανάπτυξη των υπηρεσιών τομέα AD Azure, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων των υπηρεσιών τομέα AD Azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) για την επίλυση συνηθισμένων σφαλμάτων, για να σας βοηθήσουν να εργαστείτε ξανά. 

**Δεν είναι δυνατή η απενεργοποίηση του AAD-DS**

Το AAD-DS δεν μπορεί να διακοπεί προσωρινά. Εάν θέλετε να διακόψετε τη χρήση του διαχειριζόμενου τομέα σας, πρέπει να διαγραφεί.

Εάν αντιμετωπίζετε προβλήματα, για να επιλύσετε συνηθισμένα μηνύματα σφάλματος και για τα συσχετισμένα βήματα αντιμετώπισης προβλημάτων που θα σας βοηθήσουν να εκτελέσετε ξανά τα πράγματα, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων υπηρεσιών τομέα του Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
