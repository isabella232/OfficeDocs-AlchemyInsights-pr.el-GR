---
title: 451 4.7.0 Προσωρινό σφάλμα διακομιστή. Δοκιμάστε ξανά αργότερα. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812579"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Προσωρινό σφάλμα διακομιστή. Δοκιμάστε ξανά αργότερα. PRX4

Ενδέχεται να αντιμετωπίσετε ένα πρόβλημα κατά την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου μέσω του Smarthost "smtp.office365.com" χρησιμοποιώντας τη μέθοδο υποβολής προγράμματος-πελάτη SMTP και να λάβετε το σφάλμα: "451 4.7.0 Προσωρινό σφάλμα διακομιστή. Δοκιμάστε ξανά αργότερα. Το PRX4 είναι κυρίως προσωρινό". 

Βεβαιωθείτε ότι δεν χρησιμοποιείτε ένα κοινόχρηστο γραμματοκιβώτιο για την υποβολή προγράμματος-πελάτη SMTP, καθώς η μέθοδος υποβολής προγράμματος-πελάτη SMTP απαιτεί γραμματοκιβώτιο με άδεια χρήσης για την αποστολή αλληλογραφίας. Ωστόσο, εάν δεν χρησιμοποιείτε κοινόχρηστο γραμματοκιβώτιο και το πρόβλημα παραμένει, ελέγξτε τα εξής:

1. Ενεργοποίηση υποβολής SMTP προγράμματος-πελάτη στο γραμματοκιβώτιο με άδεια χρήσης που χρησιμοποιείται με την εκτέλεση αυτής της εντολής PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OR

    1. Μεταβείτε στην Κέντρο διαχείρισης Microsoft 365 > **ενεργοί χρήστες** και επιλέξτε το χρήστη.
    1. Μεταβείτε στην καρτέλα "Αλληλογραφία" > **εφαρμογές ηλεκτρονικού** ταχυδρομείου > επιλέξτε **"Διαχείριση εφαρμογών ηλεκτρονικού ταχυδρομείου".** 
    1. Βεβαιωθείτε ότι η **ρύθμιση SMTP με έλεγχο ταυτότητας** είναι ενεργοποιημένη.
    1. Επιλέξτε **"Αποθήκευση αλλαγών".**
    
    Για να ενεργοποιήσετε τον έλεγχο ταυτότητας SMTP για έναν ολόκληρο οργανισμό, εκτελέστε αυτή την εντολή:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Σημείωση:** Για λόγους ασφαλείας, συνιστάται να ενεργοποιήσετε τον έλεγχο ταυτότητας SMTP μόνο για το γραμματοκιβώτιο που χρησιμοποιείται. Η ρύθμιση επιπέδου χρήστη παρακάμπτει τη ρύθμιση επιπέδου οργανισμού.

2. Απενεργοποιήστε τις προεπιλογές ασφαλείας Azure, ενεργοποιώντας **την επιλογή "Ενεργοποίηση προεπιλογών ασφαλείας"** σε **"Όχι":**

    1. Πραγματοποιήστε είσοδο στην πύλη Azure ως διαχειριστής ασφαλείας, διαχειριστής πρόσβασης υπό όρους ή καθολικός διαχειριστής.
    1. Μεταβείτε στην επιλογή Azure Active Directory >**  "Ιδιότητες"** και επιλέξτε **"Διαχείριση προεπιλογών ασφαλείας".**
    1. Ορίστε το **κουμπί εναλλαγής "Ενεργοποίηση προεπιλογών ασφαλείας"** σε **"Όχι".**
    1. Επιλέξτε **"Αποθήκευση".**

3. Απενεργοποιήστε τον έλεγχο ταυτότητας πολλών παραγόντων (MFA) στο γραμματοκιβώτιο με άδεια χρήσης που χρησιμοποιείται.

    1. Μεταβείτε στην Κέντρο διαχείρισης Microsoft 365 και, στο αριστερό μενού περιήγησης, επιλέξτε **"Χρήστες**  >  **ενεργοί χρήστες".**
    1. Στη σελίδα **"Ενεργοί χρήστες",** επιλέξτε **"Έλεγχος ταυτότητας πολλών παραγόντων".**
    1. Επιλέξτε το χρήστη και απενεργοποιήστε τον **έλεγχο ταυτότητας πολλών παραγόντων.**

