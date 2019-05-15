---
title: Συνταξιοδότηση υπηρεσίες πρόσβασης
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973920"
---
# <a name="access-services-retirement"></a>Συνταξιοδότηση υπηρεσίες πρόσβασης

Αρχικά ανακοινώνεται στο MC97576, στο Μαρτίου 2017, και εξακολούθησε να επικοινωνούν μέσω στον τελευταίο χρόνο πρόσβαση σε υπηρεσίες είναι να αποσυρθεί από το Office 365. Η επόμενη φάση αυτής της διαδικασίας θα είναι η κατάργηση των βάσεων δεδομένων της Access Web που χρησιμοποιούν λίστες του SharePoint τους υποκείμενη αποθήκευση δεδομένων.

## <a name="how-does-this-affect-me"></a>Πώς επηρεάζει αυτό μου;

Εκκίνηση του Ιουνίου 2019, θα σταματήσει η δημιουργία νέων βάσεων δεδομένων της Access στο SharePoint Online και τερματισμός της υπηρεσίας και τις υπόλοιπες εφαρμογές ως το 2020 Απριλίου.

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>Τι πρέπει να κάνετε για να προετοιμαστείτε για αυτήν την αλλαγή;

Σας προτείνουμε να δημιουργήσετε ένα σχέδιο μετάβασης για βάσεις δεδομένων web της Access της εταιρείας σας. "Διαχειριστές" να χρησιμοποιήσετε το [σαρωτή app πρόσβασης του SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) για να αποκτήσετε έναν κατάλογο με τις εφαρμογές της Access που χρησιμοποιούν τις τοποθεσίες. 

Υπάρχουν διάφοροι τρόποι για τη μετεγκατάσταση δεδομένων του Access web βάσεις δεδομένων:

- Εισαγωγή σε μια τοπική βάση δεδομένων της Access (. ACCDB) ή σε ένα αρχείο Excel.
- Συνιστάται επίσης να Εξερεύνηση Microsoft PowerApps ως μια εναλλακτική πλατφόρμα για να δημιουργήσετε λύσεις χωρίς κώδικα επαγγελματικών για το web και φορητές συσκευές.