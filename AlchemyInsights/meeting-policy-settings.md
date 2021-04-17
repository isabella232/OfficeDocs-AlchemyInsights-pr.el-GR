---
title: Ρυθμίσεις πολιτικής σύσκεψης
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825443"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Διαχείριση πολιτικών σύσκεψης στο Microsoft Teams

**Σημείωση: Μπορεί να διαρκέσει έως και 24 ώρες για να εφαρμοστούν οι αλλαγές πολιτικής για τους χρήστες.** Ενδέχεται να μην μπορείτε να κάνετε αμέσως αλλαγές στις πολιτικές που μόλις δημιουργήσατε. περιμένετε 4 ώρες και προσπαθήστε να τροποποιήσετε ξανά μια πολιτική που μόλις δημιουργήσατε.

Οι πολιτικές σύσκεψης χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες στη σύσκεψη για συσκέψεις που έχουν προγραμματιστεί από τους χρήστες στον οργανισμό σας. Ορισμένες δυνατότητες των πολιτικών σύσκεψης ενδέχεται να μην εφαρμόζονται ακόμη στο κέντρο διαχείρισης του Teams (αυτές επισημαίνονται ως "σύντομα σύντομα" στην τεκμηρίωση). Σε αυτή την περίπτωση ή εάν εμφανίζεται ένα σφάλμα όπως "Δεν μπορούμε να ενημερώσουμε την πολιτική αυτήν τη στιγμή, αλλά να την δοκιμάσουμε ξανά αργότερα" στο κέντρο διαχείρισης του Microsoft Teams, συνιστάται να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε πολιτικές σύσκεψης του Teams. 

Για περισσότερες πληροφορίες σχετικά με τις πολιτικές σύσκεψης, ανατρέξτε στους ακόλουθους πόρους:

- Για να μάθετε περισσότερα σχετικά με τη δημιουργία πολιτικών, την πραγματοποίηση αλλαγών και την εκχώρηση χρηστών στην πολιτική, ανατρέξτε στο θέμα [Διαχείριση πολιτικών σύσκεψης στο Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlet του PowerShell, ανατρέξτε στο [θέμα Επισκόπηση του Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Πρέπει να χρησιμοποιήσετε τη λειτουργική [μονάδα PowerShell του Skype για](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) επιχειρήσεις για τις πολιτικές σύσκεψης του Teams. 
    - Ανατρέξτε [στην τεκμηρίωση cmdlets *-CsTeamsMeetingPolicy για](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) περισσότερες πληροφορίες.

