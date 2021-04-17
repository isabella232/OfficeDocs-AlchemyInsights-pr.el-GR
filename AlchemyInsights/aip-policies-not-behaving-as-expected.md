---
title: 'AIP: Οι πολιτικές δεν συμπεριφέρεται όπως αναμένεται'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821627"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Οι πολιτικές δεν συμπεριφέρεται όπως αναμένεται

Προστασία πληροφοριών Azure: Οι πολιτικές δεν συμπεριφέρεται όπως αναμένεται, ανατρέξτε στα παρακάτω για προτεινόμενες οδηγίες για διάφορα ζητήματα πολιτικής:

1. Εάν αντιμετωπίζετε προβλήματα με τις οπτικές σημάνσεις, ελέγξτε [πότε εφαρμόζονται οπτικές σημάνσεις.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Εάν αντιμετωπίζετε προβλήματα με την αυτόματη σήμανση, ανατρέξτε στο θέμα Πώς μπορείτε να ρυθμίσετε τις παραμέτρους των συνθηκών για την αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και τι θα αναζητήσουν [οι τύποι ευαίσθητων πληροφοριών.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Εάν αντιμετωπίζετε προβλήματα με την προστασία native/Pfile, εξετάστε τη ρύθμιση [παραμέτρων του File API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Ελέγξτε εάν χρησιμοποιείτε πολιτικές εμβέλειας που δεν έχουν ρυθμιστεί σωστά: Πώς μπορείτε να ρυθμίσετε τις παραμέτρους της πολιτικής προστασίας πληροφοριών Azure για συγκεκριμένους [χρήστες, χρησιμοποιώντας πολιτικές εμβέλειας.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Εάν η αυτόματη σήμανση δεν λειτουργεί για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι το DRMEncryptProperty δεν έχει οριστεί όπως περιγράφεται εδώ: Ρυθμίσεις μητρώου [IRM για την ασφάλεια.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, συλλέξτε αρχεία καταγραφής προγράμματος-πελάτη προστασίας πληροφοριών Azure και επισυνάψτε τα αρχεία καταγραφής που έχουν εξαχθεί σε αυτό το δελτίο.

1. Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.
2. Κάντε κλικ **στην επιλογή "Προστασία/Ευαισθησία**  >  **βοήθειας και σχολίων".**
3. Κάντε κλικ στην **επιλογή "Εξαγωγή αρχείων καταγραφής".**
4. Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή της τοποθεσίας σας και επισυνάψτε τα σε αυτή την αίτηση υπηρεσίας.

Πρόσθετοι πόροι:

- [Τρόπος ρύθμισης παραμέτρων ετικέτας για οπτικές σημάνσεις για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Αναθεώρηση της τεκμηρίωσης προστασίας πληροφοριών azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Χρήση ετικετών ευαισθησίας σε εφαρμογές του Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

