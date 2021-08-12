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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925165"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Διαχείριση πολιτικών σύσκεψης Microsoft Teams

**Σημείωση: Μπορεί να διαρκέσει έως και 24 ώρες για να εφαρμοστούν οι αλλαγές πολιτικής για τους χρήστες.** Ενδέχεται να μην μπορείτε να κάνετε αμέσως αλλαγές στις πολιτικές που μόλις δημιουργήσατε. περιμένετε 4 ώρες και προσπαθήστε να τροποποιήσετε ξανά μια πολιτική που μόλις δημιουργήσατε.

Οι πολιτικές σύσκεψης χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες στη σύσκεψη για συσκέψεις που έχουν προγραμματιστεί από τους χρήστες στον οργανισμό σας. Ορισμένες δυνατότητες των πολιτικών σύσκεψης ενδέχεται να μην εφαρμοστούν ακόμη στο κέντρο διαχείρισης Teams (αυτές επισημαίνονται ως "σύντομα σύντομα" στην τεκμηρίωση). Σε αυτή την περίπτωση ή εάν εμφανίζεται ένα σφάλμα όπως "Δεν μπορούμε να ενημερώσουμε την πολιτική αυτήν τη στιγμή, αλλά να την δοκιμάσουμε ξανά αργότερα" στο κέντρο διαχείρισης του Microsoft Teams, συνιστάται να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε πολιτικές Teams σύσκεψης. 

Για περισσότερες πληροφορίες σχετικά με τις πολιτικές σύσκεψης, ανατρέξτε στους ακόλουθους πόρους:

- Για να μάθετε περισσότερα σχετικά με τη δημιουργία πολιτικών, την πραγματοποίηση αλλαγών και την εκχώρηση χρηστών στην πολιτική, ανατρέξτε στο θέμα Διαχείριση [πολιτικών σύσκεψης Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlet του PowerShell, ανατρέξτε [στο θέμα Teams Επισκόπηση του PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Πρέπει να χρησιμοποιήσετε τη λειτουργική [μονάδα Skype για επιχειρήσεις PowerShell για](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams συσκέψεων. 
    - Ανατρέξτε [στην τεκμηρίωση cmdlets *-CsTeamsMeetingPolicy για](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) περισσότερες πληροφορίες.

