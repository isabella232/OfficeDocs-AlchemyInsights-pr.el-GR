---
title: 646 πώς μπορείτε να ρυθμίσετε τις παραμέτρους του AADConnect
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704489"
---
# <a name="configure-sync-features"></a>Ρύθμιση παραμέτρων δυνατοτήτων συγχρονισμού

Το Azure AD Connect περιλαμβάνει διάφορες δυνατότητες που είναι ενεργοποιημένες από προεπιλογή ή τις οποίες μπορείτε να ενεργοποιήσετε αργότερα. Ορισμένες δυνατότητες απαιτούν πρόσθετες ρυθμίσεις παραμέτρων σε συγκεκριμένα περιβάλλοντα.

- Περιορισμοί [φιλτραρίσματος](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) τα αντικείμενα συγχρονίζονται με το Azure AD. Από προεπιλογή, όλοι οι χρήστες, οι επαφές, οι ομάδες και οι λογαριασμοί υπολογιστή με Windows 10 συγχρονίζονται. Μπορείτε να συμπεριλάβετε ή να εξαιρέσετε αντικείμενα που βασίζονται σε τομείς, οργανικές μονάδες ή άλλα χαρακτηριστικά.

- [Συγχρονισμός κατακερματισμού κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) συγχρονίζει τον κατακερματισμό κωδικού πρόσβασης από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης στο Azure AD. Αυτό επιτρέπει τη διαχείριση κωδικών πρόσβασης σε μία θέση, αλλά τη χρήση του ίδιου κωδικού πρόσβασης σε περιβάλλοντα εσωτερικής εγκατάστασης και cloud. Επειδή η υπηρεσία καταλόγου Active Directory είναι η έγκυρη προέλευση, μπορείτε να χρησιμοποιήσετε τις δικές σας πολιτικές κωδικών πρόσβασης.

- Η [Επαναφορά κωδικού πρόσβασης από το χρήστη (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) επιτρέπει στους χρήστες να επαναφέρουν τους δικούς τους κωδικούς πρόσβασης στο cloud, ενώ εξακολουθούν να εφαρμόζουν την πολιτική κωδικού πρόσβασης εσωτερικής εγκατάστασης.

- Το [Device αντιγραφής](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) επιτρέπει την εγγραφή των εγγεγραμμένων συσκευών στο Azure AD στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, ώστε να μπορούν να χρησιμοποιηθούν για πρόσβαση υπό όρους.

- [Αποτροπή τυχαίων](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) διαγραφών είναι ενεργοποιημένη από προεπιλογή για να αποτρέψετε πάρα πολλές ταυτόχρονες διαγραφές αντικειμένων (περισσότερα από 500 αντικείμενα ανά συγχρονισμό). Μπορείτε να αλλάξετε αυτήν τη ρύθμιση για να ικανοποιήσετε τις ανάγκες της εταιρείας σας.

- Η [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) είναι ενεργοποιημένη από προεπιλογή για τις γρήγορες εγκαταστάσεις και σας βοηθά να διασφαλίσετε ότι η έκδοση του Azure AD Connect είναι πάντα τρέχουσα.
