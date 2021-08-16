---
title: Ο κανόνας DLP για τον αριθμό διαβατηρίου Η.Π.Α./Ηνωμένου Βασιλείου δεν λειτουργεί
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004946"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Προβλήματα με τους αριθμούς διαβατηρίων DLP - Η.Π.Α./Ηνωμένου Βασιλείου

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Προβλήματα DLP με αριθμούς διαβατηρίων Η.Π.Α./Ηνωμένου Βασιλείου**

Αντιμετωπίζετε προβλήματα με την Αποτροπή απώλειας δεδομένων **(DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει έναν αριθμό διαβατηρίου **Η.Π.Α./Ηνωμένου** Βασιλείου όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365; Εάν ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για αυτό που αναζητά η πολιτική DLP κατά την αξιολόγηση.
  
Για παράδειγμα, για μια πολιτική αριθμού διαβατηρίου **Η.Π.Α./Ηνωμένου** Βασιλείου που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 75%, αξιολογούνται τα εξής και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας
  
- **[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Εννέα ψηφία

- **[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Εννέα διαδοχικά ψηφία

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Μια πολιτική DLP είναι 75% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε απόσταση 300 χαρακτήρων:

  - Η συνάρτηση Func_usa_uk_passport εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Βρέθηκε μια λέξη-Keyword_passport από το <a0>.</Keyword_passport</a0>

    Για παράδειγμα, το ακόλουθο δείγμα  θα ενεργοποιούσε την πολιτική αριθμού διαβατηρίου Η.Π.Α./Ηνωμένου Βασιλείου: Αριθμός διαβατηρίου Η.Π.Α. 123456789

Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό ενός αριθμού διαβατηρίου Η.Π.Α./Ηνωμένου Βασιλείου για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: Τι βλέπουν οι τύποι ευαίσθητων πληροφοριών για τον αριθμό διαβατηρίου [Η.Π.Α./Ηνωμένου Βασιλείου](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: Τι θα αναζητήσουν οι [τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  