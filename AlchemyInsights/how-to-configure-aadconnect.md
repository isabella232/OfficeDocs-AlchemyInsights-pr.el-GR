---
title: 646 Τρόπος ρύθμισης παραμέτρων του AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722541"
---
# <a name="configure-sync-features"></a>Ρύθμιση παραμέτρων δυνατοτήτων συγχρονισμού

Το Azure AD Connect περιλαμβάνει πολλές δυνατότητες που είναι ενεργοποιημένες από προεπιλογή ή τις οποίες μπορείτε να ενεργοποιήσετε αργότερα. Ορισμένες δυνατότητες απαιτούν πρόσθετες ρυθμίσεις παραμέτρων σε συγκεκριμένα περιβάλλοντα.

- [Το φιλτράρισμα](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) περιορίζει τα αντικείμενα που συγχρονίζονται με Azure AD. Από προεπιλογή, συγχρονίζονται όλοι οι χρήστες, οι επαφές, οι ομάδες και οι λογαριασμοί υπολογιστών των Windows 10. Μπορείτε να συμπεριλάβετε ή να εξαιρέσετε αντικείμενα που βασίζονται σε τομείς, δικαιώματα οδοποιίας ή άλλα χαρακτηριστικά.

- [Ο συγχρονισμός κατακερματισμού κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) συγχρονίζει τον κατακερματισμό κωδικού πρόσβασης από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης σε Azure AD. Αυτό επιτρέπει τη διαχείριση κωδικών πρόσβασης σε μία θέση, αλλά τη χρήση του ίδιου κωδικού πρόσβασης τόσο σε περιβάλλονεσωτερικής εγκατάστασης όσο και σε περιβάλλοντα cloud. Επειδή η υπηρεσία καταλόγου Active Directory είναι η έγκυρη προέλευση, μπορείτε να χρησιμοποιήσετε τις δικές σας πολιτικές κωδικού πρόσβασης.

- [Η επαναφορά κωδικού πρόσβασης από το χρήστη (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) επιτρέπει στους χρήστες να επαναφέρουν τους δικούς τους κωδικούς πρόσβασης στο cloud, ενώ εξακολουθούν να εφαρμόζουν την πολιτική κωδικού πρόσβασης εσωτερικής εγκατάστασης.

- [Η επαναφορά συσκευής](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) επιτρέπει την εγγραφή καταχωρημένων συσκευών στο Azure AD στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, ώστε να μπορούν να χρησιμοποιηθούν για πρόσβαση υπό όρους.

- [Η αποτροπή τυχαίων διαγραφών](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) είναι ενεργοποιημένη από προεπιλογή για την αποτροπή πάρα πολλών ταυτόχρονων διαγραφών αντικειμένων (περισσότερα από 500 αντικείμενα ανά συγχρονισμό). Μπορείτε να αλλάξετε αυτήν τη ρύθμιση για να ικανοποιήσετε τις ανάγκες του οργανισμού σας.

- [Η αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) είναι ενεργοποιημένη από προεπιλογή για τις εγκαταστάσεις εξπρές και διασφαλίζει ότι η έκδοση του Azure AD Connect είναι πάντα τρέχουσα.
