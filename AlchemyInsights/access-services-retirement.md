---
title: Απόσυρση υπηρεσιών της Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938695"
---
# <a name="access-services-retirement"></a>Απόσυρση υπηρεσιών της Access

Όπως ανακοινώσαμε αρχικά στο MC97576, τον Μάρτιο του 2017 και συνεχίσαμε να επικοινωνούμε κατά τη διάρκεια του Access Services αποσύρονται. Η επόμενη φάση αυτής της διαδικασίας θα είναι η κατάργηση βάσεων δεδομένων Web της Access που χρησιμοποιούν SharePoint λίστες ως υποκείμενο χώρο αποθήκευσης δεδομένων.

**Πώς με επηρεάζει αυτό;**

Από τον Ιούνιο του 2019, θα διακόψουμε τη δημιουργία νέων βάσεων δεδομένων της Access στο SharePoint Online και θα τερματίσουμε την υπηρεσία και τις υπόλοιπες εφαρμογές μέχρι τον Απρίλιο του 2020.

**Τι πρέπει να κάνω για να προετοιμαστώ για αυτήν την αλλαγή;**

Σας συνιστούμε να δημιουργήσετε ένα σχέδιο μετάβασης για τις βάσεις δεδομένων web της Access του οργανισμού σας. Οι διαχειριστές μπορούν να χρησιμοποιήσουν [SharePoint σαρωτή εφαρμογών της Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) για να αποκτήσουν ένα απόθεμα των εφαρμογών της Access που χρησιμοποιούν οι τοποθεσίες.

Υπάρχουν πολλοί τρόποι για τη μετεγκατάσταση δεδομένων βάσεων δεδομένων Web της Access:

- Εισαγωγή σε μια τοπική βάση δεδομένων της Access (. ACCDB) ή σε ένα Excel αρχείο.
- Συνιστάται επίσης να εξερευνήσετε Microsoft PowerApps ως εναλλακτική πλατφόρμα για να δημιουργήσετε επιχειρηματικές λύσεις χωρίς κώδικα για το web και κινητές συσκευές.