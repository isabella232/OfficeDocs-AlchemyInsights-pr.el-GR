---
title: Ο κανόνας DLP για τον αριθμό διαβατηρίων ΗΠΑ/ΗΒ δεν λειτουργεί
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679224"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Προβλήματα με τους αριθμούς διαβατηρίων DLP-US/UK

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Θέματα DLP με αριθμούς διαβατηρίων ΗΠΑ/ΗΒ**

Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό διαβατηρίου ΗΠΑ/ΗΒ** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών DLP στο O365; Εάν Ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαιτούμενες πληροφορίες για όσα αναζητά η πολιτική DLP όταν αξιολογείται.
  
Για παράδειγμα, για μια πολιτική **αριθμών διαβατηρίων ΗΠΑ/ΗΒ** που έχει ρυθμιστεί με επίπεδο αξιοπιστίας 75%, τα παρακάτω αξιολογούνται και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας
  
- **[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Εννέα ψηφία

- **[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Εννέα διαδοχικά ψηφία

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, μέσα σε μια εγγύτητα των 300 χαρακτήρων:

  - Η συνάρτηση Func_usa_uk_passport εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Βρέθηκε μια λέξη-κλειδί από Keyword_passport.

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει την πολιτική **αριθμών διαβατηρίων ΗΠΑ/ΗΒ** : αριθμός διαβατηρίου 123456789

Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για την ανίχνευση ενός αριθμού διαβατηρίου ΗΠΑ/ΗΒ για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για τον αριθμό διαβατηρίων ΗΠΑ/ΗΒ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Με τη χρήση διαφορετικού ενσωματωμένου τύπου ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  