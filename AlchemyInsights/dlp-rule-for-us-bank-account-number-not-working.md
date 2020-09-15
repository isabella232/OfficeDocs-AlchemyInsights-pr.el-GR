---
title: Ο κανόνας DLP για τον αριθμό τραπεζικού λογαριασμού των ΗΠΑ δεν λειτουργεί
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679296"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Θέματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Θέματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ**

Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για το περιεχόμενο που περιέχει έναν **αριθμό τραπεζικού λογαριασμού των ΗΠΑ** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών DLP στο O365; Εάν Ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαιτούμενες πληροφορίες για όσα αναζητά η πολιτική DLP όταν αξιολογείται.
  
Για παράδειγμα, για μια πολιτική **αριθμού τραπεζικού λογαριασμού των ΗΠΑ** που έχει ρυθμιστεί με επίπεδο αξιοπιστίας 85%, τα παρακάτω αξιολογούνται και πρέπει να ανιχνευθούν για να ενεργοποιείται ο κανόνας:
  
- **[Μορφοποίηση:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 ψηφία

- **[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 διαδοχικά ψηφία.

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, μέσα σε μια εγγύτητα των 300 χαρακτήρων:

  - Η κανονική παράσταση Regex_usa_bank_account_number εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο

  - Βρέθηκε μια λέξη-κλειδί από Keyword_usa_Bank_Account.

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει την πολιτική **αριθμού λογαριασμού της αμερικανικής τράπεζας** : έλεγχος του λογαριασμού 78344011

Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον **αριθμό τραπεζικού λογαριασμού των ΗΠΑ** που θα ανιχνευθεί για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για τον αριθμό τραπεζικού λογαριασμού των ΗΠΑ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Με τη χρήση διαφορετικού ενσωματωμένου τύπου ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  