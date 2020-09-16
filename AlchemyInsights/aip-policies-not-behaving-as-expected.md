---
title: 'AIP: πολιτικές που δεν συμπεριφέρονται όπως αναμένεται'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663189"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: πολιτικές που δεν συμπεριφέρονται όπως αναμένεται

Προστασία πληροφοριών Azure: πολιτικές που δεν συμπεριφέρονται όπως αναμένεται, ανατρέξτε στα παρακάτω για τις προτεινόμενες οδηγίες για διάφορα θέματα πολιτικής:

1. Εάν αντιμετωπίζετε προβλήματα με οπτικές σημάνσεις, ανατρέξτε στο θέμα [πότε εφαρμόζονται οπτικές σημάνσεις](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Εάν αντιμετωπίζετε προβλήματα με την αυτόματη σήμανση, εξετάστε τον τρόπο με τον οποίο μπορείτε [να ρυθμίσετε τις παραμέτρους για την αυτόματη και συνιστώμενη ταξινόμηση για την προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και [Τι αναζητούν οι ευαίσθητοι τύποι πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Εάν αντιμετωπίζετε προβλήματα με την εγγενή/Pfile προστασία, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων API αρχείου](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Βεβαιωθείτε ότι χρησιμοποιείτε πολιτικές εύρους που δεν έχουν ρυθμιστεί σωστά: [Πώς μπορείτε να ρυθμίσετε τις παραμέτρους της πολιτικής προστασίας πληροφοριών Azure για συγκεκριμένους χρήστες χρησιμοποιώντας πολιτικές εύρους](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Εάν η αυτόματη σήμανση δεν λειτουργεί για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι το DRMEncryptProperty δεν έχει οριστεί όπως περιγράφεται εδώ: [ρυθμίσεις μητρώου IRM για την ασφάλεια](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, παρακαλούμε να συλλέξετε αρχεία καταγραφής προγράμματος-πελάτη προστασίας πληροφοριών Azure και να επισυνάψετε τα αρχεία καταγραφής που έχουν εξαχθεί σε αυτό το εισιτήριο.

1. Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.
2. Κάντε κλικ στην επιλογή **προστασία/**  >  **Βοήθεια με ευαισθησία και σχόλια**.
3. Κάντε κλικ στην επιλογή **εξαγωγή αρχείων καταγραφής**.
4. Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή της τοποθεσίας σας και επισυνάψτε τα σε αυτή την αίτηση εξυπηρέτησης.

Πρόσθετοι πόροι:

- [Πώς μπορείτε να ρυθμίσετε τις παραμέτρους μιας ετικέτας για οπτικές σημάνσεις για την προστασία πληροφοριών του Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Αναθεώρηση τεκμηρίωσης προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Χρήση ετικετών ευαισθησίας στις εφαρμογές του Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

