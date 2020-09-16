---
title: Μετεγκατάσταση από AIP σε ΠΕΠ/ενοποιημένη επισήμανση στο κέντρο συμμόρφωσης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674326"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Μετεγκατάσταση από AIP σε ΠΕΠ/ενοποιημένη επισήμανση στο κέντρο συμμόρφωσης

Για να κάνετε μετεγκατάσταση από ετικέτες AIP σε ενοποιημένη σήμανση στο κέντρο ασφάλειας και συμμόρφωσης, κάντε τα εξής:

**Ενεργοποίηση προστασίας από την πύλη Azure**

1. Εάν δεν το έχετε κάνει ήδη, ανοίξτε ένα νέο παράθυρο του προγράμματος περιήγησης και [Πραγματοποιήστε είσοδο στην πύλη Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Μεταβείτε στη λεπίδα **προστασίας πληροφοριών Azure** . Για παράδειγμα, στο μενού Hub, κάντε κλικ στην επιλογή **όλες οι υπηρεσίες** και αρχίστε να πληκτρολογείτε **πληροφορίες** στο πλαίσιο φίλτρο. Επιλέξτε **προστασία πληροφοριών Azure**. Εάν δεν έχετε αποκτήσει πρόσβαση στο δίσκο προστασίας πληροφοριών Azure πριν, ανατρέξτε στα [πρόσθετα βήματα](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) εφάπαξ για να προσθέσετε αυτήν τη λεπίδα στην πύλη. Για να ανοίξετε το Blade προστασία πληροφοριών Azure, πρέπει να έχετε ένα [πρόγραμμα προστασίας πληροφοριών Azure Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ή ένα πρόγραμμα του Office 365 που περιλαμβάνει τη διαχείριση δικαιωμάτων. Εάν έχετε μία από αυτές τις συνδρομές, αλλά δείτε ένα μήνυμα ότι δεν είναι δυνατή η εύρεση μιας έγκυρης συνδρομής, [επικοινωνήστε με την υποστήριξη της Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ή χρησιμοποιήστε τα τυπικά κανάλια υποστήριξής σας.

2. Εντοπίστε τις επιλογές **διαχείρισης** μενού και επιλέξτε **Ενεργοποίηση προστασίας**. Κάντε κλικ στην επιλογή **Ενεργοποίηση**και, στη συνέχεια, επιβεβαιώστε την ενέργειά σας. Όταν ολοκληρωθεί η ενεργοποίηση, η γραμμή πληροφοριών εμφανίζει την **Ενεργοποίηση ολοκληρώθηκε με επιτυχία**.

**Μετεγκατάσταση ετικετών προστασίας πληροφοριών του Azure στο κέντρο συμμόρφωσης & ασφαλείας του Office 365**

1. Βεβαιωθείτε ότι έχετε συνδεθεί ως χρήστης με δικαιώματα καθολικού διαχειριστή.

2. Μεταβείτε στη λεπίδα **προστασίας πληροφοριών Azure** .

3. Από την επιλογή " **Διαχείριση** μενού", επιλέξτε " **ενοποιημένη επισήμανση**".

4. Στη λάμα **προστασίας πληροφοριών Azure-ενοποιημένη ετικέτα** , κάντε κλικ στην επιλογή **Ενεργοποίηση** και ακολουθήστε τις οδηγίες στο Internet.

**Σημείωση**: Βεβαιωθείτε ότι έχετε τα κατάλληλα δικαιώματα για να ενεργοποιήσετε τη μετεγκατάσταση του κέντρου συμμόρφωσης & ασφαλείας. Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω άρθρα:

1. [Πρέπει να είστε καθολικός διαχειριστής για να ρυθμίσετε τις παραμέτρους της προστασίας πληροφοριών του Azure ή μπορώ να αναθέτω σε άλλους διαχειριστές;](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Σημαντικές πληροφορίες σχετικά με τους ρόλους διαχείρισης μετά τη μετεγκατάσταση στο κέντρο συμμόρφωσης & ασφαλείας.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Για περισσότερες πληροφορίες σχετικά με το AIP για την ενοποιημένη επισήμανση της μετεγκατάστασης στο κέντρο ασφάλειας και συμμόρφωσης, ανατρέξτε στο θέμα [μετεγκατάσταση ετικετών](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
