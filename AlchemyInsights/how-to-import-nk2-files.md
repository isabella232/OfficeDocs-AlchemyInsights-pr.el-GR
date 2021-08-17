---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043206"
---
# <a name="how-to-import-nk2-files"></a>Τρόπος εισαγωγής αρχείων .nk2 

Όταν ξεκινάτε το Microsoft Outlook 2013, το Outlook 2016, το Outlook 2019 ή το Outlook για Microsoft 365 για πρώτη φορά, το cache ψευδωνύμων (που είναι αποθηκευμένο στο αρχείο .nk2 του ονόματος προφίλ) εισάγεται σε ένα κρυφό μήνυμα στον προεπιλεγμένο χώρο αποθήκευσης μηνυμάτων.

Για να εισαγάγετε αρχεία .nk2 στο Outlook 2013, Outlook 2016, Outlook 2019 ή Outlook για Microsoft 365, βεβαιωθείτε ότι το αρχείο .nk2 βρίσκεται στον ακόλουθο φάκελο: %appdata%\Microsoft\Outlook

**Σημείωση:** Το αρχείο .nk2 πρέπει να έχει το ίδιο όνομα με το τρέχον Outlook 2013 ή Outlook 2016 προφίλ. Από προεπιλογή, το όνομα προφίλ είναι "Outlook". Για να ελέγξετε το όνομα του προφίλ, ακολουθήστε τα παρακάτω βήματα: 
1. Κάντε κλικ **στην επιλογή "Έναρξη"** και, στη συνέχεια, **κάντε κλικ στην επιλογή "Πίνακας Ελέγχου".**
2. Κάντε διπλό κλικ στην **επιλογή Αλληλογραφία.**
3. Στο παράθυρο διαλόγου "Ρύθμιση αλληλογραφίας", επιλέξτε **"Εμφάνιση προφίλ".**
4. Επιλέξτε **"Έναρξη**  >  **εκτέλεσης".**
5. Στο πλαίσιο **"Άνοιγμα",** πληκτρολογήστε *outlook.exe /importnk2 και,* στη συνέχεια, επιλέξτε **OK.** 

Μετά την εισαγωγή του αρχείου .nk2, τα περιεχόμενα του αρχείου συγχωνεύονται στο υπάρχον cache ψευδωνύμων που είναι αποθηκευμένο στο γραμματοκιβώτιό σας.

**Σημείωση:** Το αρχείο .nk2 μετονομάζεται με επέκταση ονόματος αρχείου .old την επόμενη φορά που θα ξεκινήσετε τις Outlook 2013, Outlook 2016, Outlook 2019 ή Outlook για Microsoft 365. Εάν θέλετε να εισαγάγετε εκ νέα το αρχείο .nk2, καταργήστε πρώτα την επέκταση ονόματος αρχείου .old.

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Εισαγωγή ή αντιγραφή της λίστας αυτόματης καταχώρησης σε άλλον υπολογιστή.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)