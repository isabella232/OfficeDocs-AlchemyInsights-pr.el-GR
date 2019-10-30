---
title: Παράκαμψη λόμπι
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768440"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Έλεγχος των ρυθμίσεων του λόμπι και του επιπέδου συμμετοχής

Αν θέλετε να επιτρέψετε σε όλους, συμπεριλαμβανομένων των εισερχόμενων κλήσεων, των εξωτερικών και των ανώνυμων χρηστών να παρακάμπτουν το λόμπι στις ομάδες της Microsoft, μπορείτε να χρησιμοποιήσετε το PowerShell για να το κάνετε. Ακολουθούν ένα παράδειγμα τροποποίησης της καθολικής σύσκεψης πολιτικής για τον οργανισμό σας:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Αυτό το cmdlet απαιτεί αυτήν τη στιγμή τη χρήση του Skype για επαγγελματική PowerShell λειτουργική μονάδα. Για να λάβετε το πρόγραμμα εγκατάστασης για να χρησιμοποιήσετε αυτό το cmdlet, ελέγξτε τη [Διαχείριση πολιτικών μέσω PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Μπορείτε να ορίσετε μια νέα πολιτική, την οποία θα πρέπει να εφαρμόσετε στους χρήστες. Εάν τροποποιήσετε την καθολική πολιτική, θα εφαρμοστεί αυτόματα στους χρήστες. Για οποιαδήποτε αλλαγή πολιτικής πρέπει να περιμένετε τουλάχιστον 4 ώρες και έως και 24 ώρες για να ισχύσουν οι πολιτικές.

Βεβαιωθείτε ότι έχετε επανεξετάσει την τεκμηρίωση παρακάτω πριν κάνετε αυτές τις αλλαγές για να καταλάβετε ακριβώς τι επιτρέπει αυτό.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Κατανόηση των ομάδων που πληρούν τους ελέγχους πολιτικής του λόμπι

- Η αυτόματη ένταξη των [ατόμων](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα συμμετέχουν σε μια σύσκεψη απευθείας ή περιμένουν στο λόμπι μέχρι να εισαχθούν από έναν εξουσιοδοτημένο χρήστη.

- [Να επιτρέψετε σε ανώνυμους χρήστες να ξεκινήσουν μια σύσκεψη](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα ανώνυμα άτομα, συμπεριλαμβανομένων των χρηστών Β2Β και ομόσπονδων, μπορούν να ενταχθούν στη σύσκεψη του χρήστη χωρίς έλεγχο ταυτότητας χρήστη από τον οργανισμό στην παρουσία.

- [Να επιτρέπεται στους χρήστες τηλεφωνικών κλήσεων να παρακάμπτουν το λόμπι](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα που κάνουν κλήση μέσω τηλεφώνου συμμετέχουν στη σύσκεψη απευθείας ή περιμένουν στο λόμπι, ανεξάρτητα από την **Αυτόματη** αποδοχή των χρηστών.

- [Να επιτρέπεται στους διοργανωτές να παρακάμπτουν τις ρυθμίσεις του λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν ο οργανωτής της σύσκεψης μπορεί να παρακάμψει τις ρυθμίσεις του λόμπι που ένας διαχειριστής έχει ορίσει να δέχεται **αυτόματα άτομα** και να **επιτρέπει τη σύνδεση μέσω τηλεφώνου τους χρήστες να παρακάμψουν το λόμπι** όταν προγραμματίσουν μια νέα σύσκεψη.

**Σημείωση:** Διαβάστε την [ενότητα Διαχείριση πολιτικών συσκέψεων στις ομάδες](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) για μια πλήρη επισκόπηση των πολιτικών συσκέψεων των ομάδων της Microsoft.
