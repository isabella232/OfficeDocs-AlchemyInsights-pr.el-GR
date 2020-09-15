---
title: Ο κανόνας DLP για το SSN δεν λειτουργεί
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679369"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Θέματα DLP με αριθμούς κοινωνικής ασφάλισης

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**Θέματα DLP με το SSNs**

Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για το περιεχόμενο που περιέχει έναν **αριθμό ΚΟΙΝΩΝΙΚΉς ασφάλισης (SSN)** κατά τη χρήση ενός ευαίσθητου τύπου πληροφοριών στο Microsoft 365; Εάν Ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαιτούμενες πληροφορίες για το τι αναζητά η πολιτική DLP. 
  
Για παράδειγμα, για μια πολιτική SSN που έχει ρυθμιστεί με επίπεδο αξιοπιστίας 85%, τα παρακάτω αξιολογούνται και πρέπει να ανιχνευθούν για να ενεργοποιείται ο κανόνας:
  
- **[Μορφοποίηση:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 ψηφία, τα οποία μπορεί να βρίσκονται σε μορφοποιημένο ή μη μορφοποιημένο μοτίβο

- **[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις συναρτήσεις αναζητήστε το SSNs σε τέσσερα διαφορετικά μοτίβα:

  - Func_ssn εντοπίζει το SSNs με ισχυρή μορφοποίηση pre-2011 που είναι μορφοποιημένη με παύλες ή κενά διαστήματα (DDD-DD-ηηηη ή DDD DD ηηηη)

  - Func_unformatted_ssn εντοπίζει το SSNs με την προ-2011 ισχυρή μορφοποίηση που δεν έχει μορφοποιηθεί ως εννέα διαδοχικά ψηφία (ddddddddd)

  - Func_randomized_formatted_ssn εντοπίζει την καταχώρηση-2011 SSNs που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (DDD-DD-ηηηη ή DDD DD ηηηη)

  - Func_randomized_unformatted_ssn εντοπίζει τη δημοσίευση-2011 SSNs που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (ddddddddd)

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, μέσα σε μια εγγύτητα των 300 χαρακτήρων:

  - Η [συνάρτηση Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Βρέθηκε μια λέξη-κλειδί από [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Παραδείγματα λέξεων-κλειδιών περιλαμβάνουν:  *κοινωνική ασφάλιση, κοινωνική ασφάλιση #, SOC SEC, SSN*  . Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει την πολιτική DLP SSN: **SSN: 489-36-8350**
  
Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για την ανίχνευση του SSNs για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για το SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Με τη χρήση διαφορετικού ενσωματωμένου τύπου ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  