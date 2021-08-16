---
title: Έχω αποκλειστεί από την Πρόσβαση υπό όρους με συμβατή συσκευή
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019148"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Έχω αποκλειστεί από την Πρόσβαση υπό όρους με συμβατή συσκευή

**Εργαλεία που συνιστώνται ιδιαίτερα**

- [Εργαλείο αντιμετώπισης προβλημάτων εγγραφής συσκευής](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - Ένα ολοκληρωμένο εργαλείο που σας βοηθά να αντιμετωπίσετε τα πιο συνηθισμένα προβλήματα εγγραφής συσκευών.
- [Δοκιμή δέσμης ενεργειών συνδεσιμότητας εγγραφής συσκευής](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - Ένα εργαλείο που χρησιμοποιείται για να διασφαλιστεί ότι μια συσκευή μπορεί να αποκτήσει πρόσβαση στα τελικά σημεία καταχώρησης συσκευής κάτω από το λογαριασμό συστήματος.
- [Δέσμη ενεργειών εκκαθάρισης συσκευής Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - Ένα εργαλείο που χρησιμοποιείται για την αναζήτηση και τη διαχείριση μη γραφειών συσκευών στο περιβάλλον σας.

Ακολουθούν ορισμένοι συνηθισμένοι λόγοι για τους οποίους η πρόσβαση υπό όρους  ενδέχεται να αποτυγχάνει για μια συμβατή συσκευή ή γιατί οι χρήστες σας ενδέχεται να λαμβάνουν το μήνυμα "Δεν μπορείτε να λάβετε εκεί από εδώ κατά τη διάρκεια μιας αίτησης για είσοδο σε έναν εταιρικό πόρο".

1. **Η συσκευή δεν βρίσκεται σε απαιτούμενη κατάσταση συσκευής με MDM:**

Επαληθεύστε ότι η συσκευή έχει εγγραφεί σε μια εγκεκριμένη υπηρεσία παροχής MDM, όπως το Intune και έχει *επισημανθεί ως συμβατή.* Για περισσότερες πληροφορίες σχετικά με το Intune, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Για καλύτερη κατανόηση της συμμόρφωσης των συσκευών και του Intune, ανατρέξτε στην πολιτική συμμόρφωσης για να ορίσετε κανόνες [για συσκευές που διαχειρίζεστε με το Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Εάν αντιμετωπίζετε προβλήματα κατά την εγγραφή μιας συσκευής με το Intune, βρείτε λεπτομέρειες αντιμετώπισης προβλημάτων στο θέμα [Αντιμετώπιση προβλημάτων εγγραφής συσκευής στη Microsoft.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Για περαιτέρω υποστήριξη intune, δημιουργήστε μια αίτηση υποστήριξης. Για να το κάνετε αυτό, επισκεφθείτε τη [σελίδα Βοήθειας και υποστήριξης του Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Η συσκευή δεν είναι συνδεδεμένος στο δίκτυο οργανισμών:**

Για να αποκτήσετε πρόσβαση σε εταιρικούς πόρους, η συσκευή πρέπει να είναι συνδεδεμένη στο δίκτυο του οργανισμού, είτε μέσω άμεσης σύνδεσης είτε μέσω εικονικού ιδιωτικού δικτύου (VPN) και να συνδέεται επίσης με εσωτερική εγκατάσταση ή Azure Active Directory. Για να συμμετάσχετε σε μια συσκευή εργασίας στο δίκτυο του οργανισμού, ανατρέξτε στο θέμα Συμμετοχή [της συσκευής εργασίας σας στο δίκτυο της εταιρείας σας.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Για να καταχωρήσετε μια προσωπική συσκευή/BYOD, ανατρέξτε στο θέμα Δήλωση της [προσωπικής συσκευής σας στο δίκτυο του οργανισμού σας.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Για να επαληθεύσετε εάν η συσκευή έχει γίνει μέλος του δικτύου, μπορείτε να ακολουθήσετε τα βήματα για τις καταχωρημένες συσκευές [εδώ ή για](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) τις συσκευές εργασίας [εδώ.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Για να εμβείνετε το πρόβλημα στη συνδεσιμότητα δικτύου οργανισμού, ακολουθήστε τις παρακάτω οδηγίες:

    1. Πραγματοποιήστε είσοδο για Windows χρησιμοποιώντας τον σχολικό ή τον σχολικό λογαριασμό σας, για παράδειγμα, alain@contoso.com.
    2. Σύνδεση στο δίκτυο της εταιρείας σας μέσω VPN ή DirectAccess.
    3. Αφού συνδεθείτε, πατήστε το πλήκτρο Windows **λογότυπο+L για να κλειδώσετε** τη συσκευή σας.
    4. Ξεκλειδώστε τη συσκευή σας χρησιμοποιώντας τον λογαριασμό της εργασίας ή του σχολείου σας και, στη συνέχεια, προσπαθήστε να αποκτήσετε ξανά πρόσβαση στην προβληματική εφαρμογή ή υπηρεσία.

Εάν εμφανιστεί ξανά το **μήνυμα σφάλματος "Δεν** μπορείτε να λάβετε ξανά αυτό το μήνυμα σφάλματος από εδώ", το πρόβλημα είναι πιθανό να υπάρχει κάπου αλλού.

3. **Το λειτουργικό σύστημα δεν υποστηρίζεται:**

Βεβαιωθείτε ότι χρησιμοποιείτε μια υποστηριζόμενη έκδοση του λειτουργικού συστήματος, συμπεριλαμβανομένων των εξής:

- **Windows προγράμματος-πελάτη:** Windows 7 ή νεότερη έκδοση

- **Windows Server:** Windows Server 2008 R2 ή νεότερη έκδοση

- **macOS**: macOS X ή νεότερη έκδοση

- **Android και iOS:** Τελευταία έκδοση λειτουργικών συστημάτων Android και iOS για κινητές συσκευές

4. **Το πρόγραμμα περιήγησης Web δεν υποστηρίζεται:**

Βρείτε τα υποστηριζόμενα προγράμματα περιήγησης παρακάτω. Για την υποστήριξη του Chrome Windows έκδοση 1703 ή νεότερη έκδοση, απαιτείται Windows 10 επέκτασης λογαριασμών. Για τον Edge 85+, ο χρήστης πρέπει να συνδεθεί για να περάσει σωστά τις πληροφορίες συμμόρφωσης της συσκευής. Για περισσότερες λεπτομέρειες, ανατρέξτε [εδώ.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android:** **Microsoft Edge:** Intune Managed Browser, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Βρείτε περισσότερες πληροφορίες σχετικά με **το μήνυμα "Δεν μπορείτε να λάβετε εκεί" και** τα βήματα αντιμετώπισης προβλημάτων [εδώ.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
