---
title: Αναγνώριση δραστηριότητας κανόνα εισερχομένων σε αρχεία καταγραφής ελέγχου
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779051"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Αναγνώριση δραστηριότητας κανόνα εισερχομένων σε αρχεία καταγραφής ελέγχου

Μπορείτε να χρησιμοποιήσετε την αναζήτηση του αρχείου καταγραφής ελέγχου στο κέντρο συμμόρφωσης του Microsoft 365 Security & για να προβάλετε συμβάντα κανόνων εισερχομένων (δημιουργία, τροποποίηση και διαγραφή κανόνων εισερχομένων).

1. Συνδεθείτε στο [Κέντρο συμμόρφωσης & ασφαλείας του Microsoft 365](https://protection.office.com/).

2. Μεταβείτε στη σελίδα **Search**αναζήτησης του  >  **αρχείου καταγραφής ελέγχου** αναζήτησης.

3. Επιλέξτε την περιοχή ημερομηνιών στα πεδία ημερομηνία **έναρξης** και **ημερομηνία λήξης** .

4. Στην περιοχή **δραστηριότητες γραμματοκιβωτίου του Exchange**, επαληθεύστε ότι το πεδίο **δραστηριότητες** έχει την τιμή **Νέα-InboxRule Create/Modify/enable/disable Inbox Rule**.

5. Κάντε κλικ στην επιλογή **Αναζήτηση**.

Στα αποτελέσματα, επιλέξτε μια εγγραφή ελέγχου. Στο αναδυόμενο στοιχείο λεπτομερειών, κάντε κλικ στην επιλογή **περισσότερες πληροφορίες**. Οι πληροφορίες σχετικά με τις ρυθμίσεις του κανόνα εισερχομένων εμφανίζονται στο πεδίο **Παράμετροι** .

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Καθορισμός εάν ένας χρήστης δημιούργησε έναν κανόνα εισερχομένων](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
