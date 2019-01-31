---
title: Τεχνολογία DLP κανόνα για Ασφάλισης δεν λειτουργεί
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 7242bf2b101b45fec0fe00ab33fa6db150004ee5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657359"
---
Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει έναν **Αριθμό κοινωνικής ασφάλισης (SSN)** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών στο Office 365; Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την πολιτική DLP που αναζήτηση. 
  
Για παράδειγμα, για μια πολιτική Ασφάλισης που έχει ρυθμιστεί με ένα επίπεδο εμπιστοσύνης του 85%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης:
  
- **[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ψηφία, η οποία μπορεί να βρίσκεται σε μια διαμορφωμένη ή μη διαμορφωμένη μοτίβο 
    
- **[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις λειτουργίες αναζήτηση για SSNs σε τέσσερα διαφορετικά μοτίβα: 
    
  - Func_ssn εντοπίζει SSNs με 2011 πριν από έντονη μορφοποίηση που είναι μορφοποιημένα με παύλες ή κενά διαστήματα (dddd ηη ηηη OR ηηη-ηη-dddd)
    
  - Func_unformatted_ssn εντοπίζει SSNs με 2011 πριν από έντονη μορφοποίηση που είναι μορφοποιημένο με εννέα συνεχόμενα ψηφία (ddddddddd)
    
  - Func_randomized_formatted_ssn εντοπίζει post 2011 SSNs που είναι μορφοποιημένα με παύλες ή κενά διαστήματα (dddd ηη ηηη OR ηηη-ηη-dddd)
    
  - Func_randomized_unformatted_ssn εντοπίζει post 2011 SSNs που είναι μορφοποιημένο με εννέα συνεχόμενα ψηφία (ddddddddd)
    
- **[Αθροίσματος ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Όχι, δεν υπάρχει καμία άθροισμα ελέγχου 
    
- **[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Μια πολιτική DLP είναι 85% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες: 
    
  - Η [συνάρτηση Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο. 
    
  - Μπορείτε να βρείτε μια λέξη-κλειδί από το [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Περιλαμβάνει παραδείγματα των λέξεων-κλειδιών: *κοινωνικής ασφάλισης, κοινωνική ασφάλιση #, Soc δευτ., αριθμού κοινωνικής Ασφάλισης* . Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για την πολιτική DLP Ασφάλισης: **Ασφάλισης: 489-36-8350**
    
Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για SSNs να εντοπιστεί για το περιεχόμενό σας, ανατρέξτε στην ενότητα παρακάτω σε αυτό το άρθρο: [Τι η διάκριση πεζών-κεφαλαίων τύπους πληροφοριών αναζητούν SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

