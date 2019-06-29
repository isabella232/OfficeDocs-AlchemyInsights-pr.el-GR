---
title: Τεχνολογία DLP κανόνα για τον αριθμό της πιστωτικής κάρτας που δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389577"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Τεχνολογία DLP ζητήματα με αριθμούς πιστωτικών καρτών

Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει έναν **Αριθμό πιστωτικής κάρτας** , όταν χρησιμοποιείτε έναν τύπο ευαίσθητες πληροφορίες DLP σε O365; Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την ενεργοποίηση της πολιτικής DLP όταν που αξιολογείται. Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** έχει ρυθμιστεί με ένα επίπεδο εμπιστοσύνης του 85%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης:
  
- **[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ψηφία, τα οποία μπορούν να διαμορφωθούν ή μη μορφοποιημένο (dddddddddddddddd) και πρέπει να περάσει τη δοκιμή Luhn.

- **[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Πολύ περίπλοκη και ισχυρή μοτίβο που εντοπίζει κάρτες από σε όλο τον κόσμο, συμπεριλαμβανομένης της θεώρησης, MasterCard, ανακαλύψετε κάρτα, JCB, American Express, δώρο κάρτες και κάρτες diner κύρια σήματα.

- **[Αθροίσματος ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn

- **[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Μια πολιτική DLP είναι 85% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες:

  - Η συνάρτηση Func_credit_card εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο.

  - Ένα από τα παρακάτω είναι αληθές:

  - Μπορείτε να βρείτε μια λέξη-κλειδί από το Keyword_cc_verification.

  - Βρέθηκε μια λέξη-κλειδί από το Keyword_cc_name

  - Η συνάρτηση Func_expiration_date βρίσκει μια ημερομηνία στη μορφή ημερομηνίας δεξιά.

  - Μεταβιβάζει το άθροισμα ελέγχου

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για τεχνολογία DLP πολιτική αριθμό πιστωτικής κάρτας:

  - Θεώρηση: 7352 3952 3647 4485
  
  - Λήξη: 2/2009

Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για έναν **Αριθμό πιστωτικής κάρτας** που θα εντοπιστούν για το περιεχόμενο, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών αναζητήστε πιστωτική κάρτα #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  