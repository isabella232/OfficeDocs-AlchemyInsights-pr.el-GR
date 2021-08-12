---
title: 646 Τρόπος ρύθμισης παραμέτρων του AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963643"
---
# <a name="configure-sync-features"></a>Ρύθμιση παραμέτρων δυνατοτήτων συγχρονισμού

Το Azure AD Σύνδεση περιλαμβάνει διάφορες δυνατότητες που είναι ενεργοποιημένες από προεπιλογή ή που μπορείτε να ενεργοποιήσετε αργότερα. Ορισμένες δυνατότητες απαιτούν πρόσθετες ρυθμίσεις παραμέτρων σε συγκεκριμένα περιβάλλοντα.

- [Τα όρια φιλτραρίσματος](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) των αντικειμένων συγχρονίζονται με το Azure AD. Από προεπιλογή, όλοι οι χρήστες, οι επαφές, οι ομάδες και Windows 10 λογαριασμών υπολογιστών συγχρονίζονται. Μπορείτε να συμπεριλάβετε ή να εξαιρέσετε αντικείμενα που βασίζονται σε τομείς, OUs ή άλλα χαρακτηριστικά.

- [Ο συγχρονισμός του hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) κωδικού πρόσβασης συγχρονίζει τον κωδικό πρόσβασης από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης στο Azure AD. Αυτό επιτρέπει τη διαχείριση κωδικών πρόσβασης σε μία θέση, αλλά η χρήση του ίδιου κωδικού πρόσβασης τόσο σε περιβάλλοντα εσωτερικής εγκατάστασης όσο και σε περιβάλλοντα cloud. Επειδή η υπηρεσία καταλόγου Active Directory είναι η έγκυρη προέλευση, μπορείτε να χρησιμοποιήσετε τις δικές σας πολιτικές κωδικού πρόσβασης.

- [Η επαναφορά κωδικού πρόσβασης από το χρήστη (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) επιτρέπει στους χρήστες να επαναφέρουν τους δικούς τους κωδικούς πρόσβασης στο cloud ενώ εξακολουθούν να εφαρμόζουν την πολιτική κωδικών πρόσβασης εσωτερικής εγκατάστασης.

- [Η διαγραφή συσκευής](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) επιτρέπει την εγγραφή των καταχωρημένων συσκευών στο Azure AD στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, ώστε να μπορούν να χρησιμοποιηθούν για πρόσβαση υπό όρους.

- [Η αποτροπή τυχαίων διαγραφών](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) είναι ενεργοποιημένη από προεπιλογή για την αποτροπή πάρα πολλών ταυτόχρονων διαγραφών αντικειμένων (περισσότερα από 500 αντικείμενα ανά συγχρονισμό). Μπορείτε να αλλάξετε αυτήν τη ρύθμιση ώστε να ανταποκρίνεται στις ανάγκες της εταιρείας σας.

- [Η αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) είναι ενεργοποιημένη από προεπιλογή για εγκαταστάσεις express και σας βοηθά να εξασφαλίσετε ότι η έκδοση του Azure AD Σύνδεση είναι πάντα ενημερωμένη.
