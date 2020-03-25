---
title: Κανόνας DLP για ssn δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932522"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP θέματα με αριθμούς κοινωνικής ασφάλισης

**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο. Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας. Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.

Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας. Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων. Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.

**Ζητήματα DLP με τα SSN**

Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό κοινωνικής ασφάλισης (SSN)** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών στο Office 365; Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την αναζήτηση της πολιτικής DLP. 
  
Για παράδειγμα, για μια πολιτική SSN που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:
  
- **[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ψηφία, τα οποία μπορεί να είναι σε μορφοποιημένο ή μη μορφοποιημένο μοτίβο

- **[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις συναρτήσεις αναζητούν SSNs σε τέσσερα διαφορετικά μοτίβα:

  - Func_ssn εντοπίζει SSN με ισχυρή μορφοποίηση πριν από το 2011 που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (dd-dd-dddd ή ddd ddd ddd dddd dd dddd)

  - Func_unformatted_ssn εντοπίζει SSN με ισχυρή μορφοποίηση πριν από το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (dddddddd)

  - Func_randomized_formatted_ssn εντοπίζει ssns μετά το 2011 που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (ddd-dd-dddd ή ddd ddd ddd dddd)

  - Func_randomized_unformatted_ssn εντοπίζει ssns μετά το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (dddddddd)

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:

  - Η [συνάρτηση Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Βρέθηκε μια λέξη-κλειδί από [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) Παραδείγματα λέξεων-κλειδιών περιλαμβάνουν: *Κοινωνική Ασφάλιση, Κοινωνική Ασφάλιση#, Soc Sec , SSN* . Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική DLP SSN: **SSN: 489-36-8350**
  
Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό των SSN για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα αυτού του άρθρου: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  