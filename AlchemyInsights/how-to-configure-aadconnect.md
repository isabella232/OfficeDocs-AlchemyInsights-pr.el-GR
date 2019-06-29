---
title: 646 Τρόπος ρύθμισης των παραμέτρων AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385339"
---
# <a name="configure-sync-features"></a>Ρυθμίσετε τις δυνατότητες συγχρονισμού

Σύνδεση AD Azure περιλαμβάνει διάφορες δυνατότητες που ενεργοποιούνται από προεπιλογή ή που μπορείτε να ενεργοποιήσετε αργότερα. Ορισμένες δυνατότητες απαιτούν πρόσθετες ρυθμίσεις παραμέτρων στο συγκεκριμένο περιβάλλον.

- [Φιλτράρισμα](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) όρια τα αντικείμενα συγχρονίζονται Azure AD. Από προεπιλογή, όλες οι χρήστες, επαφές, ομάδες, και Windows 10 λογαριασμούς υπολογιστών συγχρονίζονται. Μπορείτε να συμπεριλάβετε ή να εξαιρέσετε αντικείμενα που βασίζονται σε τομείς, οργανικές μονάδες ή άλλα χαρακτηριστικά.

- [Συγχρονισμός κατακερματισμού του κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) συγχρονίζει το κλειδί κατακερματισμού κωδικού πρόσβασης από το Active Directory εσωτερικής εγκατάστασης Azure AD. Αυτό επιτρέπει τη Διαχείριση κωδικού πρόσβασης σε μία θέση, αλλά τον ίδιο κωδικό πρόσβασης και στα δύο εσωτερικής εγκατάστασης και σύννεφο περιβάλλοντα. Επειδή η υπηρεσία καταλόγου Active Directory είναι η αξιόπιστη πηγή, μπορείτε να χρησιμοποιήσετε τις δικές σας πολιτικές κωδικού πρόσβασης.

- [Αυτοεξυπηρέτησης επαναφορά του κωδικού πρόσβασης (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) επιτρέπει στους χρήστες να επαναφέρετε τους κωδικούς πρόσβασής τους στο σύννεφο κατά την εφαρμογή εξακολουθεί να σας πολιτική κωδικού πρόσβασης σε χώρους.

- [Συσκευή αντιγραφής](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) επιτρέπει στις συσκευές εγγεγραμμένων στο Azure AD να συνταχθούν πίσω στο Active Directory εσωτερικής εγκατάστασης ώστε να μπορεί να χρησιμοποιηθεί για την υπό όρους πρόσβαση.

- [Αποτροπή ακούσιας διαγραφών](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) είναι ενεργοποιημένη από προεπιλογή για την αποτροπή διαγραφές πάρα πολλές ταυτόχρονες αντικειμένου (περισσότερα από 500 αντικείμενα ανά συγχρονισμού). Μπορείτε να αλλάξετε αυτήν τη ρύθμιση για τις ανάγκες της εταιρείας σας.

- [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) είναι ενεργοποιημένη από προεπιλογή για εγκαταστάσεις express και διασφαλίζει τη δική σας έκδοση του σύνδεση AD Azure είναι πάντα ενημερωμένα.
