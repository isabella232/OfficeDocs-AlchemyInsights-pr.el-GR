---
title: 'AIP: Οι πολιτικές δεν συμπεριφέρονται όπως αναμένεται'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506558"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Οι πολιτικές δεν συμπεριφέρονται όπως αναμένεται

Προστασία πληροφοριών Azure: Οι πολιτικές δεν συμπεριφέρονται όπως αναμένεται, ανατρέξτε στα παρακάτω για τις προτεινόμενες οδηγίες για διάφορα ζητήματα πολιτικής:

1. Εάν αντιμετωπίζετε προβλήματα με οπτικές σημάνσεις, ανατρέξτε [στο θέμα Όταν εφαρμόζονται οπτικές σημάνσεις](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Εάν αντιμετωπίζετε προβλήματα με την αυτόματη επισήμανση, ανατρέξτε στο [θέμα Τρόπος ρύθμισης παραμέτρων συνθηκών για την αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και [τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Εάν αντιμετωπίζετε προβλήματα με την προστασία εγγενούς/pfile, εξετάστε [τη ρύθμιση παραμέτρων API αρχείου](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Ελέγξτε εάν χρησιμοποιείτε πολιτικές εμβέλειας που δεν έχουν ρυθμιστεί σωστά: [Πώς να ρυθμίσετε τις παραμέτρους της πολιτικής προστασίας πληροφοριών Azure για συγκεκριμένους χρήστες, χρησιμοποιώντας πολιτικές εμβέλειας](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Εάν η αυτόματη επισήμανση δεν λειτουργεί για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι το DRMEncryptProperty δεν έχει οριστεί όπως περιγράφεται εδώ: [ρυθμίσεις μητρώου IRM για ασφάλεια](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, συλλέξτε αρχεία καταγραφής υπολογιστών-πελατών προστασίας πληροφοριών Azure και επισυνάψτε τα αρχεία καταγραφής που έχουν εξαχθεί σε αυτό το δελτίο.

1. Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.
2. Κάντε κλικ στην επιλογή **Προστασία/Ευαισθησία**  >  **Βοήθεια και ανατροφοδότηση**.
3. Κάντε κλικ στην επιλογή **Εξαγωγή αρχείων καταγραφής**.
4. Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή τοποθεσίας σας και επισυνάψτε τα σε αυτήν την αίτηση υπηρεσίας.

Πρόσθετοι πόροι:

- [Τρόπος ρύθμισης παραμέτρων ετικέτας για οπτικές σημάνσεις για προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Αναθεώρηση της τεκμηρίωσης προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Χρήση ετικετών ευαισθησίας σε εφαρμογές του Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

