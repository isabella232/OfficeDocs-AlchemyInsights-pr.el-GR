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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679441"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Θέματα DLP με αριθμούς πιστωτικών καρτών

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Θέματα DLP με αριθμούς πιστωτικών καρτών**

Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για το περιεχόμενο που περιέχει έναν **αριθμό πιστωτικής κάρτας** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365; Εάν Ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαιτούμενες πληροφορίες για να ενεργοποιήσετε την πολιτική DLP όταν αξιολογείται. Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** που έχει ρυθμιστεί με επίπεδο αξιοπιστίας 85%, τα παρακάτω αξιολογούνται και πρέπει να ανιχνευθούν για να ενεργοποιείται ο κανόνας:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 ψηφία τα οποία μπορούν να μορφοποιηθούν ή να μην μορφοποιηθούν (dddddddddddddddd) και πρέπει να περάσουν από τη δοκιμή Luhn.

- **[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Πολύ περίπλοκο και στιβαρό μοτίβο που εντοπίζει κάρτες από όλες τις μεγάλες μάρκες παγκοσμίως, όπως βίζα, MasterCard, κάρτα Discover, JCB, American Express, δωροκάρτες και κάρτες Diner.

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, μέσα σε μια εγγύτητα των 300 χαρακτήρων:

  - Η συνάρτηση Func_credit_card εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Ισχύει ένα από τα εξής:

  - Βρέθηκε μια λέξη-κλειδί από Keyword_cc_verification.

  - Βρέθηκε μια λέξη-κλειδί από Keyword_cc_name

  - Η συνάρτηση Func_expiration_date εντοπίζει μια ημερομηνία στη σωστή μορφή ημερομηνίας.

  - Οι φάσεις του αθροίσματος ελέγχου

    Για παράδειγμα, το ακόλουθο δείγμα θα προκαλέσει μια πολιτική αριθμών πιστωτικής κάρτας DLP:

  - Βίζα: 4485 3647 3952 7352
  
  - Λήγει: 2/2009

Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για την ανίχνευση ενός **αριθμού πιστωτικής κάρτας** για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για την πιστωτική κάρτα #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Με τη χρήση διαφορετικού ενσωματωμένου τύπου ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  