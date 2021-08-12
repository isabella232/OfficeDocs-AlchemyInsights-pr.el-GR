---
title: Συσκευή σε κατάσταση εκκρεμότητας
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914003"
---
# <a name="device-in-pending-state"></a>Συσκευή σε κατάσταση εκκρεμότητας

**Προαπαιτούμενα:**

1. Εάν ρυθμίζετε καταχωρήσεις συσκευών για πρώτη φορά, βεβαιωθείτε ότι έχετε ελέγξει την Εισαγωγή στη διαχείριση συσκευών στο [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) που θα σας καθοδηγήσει σχετικά με τον τρόπο με τον οποίο μπορείτε να έχετε συσκευές υπό τον έλεγχο του Azure AD.
2. Εάν καταχωρείτε συσκευές απευθείας στο Azure AD και τις εγγράφετε στο Intune, θα πρέπει πρώτα [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) να βεβαιωθείτε ότι έχετε ρυθμίσει τις παραμέτρους του [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) και ότι έχετε ήδη ρυθμίσει τις άδειες χρήσης.
3. Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Azure AD και την εσωτερική εγκατάσταση AD. Μόνο ένας καθολικός διαχειριστής στο Microsoft Azure Active Directory μπορεί να διαχειρίζεται τις ρυθμίσεις για εγγραφές συσκευών. Επιπλέον, εάν ρυθμίζετε τις αυτόματες εγγραφές στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, θα πρέπει να είστε διαχειριστής της υπηρεσίας καταλόγου Active Directory και των υπηρεσιών AD FS (εάν υπάρχουν).

Η υβριδική διαδικασία εγγραφής συμμετοχής στο Azure AD απαιτεί οι συσκευές να είναι σε εταιρικό δίκτυο. Λειτουργεί επίσης μέσω VPN, αλλά υπάρχουν ορισμένες προειδοποιήσεις για αυτό. Έχουμε ακούσει ότι οι πελάτες χρειάζονται βοήθεια σχετικά με την αντιμετώπιση προβλημάτων της υβριδικής διαδικασίας εγγραφής συμμετοχής στο Azure AD υπό συνθήκες απομακρυσμένης εργασίας.

**Περιβάλλον ελέγχου ταυτότητας στο cloud (με χρήση του συγχρονισμού ή του ελέγχου ταυτότητας πρόσβασης μέσω του Azure AD)**

Αυτή η ροή καταχώρησης είναι επίσης γνωστή ως "Συμμετοχή συγχρονισμού".

Ακολουθεί μια ανάλυση του τι συμβαίνει κατά τη διαδικασία εγγραφής:

1. Windows 10 την εγγραφή σημείου σύνδεσης υπηρεσίας (SCP) όταν ο χρήστης συνδέεται στη συσκευή.

    1. Η συσκευή προσπαθεί πρώτα να ανακτήσει πληροφορίες μισθωτή από το SCP από την πλευρά του προγράμματος-πελάτη στο μητρώο [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Για περισσότερες πληροφορίες, ανατρέξτε στο [έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Εάν αποτύχει, η συσκευή επικοινωνεί με την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης για να λάβετε πληροφορίες μισθωτή από το SCP. Για να επαληθεύσετε το SCP, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Συνιστάται να ενεργοποιήσετε το SCP στην υπηρεσία καταλόγου Active Directory και να χρησιμοποιείτε μόνο SCP από την πλευρά του προγράμματος-πελάτη για την αρχική επικύρωση.

2. Windows 10 να επικοινωνήσει με το Azure AD στο περιβάλλον του συστήματος για τον έλεγχο ταυτότητας σε σχέση με το Azure AD.

    Μπορείτε να επαληθεύσετε εάν η συσκευή μπορεί να αποκτήσει πρόσβαση σε πόρους της Microsoft κάτω από το λογαριασμό συστήματος, χρησιμοποιώντας τη [δέσμη ενεργειών συνδεσιμότητας εγγραφής συσκευής δοκιμής.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 δημιουργεί αυτο-υπογεγραμμένο πιστοποιητικό και το αποθηκεύει κάτω από το αντικείμενο υπολογιστή στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης. Αυτό απαιτεί οπτική επαφή με τον ελεγκτή τομέα.

4. Το αντικείμενο συσκευής που έχει πιστοποιητικό συγχρονίζεται με το Azure AD μέσω του Azure AD Σύνδεση. Ο κύκλος συγχρονισμού είναι κάθε 30 λεπτά από προεπιλογή, αλλά εξαρτάται από τη ρύθμιση παραμέτρων του Azure AD Σύνδεση. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Σε αυτό το στάδιο, θα πρέπει να μπορείτε να δείτε τη συσκευή θέματος στην κατάσταση **"Σε εκκρεμότητα"** στην περιοχή "Συσκευή blade" της Πύλης Azure.

6. Στην επόμενη σύνδεση χρήστη στο Windows 10, η εγγραφή θα ολοκληρωθεί.

    > [!NOTE]
    > Εάν είστε σε VPN και η αποσύνδεση/σύνδεση τερματίσει τη σύνδεση τομέα, μπορείτε να ενεργοποιήσετε την εγγραφή με μη αυτόματο τρόπο. Για να το κάνετε αυτό:
    >
    > Εκδόξτε `dsregcmd /join` ένα τοπικά μήνυμα διαχειριστή ή από απόσταση μέσω PSExec στον υπολογιστή σας.
    >
    > Για παράδειγμα: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Για συνήθη προβλήματα με την εγγραφή Azure Active Directory συσκευής, ανατρέξτε στις Συνήθεις [ερωτήσεις για τις συσκευές.](https://docs.microsoft.com/azure/active-directory/devices/faq)
