---
title: Κανόνας DLP για τον αριθμό πιστωτικής κάρτας που δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704201"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Ζητήματα DLP με αριθμούς πιστωτικών καρτών

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Ζητήματα DLP με αριθμούς πιστωτικών καρτών**

Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό πιστωτικής κάρτας** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365; Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για να ενεργοποιήσετε την πολιτική DLP κατά την αξιολόγησή της. Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:
  
- **[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ψηφία που μπορούν να μορφοποιηθεί ή χωρίς μορφοποίηση (ddddddddddddddddddd) και πρέπει να περάσει τη δοκιμή Luhn.

- **[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Πολύ πολύπλοκο και στιβαρό μοτίβο που ανιχνεύει κάρτες από όλες τις μεγάλες μάρκες σε όλο τον κόσμο, συμπεριλαμβανομένων των Visa, MasterCard, Discover Card, JCB, American Express, δωροκαρτών και καρτών γευματοειδών.

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn

- **[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:

  - Η συνάρτηση Func_credit_card εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Ένα από τα εξής είναι αλήθεια:

  - Βρέθηκε μια λέξη-κλειδί από Keyword_cc_verification.

  - Βρέθηκε μια λέξη-κλειδί από Keyword_cc_name

  - Η συνάρτηση Func_expiration_date βρίσκει μια ημερομηνία στη σωστή μορφή ημερομηνίας.

  - Το άθροισμα ελέγχου περνά

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε για μια πολιτική αριθμού πιστωτικής κάρτας DLP:

  - Βίζα: 4485 3647 3952 7352
  
  - Λήξη: 2/2009

Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό **ενός αριθμού πιστωτικής κάρτας** για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για την πιστωτική κάρτα#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  