---
title: Αλλαγή καναλιών ενημέρωσης για εφαρμογές του Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439386"
---
# <a name="change-update-channels-for-office-apps"></a>Αλλαγή καναλιών ενημέρωσης για εφαρμογές του Office

Για νέες εγκαταστάσεις του Office, χρησιμοποιήστε τις Ρυθμίσεις λήψης λογισμικού του Office για να επιλέξετε το επιθυμητό κανάλι ενημέρωσης και, στη συνέχεια, εγκαταστήστε (ή εγκαταστήστε ξανά) τις εφαρμογές του Office. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση ρυθμίσεων λήψης λογισμικού στο Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Σημείωση** Το κανάλι ενημέρωσης που έχει επιλεγεί χρησιμοποιώντας τις Ρυθμίσεις λήψης λογισμικού του Office ισχύει για όλους τους χρήστες που εκτελούν νέες εγκαταστάσεις χρησιμοποιώντας την πύλη O365. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Λήψη και εγκατάσταση ή επανεγκατάσταση του Microsoft 365 ή του Office 2019 σε PC ή Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Για υπάρχουσες εγκαταστάσεις του Office, χρησιμοποιήστε το Εργαλείο ανάπτυξης του Office (ODT) για να μεταβείτε σε διαφορετικό κανάλι ενημέρωσης:  

1. Κάντε λήψη της πιο πρόσφατης έκδοσης του Εργαλείου ανάπτυξης του Office (setup.exe) από το [Κέντρο λήψης](https://go.microsoft.com/fwlink/p/?LinkID=626065)της Microsoft .
2. Προσδιορίστε το όνομα του καναλιού στο οποίο θέλετε να μεταβείτε. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Επιλογές ρύθμισης παραμέτρων για το εργαλείο ανάπτυξης του Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Δημιουργήστε ένα αρχείο XML ρύθμισης παραμέτρων που καθορίζει το κατάλληλο όνομα καναλιού, για παράδειγμα, update.xml.  
    a. <Configuration>  
    b. <ενημερώνει **το κανάλι="Μηνιαία"** />  
    c. </Configuration>
4. Από μια γραμμή εντολών με αυξημένα δικαιώματα, μεταβείτε στη θέση φακέλου όπου βρίσκεται setup.exe και εκτελέστε την ακόλουθη εντολή:  
    a. setup.exe /configure update.xml
5. Ξεκινήστε μια εφαρμογή του Office (όπως το Excel) και, στη συνέχεια, επιλέξτε **Λογαριασμός αρχείου**  >  **Account**. Στην ενότητα Πληροφορίες προϊόντος, επιλέξτε **Άμεση ενημέρωση των επιλογών**  >  **ενημέρωσης**.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τρόπος εναλλαγής καναλιών ενημέρωσης για υπάρχουσες εφαρμογές του Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Για εναλλαγή καναλιών ενημέρωσης για μια επιλεγμένη ομάδα χρηστών ή χρησιμοποιώντας τη Διαχείριση ρύθμισης παραμέτρων (SCCM), ρυθμίστε τις παραμέτρους της ρύθμισης "Ενημέρωση καναλιού" χρησιμοποιώντας αντικείμενο πολιτικής ομάδας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Επισκόπηση των καναλιών ενημέρωσης για τις εφαρμογές Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Για λεπτομέρειες, ανατρέξτε στο θέμα [Τρόπος διαχείρισης των καναλιών Office 365 ProPlus για επαγγελματίες πληροφορικής](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) και [διαχείριση ενημερώσεων σε εφαρμογές microsoft 365 με τη Διαχείριση ρύθμισης παραμέτρων τελικού σημείου της Microsoft](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).