---
title: Κανόνας DLP για τον αριθμό τραπεζικού λογαριασμού των ΗΠΑ που δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977162"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Ζητήματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ

**Σημαντικό:** Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες – Επισκεφθείτε [τις προσωρινές προσαρμογές δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Ζητήματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ**

Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **έναν αριθμό τραπεζικού λογαριασμού των ΗΠΑ** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365; Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για αυτό που αναζητά η πολιτική DLP κατά την αξιολόγησή της.
  
Για παράδειγμα, για μια πολιτική **αριθμού τραπεζικού λογαριασμού των Η.Π.Α.** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:
  
- **[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 ψηφία

- **[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 συνεχόμενα ψηφία.

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:

  - Η κανονική έκφραση Regex_usa_bank_account_number βρίσκει περιεχόμενο που ταιριάζει με το μοτίβο

  - Βρέθηκε μια λέξη-κλειδί από Keyword_usa_Bank_Account.

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική **αριθμού τραπεζικού λογαριασμού ΗΠΑ:** Έλεγχος λογαριασμού 78344011

Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό ενός **αριθμού τραπεζικού λογαριασμού των ΗΠΑ** για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: Τι αναζητούν οι [Τύποι ευαίσθητων πληροφοριών για τον αριθμό τραπεζικού λογαριασμού ΤΩΝ ΗΠΑ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  