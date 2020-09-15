---
title: Συνταξιοδότηση υπηρεσιών Access Services
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
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698682"
---
# <a name="access-services-retirement"></a>Συνταξιοδότηση υπηρεσιών Access Services

Όπως ανακοινώθηκε αρχικά στο MC97576, τον Μάρτιο του 2017, και συνέχισε να επικοινωνεί κατά το παρελθόν έτος, οι υπηρεσίες πρόσβασης αποσύρονται. Η επόμενη φάση σε αυτήν τη διαδικασία θα είναι η κατάργηση των βάσεων δεδομένων Web της Access που χρησιμοποιούν λίστες του SharePoint ως υποκείμενες Αποθήκευση δεδομένων.

**Πώς αυτό με επηρεάζει;**

Ξεκινώντας από τον Ιούνιο του 2019, θα διακοπεί η δημιουργία νέων βάσεων δεδομένων της Access στο SharePoint Online και θα διακοπεί η λειτουργία της υπηρεσίας και τυχόν υπόλοιπων εφαρμογών μέχρι τον Απρίλιο του 2020.

**Τι πρέπει να κάνω για να προετοιμαστώ για αυτή την αλλαγή;**

Σας συνιστούμε να δημιουργήσετε ένα πρόγραμμα μετάβασης για τις βάσεις δεδομένων Web της εταιρείας σας στην Access. Οι διαχειριστές μπορούν να χρησιμοποιήσουν το [πρόγραμμα σάρωσης εφαρμογών του SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) για να αποκτήσουν ένα απόθεμα των εφαρμογών της Access που χρησιμοποιούν οι τοποθεσίες.

Υπάρχουν διάφοροι τρόποι για τη μετεγκατάσταση δεδομένων βάσεων δεδομένων Web της Access:

- Εισαγωγή σε μια τοπική βάση δεδομένων της Access (. ACCDB) ή σε ένα αρχείο του Excel.
- Συνιστούμε επίσης να εξερευνήσετε το Microsoft PowerApps ως εναλλακτική πλατφόρμα για να δημιουργήσετε λύσεις χωρίς κώδικα για τις επιχειρηματικές λύσεις για το Web και τις κινητές συσκευές.