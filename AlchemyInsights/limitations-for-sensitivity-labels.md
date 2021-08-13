---
title: Περιορισμοί για ετικέτες ευαισθησίας για Office αρχείων σε SharePoint και OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813155"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Περιορισμοί για ετικέτες ευαισθησίας για Office αρχείων σε SharePoint και OneDrive

Κατά την ενεργοποίηση ετικετών ευαισθησίας για Office αρχείων σε SharePoint και OneDrive, πρέπει να γνωρίζετε τις απαιτήσεις και τους περιορισμούς, οι οποίοι περιλαμβάνουν:

- SharePoint και OneDrive δεν μπορούν να επεξεργαστούν ορισμένα αρχεία με ετικέτα και κρυπτογράφηση από εφαρμογές υπολογιστή του Office όταν τα αρχεία περιέχουν δεδομένα PowerQuery, δεδομένα που είναι αποθηκευμένα από προσαρμοσμένα πρόσθετα ή προσαρμοσμένα τμήματα XML.
- SharePoint και OneDrive δεν εφαρμόζουν ετικέτες ευαισθησίας αυτόματα σε υπάρχοντα αρχεία που έχετε ήδη κρυπτογραφήσει χρησιμοποιώντας ετικέτες Προστασίας πληροφοριών Azure (AIP). Για να εφαρμόσετε ετικέτες ευαισθησίας σε κρυπτογραφημένα αρχεία: 
    - Βεβαιωθείτε ότι οι ετικέτες AIP έχουν μετεγκατασταθεί και δημοσιευτεί στο Microsoft 365 Συμμόρφωσης.
    - Κάντε λήψη των αρχείων με ετικέτα και, στη συνέχεια, αποστείλετε τα στην αρχική SharePoint ή OneDrive τους.
- Για κρυπτογραφημένα έγγραφα, η εκτύπωση δεν υποστηρίζεται.

Για πρόσθετες λεπτομέρειες σχετικά με τους περιορισμούς, ανατρέξτε στο θέμα Ενεργοποίηση ετικετών [ευαισθησίας για Office αρχείων SharePoint και OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
