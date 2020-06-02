---
title: Η αυτόματη ταξινόμηση δεν συμπεριφέρεται όπως αναμένεται με το πρόγραμμα-πελάτη AIP
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
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493032"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Η αυτόματη ταξινόμηση δεν συμπεριφέρεται όπως αναμένεται με το πρόγραμμα-πελάτη AIP

Η αυτόματη ταξινόμηση δεν συμπεριφέρεται όπως αναμένεται, χρησιμοποιήστε τις ακόλουθες συνιστώμενες οδηγίες:

1. Εάν αντιμετωπίζετε προβλήματα με την αυτόματη επισήμανση, ανατρέξτε στο θέμα [Τρόπος ρύθμισης παραμέτρων συνθηκών για την αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και [τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. Ελέγξτε εάν χρησιμοποιείτε πολιτικές εμβέλειας που δεν έχουν ρυθμιστεί σωστά: [Πώς να ρυθμίσετε τις παραμέτρους της πολιτικής προστασίας πληροφοριών Azure για συγκεκριμένους χρήστες, χρησιμοποιώντας πολιτικές εμβέλειας](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Εάν η αυτόματη επισήμανση δεν λειτουργεί για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι `DRMEncryptProperty` δεν έχει οριστεί όπως περιγράφεται εδώ: ρυθμίσεις [μητρώου IRM για ασφάλεια](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Εάν χρησιμοποιήσατε [τους ενσωματωμένους τύπους πληροφοριών](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) για την πολιτική προστασίας πληροφοριών Azure, βεβαιωθείτε ότι το περιεχόμενό σας ταιριάζει με την αναμενόμενη μορφή.
5. Βεβαιωθείτε ότι η ετικέτα έχει ρυθμιστεί κατάλληλα για **αυτόματη** ή **συνιστώμενη**. (Η**αυτόματη** επισήμανση είναι διαθέσιμη για όλες τις εφαρμογές του Office, ενώ η **συνιστώμενη** είναι διαθέσιμη για όλες τις εφαρμογές του Office εκτός από το Outlook.)
6. Δεν μπορείτε να χρησιμοποιήσετε την αυτόματη ταξινόμηση για έγγραφα και μηνύματα ηλεκτρονικού ταχυδρομείου που προηγουμένως είχαν επισημανθεί με μη αυτόματο τρόπο ή προηγουμένως έχουν επισημανθεί αυτόματα με υψηλότερη ταξινόμηση.  Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα: [Πώς εφαρμόζονται οι αυτόματες ή οι προτεινόμενες ετικέτες](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, συλλέξτε αρχεία καταγραφής υπολογιστών-πελατών προστασίας πληροφοριών Azure και επισυνάψτε τα αρχεία καταγραφής που έχουν εξαχθεί στο δελτίο υποστήριξης. Για να εξαγάγετε αρχεία καταγραφής προστασίας πληροφοριών Azure:
    - Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.
    - Κάντε κλικ στην επιλογή **Προστασία/Ευαισθησία**  >  **Βοήθεια και ανατροφοδότηση**.
    - Κάντε κλικ στην επιλογή **Εξαγωγή αρχείων καταγραφής**.
    - Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή τοποθεσίας σας και επισυνάψτε τα στο αίτημα εξυπηρέτησης.

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

- [Τρόπος ρύθμισης παραμέτρων συνθηκών για αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Οδηγίες για κοινά σενάρια που χρησιμοποιούν την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Αναθεώρηση της τεκμηρίωσης προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Αναθεώρηση συνδρομών και δυνατοτήτων προστασίας πληροφοριών Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Απαιτήσεις για την προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Πρόγραμμα εκμάθησης γρήγορης εκκίνησης για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Λήψη προγράμματος-πελάτη προστασίας πληροφοριών Azure](https://www.microsoft.com/download/details.aspx?id=53018)
