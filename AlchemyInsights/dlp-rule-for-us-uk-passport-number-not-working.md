---
title: Τεχνολογία DLP κανόνα για ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου δεν λειτουργεί
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656423"
---
Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει ένα **ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου** κατά τη χρήση ενός τύπου ευαίσθητες πληροφορίες DLP σε O365; Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για το τι είναι αναζητούν την πολιτική DLP όταν που αξιολογείται. 
  
Για παράδειγμα, για μια **ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου** πολιτική είναι ρυθμισμένη με επίπεδο εμπιστοσύνης του 75%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης 
  
- **[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Εννέα ψηφία 
    
- **[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Εννέα ψηφία διαδοχικά 
    
- **[Αθροίσματος ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Όχι, δεν υπάρχει καμία άθροισμα ελέγχου 
    
- **[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Μια πολιτική DLP είναι 75% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες: 
    
  - Η συνάρτηση Func_usa_uk_passport εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο.
    
  - Μπορείτε να βρείτε μια λέξη-κλειδί από το Keyword_passport.
    
    Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για την **των η.π.α. / αριθμός διαβατηρίου UK** πολιτικής: αριθμός διαβατηρίου ΗΠΑ 123456789 
    
Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για ένα ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου που θα εντοπιστούν για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι οι ευαίσθητες πληροφορίες τύπους αναζητήστε η.π.α. / αριθμός διαβατηρίου Ηνωμένο Βασίλειο](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

