---
title: Ο κανόνας DLP για τον αριθμό πιστωτικής κάρτας δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005090"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Προβλήματα DLP με αριθμούς πιστωτικών καρτών

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Προβλήματα DLP με αριθμούς πιστωτικών καρτών**

Αντιμετωπίζετε προβλήματα με την Αποτροπή απώλειας δεδομένων **(DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει έναν αριθμό πιστωτικής κάρτας όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365;  Εάν ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την ενεργοποίηση της πολιτικής DLP κατά την αξιολόγηση. Για παράδειγμα,  για μια πολιτική πιστωτικής κάρτας που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα εξής και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:
  
- **[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 ψηφία που μπορούν να μορφοποιήσετε ή να μορφοποιήσετε (ddddddd) και πρέπει να περάσουν τον έλεγχο Luhn.

- **[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Πολύ σύνθετο και ισχυρό μοτίβο που εντοπίζει κάρτες από όλες τις κύριες επωνυμίες παγκοσμίως, όπως κάρτες Visa, MasterCard, Discover Card, JCB, American Express, δωροκάρτες και κάρτες δείπνου.

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Μια πολιτική DLP είναι 85% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε απόσταση 300 χαρακτήρων:

  - Η συνάρτηση Func_credit_card εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Ισχύει ένα από τα εξής:

  - Μια λέξη-κλειδί από Keyword_cc_verification βρέθηκε.

  - Βρέθηκε μια λέξη-Keyword_cc_name από το Keyword_cc_name

  - Η συνάρτηση Func_expiration_date βρίσκει μια ημερομηνία στη σωστή μορφή ημερομηνίας.

  - Το άθροισμα ελέγχου περνά

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε μια πολιτική αριθμού πιστωτικής κάρτας DLP:

  - Visa: 4485 3647 3952 7352
  
  - Λήγει: 2/2009

Για περισσότερες πληροφορίες σχετικά με  το τι απαιτείται για τον εντοπισμό ενός αριθμού πιστωτικής κάρτας για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: Τι είναι οι τύποι ευαίσθητων πληροφοριών για [την πιστωτική κάρτα#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: Τι θα αναζητήσουν οι [τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  