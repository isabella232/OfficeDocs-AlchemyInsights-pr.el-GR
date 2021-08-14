---
title: Ο κανόνας DLP για SSN δεν λειτουργεί
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004982"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Προβλήματα DLP με αριθμούς κοινωνικής ασφάλισης

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Προβλήματα DLP με SSN**

Αντιμετωπίζετε προβλήματα με την Αποτροπή απώλειας δεδομένων **(DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει έναν αριθμό κοινωνικής **ασφάλισης (SSN)** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών στο Microsoft 365; Εάν ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την εμφάνιση της πολιτικής DLP. 
  
Για παράδειγμα, για μια πολιτική SSN που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα εξής και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:
  
- **[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 ψηφία, τα οποία μπορεί να είναι σε μορφοποιημένο ή μη μορφοποιημένο μοτίβο

- **[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις συναρτήσεις αναζητήστε SSN σε τέσσερα διαφορετικά μοτίβα:

  - Func_ssn SSN με ισχυρή μορφοποίηση πριν από το 2011 που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (ηηη-ηη-η Ή η)

  - Func_unformatted_ssn SSN με ισχυρή μορφοποίηση πριν από το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (ηηη)

  - Func_randomized_formatted_ssn τα SSN μετά το 2011 που είναι μορφοποιημένα με παύλες ή κενά διαστήματα (ηηη-ηη-η Ή η)

  - Func_randomized_unformatted_ssn τα SSN μετά το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (ηηηηη)

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Μια πολιτική DLP είναι 85% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε απόσταση 300 χαρακτήρων:

  - Η [συνάρτηση Func_ssn βρίσκει](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) περιεχόμενο που ταιριάζει με το μοτίβο.

  - A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found. Στα παραδείγματα λέξεων-κλειδιών περιλαμβάνονται τα εξής: *Social Security, Social Security#, Soc Sec ,SSN.* Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική DLP **SSN: SSN: 489-36-8350**
  
Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό SSN για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: Τι είναι οι τύποι ευαίσθητων πληροφοριών για [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: Τι θα αναζητήσουν οι [τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  