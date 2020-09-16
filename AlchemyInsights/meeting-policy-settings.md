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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794334"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Διαχείριση πολιτικών συσκέψεων στο Microsoft teams

**Σημείωση: μπορεί να χρειαστούν έως και 24 ώρες για να εφαρμοστούν οι αλλαγές πολιτικής για τους χρήστες.** Ενδέχεται να μην μπορείτε να κάνετε αμέσως αλλαγές σε νέες πολιτικές που έχουν δημιουργηθεί. περιμένετε 4 ώρες και προσπαθήστε να τροποποιήσετε ξανά μια πολιτική που μόλις δημιουργήσατε.

Οι πολιτικές συσκέψεων χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες της σύσκεψης για συσκέψεις που έχουν προγραμματιστεί από τους χρήστες στην εταιρεία σας. Ορισμένες δυνατότητες των πολιτικών συσκέψεων ενδέχεται να μην υλοποιούνται στο κέντρο διαχείρισης ομάδων ακόμη (αυτά είναι χαρακτηρισμένα ως "σύντομα διαθέσιμα" στην τεκμηρίωση). Σε αυτή την περίπτωση, ή εάν εμφανίζεται ένα σφάλμα όπως "δεν είναι δυνατή η ενημέρωση της πολιτικής αυτή τη στιγμή, αλλά δοκιμάστε ξανά αργότερα" στο κέντρο διαχείρισης του Microsoft teams, συνιστάται να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε πολιτικές συσκέψεων ομάδων. 

Για περισσότερες πληροφορίες σχετικά με τις πολιτικές συσκέψεων, ανατρέξτε στους ακόλουθους πόρους:

- Για να μάθετε πώς να δημιουργείτε πολιτικές, να κάνετε αλλαγές και να εκχωρείτε χρήστες στην πολιτική, ανατρέξτε [στο θέμα Διαχείριση πολιτικών συσκέψεων στο teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlet PowerShell, ανατρέξτε στην [Επισκόπηση teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Πρέπει να χρησιμοποιήσετε τη [λειτουργική μονάδα του Skype για Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) για τις πολιτικές συσκέψεων των ομάδων. 
    - Εξετάστε την [τεκμηρίωση για τα cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) για περισσότερες πληροφορίες.

