---
title: Ο κανόνας DLP για τον αριθμό τραπεζικού λογαριασμού Η.Π.Α. δεν λειτουργεί
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005018"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Προβλήματα DLP με αριθμούς τραπεζικού λογαριασμού Η.Π.Α.

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Προβλήματα DLP με αριθμούς τραπεζικού λογαριασμού Η.Π.Α.**

Αντιμετωπίζετε προβλήματα με την Αποτροπή απώλειας δεδομένων **(DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει έναν αριθμό τραπεζικού λογαριασμού Η.Π.Α., όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365;  Εάν ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για αυτό που αναζητά η πολιτική DLP κατά την αξιολόγηση.
  
Για παράδειγμα,  για μια πολιτική αριθμού τραπεζικού λογαριασμού Η.Π.Α. που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα εξής και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:
  
- **[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 ψηφία

- **[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 διαδοχικά ψηφία.

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Μια πολιτική DLP είναι 75% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε απόσταση 300 χαρακτήρων:

  - Η κανονική παράσταση Regex_usa_bank_account_number βρίσκει περιεχόμενο που ταιριάζει με το μοτίβο

  - Μια λέξη-κλειδί από Keyword_usa_Bank_Account βρέθηκε.

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε για την πολιτική "Αριθμός τραπεζικού λογαριασμού **Η.Π.Α.":** Έλεγχος 78344011

Για περισσότερες πληροφορίες σχετικά με  το τι απαιτείται για τον εντοπισμό ενός αριθμού τραπεζικού λογαριασμού Η.Π.Α. για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: Τι φαίνεται στους τύπους ευαίσθητων πληροφοριών για τον αριθμό τραπεζικού [λογαριασμού Η.Π.Α.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: Τι θα αναζητήσουν οι [τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  