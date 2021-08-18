---
title: Προσδιορισμός δραστηριότητας κανόνα εισερχομένων σε αρχεία καταγραφής ελέγχου
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331123"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Προσδιορισμός δραστηριότητας κανόνα εισερχομένων σε αρχεία καταγραφής ελέγχου

Μπορείτε να χρησιμοποιήσετε την αναζήτηση αρχείου καταγραφής ελέγχου στο Κέντρο συμμόρφωσης Microsoft 365 για να προβάλετε συμβάντα κανόνα εισερχομένων (δημιουργία, τροποποίηση και διαγραφή κανόνων εισερχομένων).

1. Κάντε ένα από τα παρακάτω βήματα:
   - Στο πλαίσιο <https://compliance.microsoft.com> Κέντρο συμμόρφωσης Microsoft 365, μεταβείτε στην ομάδα **"Έλεγχος** \> **λύσεων".** Εναλλακτικά, για να μεταβείτε απευθείας στη **σελίδα ελέγχου,** χρησιμοποιήστε <https://compliance.microsoft.com/auditlogsearch> το .
   - Στην πύλη Microsoft 365 Defender, <https://security.microsoft.com> μεταβείτε στην τοποθεσία **"Έλεγχος".** Εναλλακτικά, για να μεταβείτε απευθείας στη **σελίδα ελέγχου,** χρησιμοποιήστε <https://security.microsoft.com/auditlogsearch> το .

2. Στην καρτέλα **"Αναζήτηση"** της σελίδας **"Έλεγχος",** ρυθμίστε τις παραμέτρους των ακόλουθων ρυθμίσεων:
   - **Εύρος ημερομηνιών και ώρας:** Επιλέξτε το εύρος ημερομηνίας/ώρας στα **πλαίσια "Έναρξη"** **και "Λήξη".**
   - **Δραστηριότητες:** Επιλέξτε μία ή περισσότερες από τις παρακάτω τιμές:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App.**
     - **Ενημέρωση κανόνων εισερχομένων από Outlook πελάτη**

3. Όταν τελειώσετε, κάντε κλικ στην επιλογή **"Αναζήτηση".** Οι δραστηριότητες εμφανίζονται στη νέα **σελίδα αναζήτησης ελέγχου.**

4. Επιλέξτε μια δραστηριότητα στα αποτελέσματα για να ανοίξετε το αναδυόμενο στοιχείο λεπτομερειών. Οι πληροφορίες σχετικά με τις ρυθμίσεις κανόνα εισερχομένων εμφανίζονται στο πεδίο **"Παράμετροι".**

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Προσδιορισμός εάν ένας χρήστης δημιούργησε έναν κανόνα εισερχομένων.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
