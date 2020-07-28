---
title: Έλεγχος αυτόματων ενημερώσεων για εφαρμογές του Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439330"
---
# <a name="control-automatic-updates-for-office-apps"></a>Έλεγχος αυτόματων ενημερώσεων για εφαρμογές του Office

Από προεπιλογή, οι ενημερώσεις για το Office Apps λαμβάνονται αυτόματα και εφαρμόζονται στο παρασκήνιο χωρίς καμία παρέμβαση του χρήστη. Ωστόσο, οι διαχειριστές μπορούν να ελέγχουν τον τρόπο εφαρμογής των ενημερώσεων χρησιμοποιώντας τις ρυθμίσεις του Office Update. Οι ρυθμίσεις ενημέρωσης επιτρέπουν στους διαχειριστές να ενεργοποιούν ή να απενεργοποιούν τις αυτόματες ενημερώσεις, να εμφανίζουν ή να αποκρύπτουν το κουμπί **Άμεση ενημέρωση** στο Office, να ορίσουν προθεσμίες ενημέρωσης και πολλά άλλα. Για λεπτομερείς πληροφορίες, ανατρέξτε στα θέματα:

- [Ρύθμιση παραμέτρων ενημέρωσης για το Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Η αυτόματη ενημέρωση για το Office δεν είναι ενεργοποιημένη](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Ορισμός του τρόπου ενημέρωσης του Office μετά την εγκατάστασή του](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Για να εξετάσετε τις υπάρχουσες ρυθμίσεις ενημερωμένων εκδόσεων που εφαρμόζονται σε έναν υπολογιστή-πελάτη, ακολουθήστε τα εξής βήματα:

1. Ανοίξτε τον Επεξεργαστή Μητρώου (Registry Editor) **μεταβαίνοντας στην επιλογή Έναρξη**  >  **Run**  >  **εκτέλεσης του regedit**.
2. Μεταβείτε στην ακόλουθη θέση και εξετάστε τις ρυθμίσεις του Office Update:  
    a. HKEY_LOCAL_MACHINE\ΛΟΓΙΣΜΙΚΟ\Microsoft\Office\  
    b. Κάντε κλικ στο κουμπί Για να κάνετε\ρύθμιση παραμέτρων

**Σημείωση**  Εάν έχει οριστεί το κλειδί OfficeMgmtCOM, ενδέχεται να εμφανιστεί το μήνυμα "Η διαχείριση των ενημερωμένων εκδόσεων γίνεται από το διαχειριστή του συστήματός σας" **στις**  >  **Account**  >  **Ενημερωμένες εκδόσεις του Office**Account Office . Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση ενημερώσεων σε εφαρμογές του Microsoft 365 με τη Διαχείριση ρύθμισης παραμέτρων τελικού σημείου της Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  