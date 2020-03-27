---
title: DLP κανόνας για ηπα / UK αριθμός διαβατηρίου δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977106"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Προβλήματα με DLP - ΗΠΑ / Ηνωμένο Βασίλειο αριθμούς διαβατηρίων

**Σημαντικό:** Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες – Επισκεφθείτε [τις προσωρινές προσαρμογές δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

**DLP θέματα με τις ΗΠΑ / Ηνωμένο Βασίλειο αριθμούς διαβατηρίων**

Αντιμετωπίζετε προβλήματα με **την Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό διαβατηρίου ΗΠΑ/Ηνωμένου Βασιλείου** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών DLP στο O365; Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για αυτό που αναζητά η πολιτική DLP κατά την αξιολόγησή της.
  
Για παράδειγμα, για μια πολιτική **αριθμού διαβατηρίου ΗΠΑ/Ηνωμένου Βασιλείου** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 75%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπίζονται για να ενεργοποιηθεί ο κανόνας
  
- **[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Εννέα ψηφία

- **[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Εννέα συνεχόμενα ψηφία

- **[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου

- **[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:

  - Η συνάρτηση Func_usa_uk_passport εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.

  - Βρέθηκε μια λέξη-κλειδί από Keyword_passport.

    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική **αριθμού διαβατηρίου ΗΠΑ/Ηνωμένου Βασιλείου:** Αριθμός διαβατηρίου 123456789

Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό ενός αριθμού διαβατηρίου Η.Π.Α./ΗΒ για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για τον αριθμό διαβατηρίου Η.Π.Α./Uk](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  