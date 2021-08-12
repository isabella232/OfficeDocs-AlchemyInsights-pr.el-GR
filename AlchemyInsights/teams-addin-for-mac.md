---
title: Teams πρόσθετο για Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940675"
---
# <a name="teams-add-in-for-mac"></a>Teams πρόσθετο για Mac

Για να αντιμετωπίσετε ένα πρόσθετο Teams που λείπει για τους χρήστες λειτουργικού συστήματος Mac, ακολουθήστε τα παρακάτω βήματα:

**Βήμα 1:** Εάν έχετε υβριδική έκδοση Exchange εσωτερικής εγκατάστασης (απαιτείται CU3 2016 ή νεότερη έκδοση), χρησιμοποιήστε το εργαλείο Test-HMA.ps1 για να επιβεβαιώσετε ότι οι παράμετροι του υβριδικού σύγχρονου ελέγχου ταυτότητας έχουν ρυθμιστεί σωστά. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Επικύρωση ρύθμισης υβριδικού σύγχρονου ελέγχου ταυτότητας για Outlook για iOS και Android.](https://aka.ms/TestHMAEAS)  

**Σημείωση** Χρησιμοποιήστε τη μορφή διεύθυνσης UPN (για παράδειγμα, [username@contoso.com](mailto:username@contoso.com)), όχι τον τομέα\όνομα χρήστη. Κάντε το αυτό ακόμη και για τους χρήστες με Exchange Online γραμματοκιβώτια.

**Βήμα 2:** Να μεταβεί ο χρήστης στην επιλογή **"Εργαλεία**  >  **λογαριασμών"**... στο Outlook για Mac και βρείτε και επιλέξτε το λογαριασμό. Επιβεβαιώστε ότι το όνομα χρήστη που αναφέρεται είναι σε μορφή UPN (για παράδειγμα, [username@contoso.com).](mailto:username@contoso.com)

**Βήμα 3:** Επιβεβαιώστε ότι ο χρήστης διαθέτει άδεια χρήσης Microsoft Teams χρήστη. Ο χρήστης πρέπει να χρησιμοποιεί τη Office 365 για Mac, έκδοση προϊόντος 16.24 ή νεότερη.