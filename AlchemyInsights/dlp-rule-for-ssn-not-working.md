---
title: Κανόνας DLP για ssn δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507370"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP θέματα με αριθμούς κοινωνικής ασφάλισης

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Ζητήματα DLP με τα SSN**

Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό κοινωνικής ασφάλισης (SSN)** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών στο Microsoft 365; Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την αναζήτηση της πολιτικής DLP. 
  
Για παράδειγμα, για μια πολιτική SSN που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:
  
- **[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 ψηφία, τα οποία μπορεί να είναι σε μορφοποιημένο ή μη μορφοποιημένο μοτίβο

- **[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις συναρτήσεις αναζητούν SSNs σε τέσσερα διαφορετικά μοτίβα:

  - Func_ssn εντοπίζει SSN με ισχυρή μορφοποίηση πριν από το 2011 που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (dd-dd-dddd ή ddd ddd ddd dddd dd dddd)

  - Func_unformatted_ssn εντοπίζει SSN με ισχυρή μορφοποίηση πριν από το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (dddddddd)

  - Func_randomized_formatted_ssn εντοπίζει ssns μετά το 2011 που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (ddd-dd-dddd ή ddd ddd ddd dddd)

  - Func_randomized_unformatted_ssn εντοπίζει ssns μετά το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (dddddddd)

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:

  - Η [συνάρτηση Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Βρέθηκε μια λέξη-κλειδί από [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Παραδείγματα λέξεων-κλειδιών περιλαμβάνουν: *Κοινωνική Ασφάλιση, Κοινωνική Ασφάλιση#, Soc Sec , SSN* . Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική DLP SSN: **SSN: 489-36-8350**
  
Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό των SSN για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα αυτού του άρθρου: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  