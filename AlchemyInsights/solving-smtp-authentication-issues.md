---
title: Ενεργοποίηση ελέγχου ταυτότητας ΚΑΙ αντιμετώπισης προβλημάτων SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890434"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Ενεργοποίηση ελέγχου ταυτότητας ΚΑΙ αντιμετώπισης προβλημάτων SMTP

Εάν θέλετε να ενεργοποιήσετε τον έλεγχο ταυτότητας SMTP για ένα γραμματοκιβώτιο ή εάν εμφανίζεται ένα σφάλμα "Ο υπολογιστής-πελάτης δεν έχει ελεγχθεί", "Ανεπιτυχής έλεγχος ταυτότητας" ή σφάλμα "SmtpClientAuthentication" με κωδικό 5.7.57 ή 5.7.3 ή 5.7.139 κατά την προσπάθεια αναμετάδοσης ηλεκτρονικού ταχυδρομείου με έλεγχο ταυτότητας μιας συσκευής ή εφαρμογής με το Microsoft 365, εκτελέστε αυτές τις τρεις ενέργειες για να επιλύσετε το πρόβλημα:

1. Απενεργοποιήστε [τις προεπιλογές ασφαλείας του Azure,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ενεργοποιώντας **την επιλογή "Ενεργοποίηση προεπιλογών ασφαλείας"** σε **"Όχι".**

    a. Πραγματοποιήστε είσοδο στην πύλη Azure ως διαχειριστής ασφαλείας, διαχειριστής πρόσβασης υπό όρους ή καθολικός διαχειριστής.<BR/>
    b. Μεταβείτε στην επιλογή Azure Active Directory > **Ιδιότητες.**<BR/>
    c. Επιλέξτε **"Διαχείριση προεπιλογών ασφαλείας".**<BR/>
    d. Ορισμός **προεπιλογών ενεργοποίησης ασφαλείας** σε **"Όχι".**<BR/>
    e. Επιλέξτε **"Αποθήκευση".**

2. [Ενεργοποίηση υποβολής SMTP προγράμματος-πελάτη](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) στο γραμματοκιβώτιο με άδεια χρήσης.

    a. Από το Κέντρο διαχείρισης Microsoft 365, μεταβείτε στην επιλογή **"Ενεργοί χρήστες"** και επιλέξτε το χρήστη.<BR/>
    b. Μεταβείτε στην καρτέλα "Αλληλογραφία" και, στην περιοχή **"Εφαρμογές ηλεκτρονικού ταχυδρομείου",** επιλέξτε **"Διαχείριση εφαρμογών ηλεκτρονικού ταχυδρομείου".**<BR/>
    d. Βεβαιωθείτε ότι είναι **επιλεγμένο το SMTP** με έλεγχο ταυτότητας (ενεργοποιημένο).<BR/>
    e. Επιλέξτε **"Αποθήκευση αλλαγών".**<BR/>

3. [Απενεργοποιήστε τον έλεγχο ταυτότητας πολλών παραγόντων (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) στο γραμματοκιβώτιο με άδεια χρήσης.

    a. Μεταβείτε στην Κέντρο διαχείρισης Microsoft 365 και, στο αριστερό μενού περιήγησης, επιλέξτε **"Χρήστες**  >  **ενεργοί χρήστες".**<BR/>
    b. Επιλέξτε έλεγχο **ταυτότητας πολλών παραγόντων.**<BR/>
    c. Επιλέξτε το χρήστη και απενεργοποιήστε **την ταυτότητα πολλών παραγόντων.**<BR/>
