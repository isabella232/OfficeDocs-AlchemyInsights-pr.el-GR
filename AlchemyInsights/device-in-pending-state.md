---
title: Συσκευή σε κατάσταση εκκρεμούς
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678479"
---
# <a name="device-in-pending-state"></a>Συσκευή σε κατάσταση εκκρεμούς

**Τις προϋποθέσεις**

1. Εάν ρυθμίζετε εγγραφές συσκευών για πρώτη φορά, βεβαιωθείτε ότι έχετε αναθεωρηθεί [Εισαγωγή στη διαχείριση συσκευών στο Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) που θα σας καθοδηγήσει στον τρόπο με τον οποίο μπορείτε να λάβετε συσκευές υπό τον έλεγχο του Azure AD.
2. Εάν καταχωρείτε συσκευές στο Azure AD απευθείας και τις εγγράφετε σε Intune, θα πρέπει να εξασφαλίσετε ότι έχετε ρυθμίσει τις [παραμέτρους του Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) και ότι θα έχετε την [άδεια χρήσης](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) στη θέση της πρώτα.
3. Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Azure AD και τη διαφήμιση εσωτερικής εγκατάστασης. Μόνο ένας καθολικός διαχειριστής στο Azure AD μπορεί να διαχειριστεί ρυθμίσεις για τις καταχωρήσεις συσκευών. Επιπλέον, εάν ρυθμίζετε αυτόματες εγγραφές στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, θα πρέπει να είστε διαχειριστής της υπηρεσίας καταλόγου Active Directory και του AD FS (εάν υπάρχει).

Η διαδικασία δήλωσης σύνδεσης του υβριδικού Azure AD απαιτεί συσκευές για να είναι σε εταιρικό δίκτυο. Λειτουργεί επίσης μέσω VPN, αλλά υπάρχουν ορισμένες προειδοποιήσεις για αυτό. Ακούσαμε ότι οι πελάτες χρειάζονται βοήθεια για την αντιμετώπιση της διαδικασίας δήλωσης συμμετοχής στο υβριδικό Azure AD, στην περιοχή απομακρυσμένες συνθήκες εργασίας.

**Περιβάλλον ελέγχου ταυτότητας cloud (χρησιμοποιώντας τον συγχρονισμό κατακερματισμού κωδικού πρόσβασης AD Azure ή τον έλεγχο ταυτότητας διαβίβασης)**

Αυτή η ροή δήλωσης είναι επίσης γνωστή ως "Συγχρονισμός συνδέσμου".

Ακολουθεί μια ανάλυση για το τι συμβαίνει κατά τη διαδικασία εγγραφής:

1. Τα Windows 10 ανακαλύπτουν την εγγραφή του σημείο σύνδεσης υπηρεσίας (SCP) όταν ο χρήστης συνδέεται στη συσκευή.

    1. Η συσκευή επιχειρεί πρώτα να ανακτήσει πληροφορίες μισθωτών από το SCP του προγράμματος-πελάτη στο μητρώο [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [έγγραφο](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Εάν αποτύχει, η συσκευή επικοινωνεί με την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης για να λάβετε πληροφορίες μισθωτών από την SCP. Για να επαληθεύσετε το SCP, ανατρέξτε σε αυτό το [έγγραφο](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Συνιστούμε να ενεργοποιήσετε την SCP στην υπηρεσία καταλόγου Active Directory και να χρησιμοποιείτε μόνο το SCP προγράμματος-πελάτη για την αρχική επικύρωση.

2. Τα Windows 10 προσπαθούν να επικοινωνούν με το Azure AD κάτω από το περιβάλλον συστήματος για τον έλεγχο ταυτότητας από το Azure AD.

    Μπορείτε να επαληθεύσετε εάν η συσκευή μπορεί να αποκτήσει πρόσβαση σε πόρους της Microsoft κάτω από το λογαριασμό συστήματος, χρησιμοποιώντας τη [δέσμη ενεργειών συνδεσιμότητας δήλωσης δοκιμής συσκευής](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Τα Windows 10 παράγουν αυτο-υπογεγραμμένο πιστοποιητικό και το αποθηκεύουν κάτω από το αντικείμενο υπολογιστή στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης. Αυτό απαιτεί οπτική επαφή με τον ελεγκτή τομέα.

4. Αντικείμενο συσκευής που έχει το πιστοποιητικό συγχρονίζεται με το Azure AD μέσω σύνδεσης Azure AD. Ο κύκλος συγχρονισμού είναι κάθε 30 λεπτά από προεπιλογή, αλλά εξαρτάται από τη ρύθμιση παραμέτρων του Azure AD Connect. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό το [έγγραφο](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Σε αυτό το στάδιο, θα πρέπει να μπορείτε να δείτε τη συσκευή θέματος σε κατάσταση "σε **εκκρεμότητα**" στην περιοχή "λεπίδα συσκευής" του Azure Portal.

6. Στην επόμενη σύνδεση χρήστη στα Windows 10, η καταχώρηση θα ολοκληρωθεί.

    > [!NOTE]
    > Εάν βρίσκεστε σε VPN και η αποσύνδεση/σύνδεση τερματίζει τη συνδεσιμότητα τομέα, μπορείτε να ενεργοποιήσετε την καταχώρηση με μη αυτόματο τρόπο. Για να το κάνετε αυτό:
    >
    > Εκδώσετε ένα `dsregcmd /join` τοπικό μήνυμα στο διαχειριστή ή απομακρυσμένα μέσω του PSExec στον υπολογιστή σας.
    >
    > Για παράδειγμα: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Για συνηθισμένα προβλήματα με την καταχώρηση συσκευής του Azure Active Directory, ανατρέξτε στο θέμα [Συνήθεις ερωτήσεις](https://docs.microsoft.com/azure/active-directory/devices/faq)για τις συσκευές.
