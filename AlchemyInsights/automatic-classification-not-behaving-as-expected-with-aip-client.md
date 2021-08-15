---
title: Η αυτόματη ταξινόμηση δεν λειτουργεί ως αναμενόταν με το πρόγραμμα-πελάτη AIP
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979709"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Η αυτόματη ταξινόμηση δεν λειτουργεί ως αναμενόταν με το πρόγραμμα-πελάτη AIP

Η αυτόματη ταξινόμηση δεν λειτουργεί ως αναμενόταν, χρησιμοποιήστε τις παρακάτω προτεινόμενες οδηγίες:

1. Εάν αντιμετωπίζετε προβλήματα με την αυτόματη σήμανση, ανατρέξτε στο θέμα [Τρόπος ρύθμισης συνθηκών για την αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Ελέγξτε εάν χρησιμοποιείτε πολιτικές εμβέλειας που δεν έχουν ρυθμιστεί καταλλήλως: [Τρόπος ρύθμισης της πολιτικής Προστασίας πληροφοριών Azure για συγκεκριμένους χρήστες, χρησιμοποιώντας πολιτικές εμβέλειας](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Αν δεν λειτουργεί η αυτόματη σήμανση για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι το `DRMEncryptProperty` δεν έχει οριστεί όπως περιγράφεται εδώ: [Ρυθμίσεις μητρώου IRM για την ασφάλεια](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Εάν χρησιμοποιήσατε τους [ενσωματωμένους τύπους πληροφοριών](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) για την πολιτική Προστασίας πληροφοριών Azure, επιβεβαιώστε ότι το περιεχόμενό σας αντιστοιχεί στην αναμενόμενη μορφή.
5. Βεβαιωθείτε ότι η ετικέτα έχει ρυθμιστεί κατάλληλα για την **Αυτόματη** ή **Συνιστώμενη**. (Η **Αυτόματη** σήμανση είναι διαθέσιμη για όλες τις εφαρμογές του Microsoft 365, ενώ η **Συνιστώμενη** είναι διαθέσιμη για όλες τις εφαρμογές του Microsoft 365 εκτός από το Outlook.)
6. Δεν μπορείτε να χρησιμοποιήσετε την αυτόματη ταξινόμηση για έγγραφα και μηνύματα ηλεκτρονικού ταχυδρομείου τα οποία είχαν προηγουμένως επισημανθεί με ετικέτες υψηλότερης διαβάθμισης με αυτόματο ή με μη αυτόματο τρόπο.  Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα: [Πώς εφαρμόζονται οι αυτόματες ή οι συνιστώμενες ετικέτες](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, συλλέξτε αρχεία καταγραφής προγράμματος-πελάτη της Προστασίας πληροφοριών Azure και επισυνάψτε τα εξαγόμενα αρχεία καταγραφής στο δελτίο υποστήριξης. Για να εξάγετε αρχεία καταγραφής της Προστασίας πληροφοριών Azure:
    - Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.
    - Κάντε κλικ στην **Προστασία/Ευαισθησία** > **Βοήθεια και σχόλια**.
    - Κάντε κλικ στην **Εξαγωγή αρχείων καταγραφής**.
    - Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή θέσης σας και επισυνάψτε τα στην αίτηση εξυπηρέτησης.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα: 

- [Πώς να ρυθμίσετε τις παραμέτρους συνθηκών για αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Οδηγοί για συνηθισμένα σενάρια που χρησιμοποιούν την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Αναθεώρηση τεκμηρίωσης της Προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Αναθεώρηση των συνδρομών και δυνατοτήτων της Προστασίας πληροφοριών Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Απαιτήσεις για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Εκμάθηση γρήγορης εκκίνησης για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Λήψη προγράμματος-πελάτη Προστασίας πληροφοριών Azure](https://www.microsoft.com/download/details.aspx?id=53018)
