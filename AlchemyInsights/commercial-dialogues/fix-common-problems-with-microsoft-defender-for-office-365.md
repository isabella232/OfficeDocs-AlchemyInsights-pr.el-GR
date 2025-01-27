---
title: Επιδιόρθωση συνηθισμένων προβλημάτων με τον Microsoft Defender για Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330060"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Επιδιόρθωση συνηθισμένων προβλημάτων με τον Microsoft Defender για Office 365

Ακολουθούν ορισμένες λύσεις για συνήθη προβλήματα με τον Microsoft Defender για Office 365:

- **Καθυστέρηση μηνύματος:**

  Οι καθυστερήσεις στην παράδοση ηλεκτρονικού ταχυδρομείου μπορεί να προκαλέσουν Θυρίδα συνημμένα σάρωσης μηνυμάτων. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Θυρίδα ρυθμίσεις πολιτικής συνημμένων.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Αναφορά ψευδών θετικών ή αρνητικών αποτελεσμάτων:**

  Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Αναφορά μηνυμάτων και αρχείων στη Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Ενεργοποίηση Θυρίδα σύνδεσης:**

  1. Στην πύλη Microsoft 365 Defender, μεταβείτε στην ενότητα "Ηλεκτρονικό ταχυδρομείο& πολιτικές συνεργασίας & πολιτικές απειλής <https://security.microsoft.com/>  \>  \>  \> **κανόνων Θυρίδα συνδέσεις** στην ενότητα **"Πολιτικές".**

     Για να μεταβείτε απευθείας στη **Θυρίδα "Συνδέσεις",** χρησιμοποιήστε <https://security.microsoft.com/safelinksv2> το .

  2. Στη σελίδα **Θυρίδα "Συνδέσεις",** επιλέξτε την πολιτική κάνοντας κλικ στο όνομα της πολιτικής.
  3. Στο αναδυόμενο παράθυρο λεπτομερειών που εμφανίζεται, κάντε ένα από τα παρακάτω βήματα:
     - Για να προσθέσετε μια νέα πολιτική, επιλέξτε **+ Δημιουργία.** Θα ξεκινήσει ένας οδηγός για να σας βοηθήσει να ορίσετε τις ρυθμίσεις πολιτικής σας.
     - Για να επεξεργαστείτε μια υπάρχουσα πολιτική, επιλέξτε την πολιτική κάνοντας κλικ στο όνομα της πολιτικής. Στο αναδυόμενο στοιχείο λεπτομερειών που εμφανίζεται, επιλέξτε **"Επεξεργασία"** στην **ενότητα "Ρυθμίσεις προστασίας".**
  4. Στη σελίδα **"Ρυθμίσεις προστασίας",** ρυθμίστε τις παραμέτρους των ακόλουθων ρυθμίσεων:
     - Ενεργοποιήστε **την επιλογή της ενέργειας για άγνωστες ενδεχομένως κακόβουλες διευθύνσεις URL στα μηνύματα.**
     - Επιλέξτε **"Εφαρμογή ασφαλών συνδέσεων" σε μηνύματα που αποστέλλονται εντός του οργανισμού.**

  Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Θυρίδα Συνδέσεις στο Microsoft Defender για Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
