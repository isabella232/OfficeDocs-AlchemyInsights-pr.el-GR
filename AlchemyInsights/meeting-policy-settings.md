---
title: Ρυθμίσεις πολιτικής σύσκεψης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704606"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Διαχείριση πολιτικών σύσκεψης στο Microsoft Teams

**Σημείωση: Μπορεί να διαρκέσει έως και 24 ώρες για να εφαρμοστούν οι αλλαγές πολιτικής στους χρήστες.** Ενδέχεται να μην μπορείτε να κάνετε αλλαγές στις πολιτικές που μόλις δημιουργήσατε αμέσως. περιμένετε 4 ώρες και προσπαθήστε να τροποποιήσετε ξανά μια πολιτική που μόλις δημιουργήσατε.

Οι πολιτικές σύσκεψης χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες στη σύσκεψη για συσκέψεις που έχουν προγραμματιστεί από τους χρήστες στον οργανισμό σας. Ορισμένες δυνατότητες των πολιτικών σύσκεψης ενδέχεται να μην έχουν υλοποιηθεί ακόμα στο κέντρο διαχείρισης του Teams (αυτές φέρουν την ένδειξη "σύντομα σύντομα" στην τεκμηρίωση). Σε αυτή την περίπτωση ή εάν εμφανίζεται ένα μήνυμα σφάλματος όπως "Δεν μπορούμε να ενημερώσουμε την πολιτική αυτήν τη στιγμή, αλλά να την δοκιμάσουμε ξανά αργότερα" στο κέντρο διαχείρισης του Microsoft Teams, συνιστάται να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε πολιτικές σύσκεψης του Teams. 

Για περισσότερες πληροφορίες σχετικά με τις πολιτικές σύσκεψης, ανατρέξτε στους ακόλουθους πόρους:

- Για να μάθετε περισσότερα σχετικά με τη δημιουργία πολιτικών, την πραγματοποίηση αλλαγών και την εκχώρηση χρηστών στην πολιτική, ανατρέξτε στο θέμα ["Διαχείριση πολιτικών σύσκεψης στο Teams".](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlet του PowerShell, ανατρέξτε στην [Επισκόπηση του Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Πρέπει να χρησιμοποιήσετε τη λειτουργική [μονάδα Skype για επιχειρήσεις PowerShell για](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) πολιτικές σύσκεψης του Teams. 
    - Ανατρέξτε [στην τεκμηρίωση cmdlets *-CsTeamsMeetingPolicy για](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) περισσότερες πληροφορίες.

