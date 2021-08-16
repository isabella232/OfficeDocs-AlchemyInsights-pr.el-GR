---
title: Μετεγκατάσταση από AIP σε MIP/Ενοποιημένη σήμανση στο Κέντρο συμμόρφωσης
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000356"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Μετεγκατάσταση από AIP σε MIP/Ενοποιημένη σήμανση στο Κέντρο συμμόρφωσης

Για να μετεγκαταστήσετε από ετικέτες AIP σε ενοποιημένες ετικέτες στο κέντρο ασφάλειας και συμμόρφωσης, κάντε τα εξής:

**Ενεργοποίηση προστασίας από την πύλη Azure**

1. Εάν δεν το έχετε κάνει ήδη, ανοίξτε ένα νέο παράθυρο του προγράμματος περιήγησης [και πραγματοποιήστε είσοδο στην πύλη Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Μεταβείτε στη **λάμα προστασίας πληροφοριών** Azure. Για παράδειγμα, στο μενού διανομέα, κάντε κλικ στην επιλογή "Όλες **οι υπηρεσίες" και** αρχίστε να **πληκτρολογείτε "Πληροφορίες"** στο πλαίσιο "Φίλτρο". Επιλέξτε **"Προστασία πληροφοριών Azure".** Εάν δεν έχετε αποκτήσει ξανά πρόσβαση στη λάμα προστασίας [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) πληροφοριών Azure, ανατρέξτε στα πρόσθετα βήματα που απαιτούνται για την προσθήκη αυτής της λάμας στην πύλη. Για να ανοίξετε τη λάμα προστασίας πληροφοριών Azure, πρέπει να έχετε ένα σχέδιο προστασίας [πληροφοριών Azure Premium ή](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ένα Office 365 που περιλαμβάνει τη Διαχείριση δικαιωμάτων. Εάν έχετε μία από αυτές τις συνδρομές, αλλά βλέπετε ένα μήνυμα ότι δεν είναι δυνατή η βρείτε μια έγκυρη συνδρομή, επικοινωνήστε με την Υποστήριξη [της Microsoft ή](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) χρησιμοποιήστε τα τυπικά κανάλια υποστήριξης.

2. Εντοπίστε **τις επιλογές** μενού "Διαχείριση" και επιλέξτε **"Ενεργοποίηση προστασίας".** Κάντε κλικ **στην επιλογή "Ενεργοποίηση"** και, στη συνέχεια, επιβεβαιώστε την ενέργεια. Όταν ολοκληρωθεί η ενεργοποίηση, η γραμμή πληροφοριών εμφανίζει ότι η ενεργοποίηση **ολοκληρώθηκε με επιτυχία.**

**Μετεγκατάσταση ετικετών προστασίας πληροφοριών Azure στο κέντρο Office 365 ασφάλειας & συμμόρφωσης**

1. Βεβαιωθείτε ότι έχετε συνδεθεί ως χρήστης με δικαιώματα καθολικού διαχειριστή.

2. Μεταβείτε στη **λάμα προστασίας πληροφοριών** Azure.

3. Από την **επιλογή μενού** "Διαχείριση", επιλέξτε **"Ενοποιημένη σήμανση".**

4. Στην Προστασία **πληροφοριών Azure - Ενοποιημένος δίσκος ετικετών,** κάντε κλικ στην επιλογή **"Ενεργοποίηση"** και ακολουθήστε τις οδηγίες στο Internet.

**Σημείωση:** Βεβαιωθείτε ότι έχετε τα κατάλληλα δικαιώματα πριν από την ενεργοποίηση της μετεγκατάστασης του Κέντρου & ασφάλειας. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτά τα άρθρα:

1. [Πρέπει να είστε καθολικός διαχειριστής για να ρυθμίσετε τις παραμέτρους της Προστασίας πληροφοριών Azure ή μπορώ να αναθέσω σε άλλους διαχειριστές;](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Σημαντικές πληροφορίες σχετικά με τους ρόλους διαχείρισης μετά τη μετεγκατάσταση στο Κέντρο & ασφάλειας.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Για περισσότερες πληροφορίες σχετικά με τη μετεγκατάσταση AIP σε ενοποιημένη σήμανση στο Κέντρο ασφάλειας και συμμόρφωσης, ανατρέξτε στο θέμα [Μετεγκατάσταση ετικετών.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
