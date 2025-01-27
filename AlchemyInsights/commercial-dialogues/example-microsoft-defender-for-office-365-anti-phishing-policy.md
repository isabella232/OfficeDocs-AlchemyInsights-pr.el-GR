---
title: Παράδειγμα πολιτικής προστασίας του Microsoft Defender για Office 365 ηλεκτρονικού "ψαρέματος"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035006"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Παράδειγμα πολιτικής προστασίας του Microsoft Defender για Office 365 ηλεκτρονικού "ψαρέματος"

Αυτές οι ρυθμίσεις ενεργοποιούν μια πολιτική που *ονομάζεται Τομέας και Διευθύνων Σύμβουλος.* Αυτή η πολιτική παρέχει προστασία χρήστη και τομέα από απομίμηση και, στη συνέχεια, εφαρμόζει την πολιτική σε όλα τα μηνύματα ηλεκτρονικού ταχυδρομείου που λαμβάνονται από τους χρήστες εντός του τομέα. Πρώτα, προσθέστε τις ακόλουθες πληροφορίες για να δημιουργήσετε την πολιτική:

- **Όνομα:** Περιγραφή τομέα και **διευθύνοντος σύμβουλου:** Εξασφαλίζει ότι ο Διευθύνων Σύμβουλος και ο τομέας σας δεν μιμηθείτε.
  **Εφαρμόζεται σε**: Επιλέξτε **τον τομέα παραλήπτη.** Στην **περιοχή "Οποιοδήποτε από αυτά",** **επιλέξτε "Επιλογή"** και, στη συνέχεια, επιλέξτε έναν τομέα. Επιλέξτε **+ Προσθήκη.** Επιλέξτε το πλαίσιο ελέγχου δίπλα στο όνομα του τομέα στη λίστα (για παράδειγμα, contoso.com ) και, *στη* συνέχεια, επιλέξτε **"Προσθήκη".** Επιλέξτε **"Τέλος".**
- Μετά τη δημιουργία της πολιτικής, μπορείτε να ρυθμίσετε με ακρίβεια την πολιτική, χρησιμοποιώντας τις ακόλουθες επιλογές:
  - **Προσθήκη χρηστών για προστασία:** Για αυτό το παράδειγμα, προσθέστε τουλάχιστον τη διεύθυνση ηλεκτρονικού ταχυδρομείου του διευθύνοντος σύμβουλου.
  - **Προσθέστε τομείς για προστασία:** Προσθέστε τον εταιρικό τομέα που περιλαμβάνει το γραφείο του Διευθύνοντος Σύμβουλου.
  - **Επιλέξτε ενέργειες:** Για την περίπτωση αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου από έναν απρόσωπο **χρήστη,** επιλέξτε "Ανακατεύθυνση μηνύματος σε άλλη διεύθυνση ηλεκτρονικού ταχυδρομείου" **και,** στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του διαχειριστή ασφαλείας (για παράδειγμα, *securityadmin@contoso.com).* Για **την περίπτωση αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου από έναν τομέα απομίμησης,** επιλέξτε **"Καραντίνα" του μηνύματος.**
  - **Ευφυΐα** γραμματοκιβωτίου: Από προεπιλογή, αυτή η επιλογή είναι ενεργοποιημένη όταν δημιουργείτε μια νέα πολιτική προστασίας από το ηλεκτρονικό "ψάρεμα". Αφήστε αυτήν τη ρύθμιση **σε αυτήν την** επιλογή για καλύτερα αποτελέσματα.
  - **Προσθήκη αξιόπιστων αποστολέων και τομέων:** Για αυτό το παράδειγμα, μην ορίσετε παρακάμψεις.
- Αφού εξετάσετε τις ρυθμίσεις σας, επιλέξτε "Δημιουργία αυτής **της πολιτικής" ή** **"Αποθήκευση",** ανάλογα με την περίπτωση.

Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα Πολιτικές προστασίας από το ηλεκτρονικό "ψάρεμα" Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
