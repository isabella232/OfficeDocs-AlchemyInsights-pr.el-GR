---
title: Ανάπτυξη ομάδων ως αυτόνομων ή με νέες ή υπάρχουσες εγκαταστάσεις του Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617895"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Ανάπτυξη ομάδων ως αυτόνομων ή με νέες ή υπάρχουσες εγκαταστάσεις του Office

Το Microsoft Teams περιλαμβάνεται πλέον ως μέρος των ***νέων εγκαταστάσεων*** των Εφαρμογών Microsoft 365 για επιχειρήσεις, των Εφαρμογών Microsoft 365 για επιχειρήσεις και του Office για Mac. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Πότε θα αρχίσουν να περιλαμβάνονται οι ομάδες της Microsoft με νέες εγκαταστάσεις του Office;](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Επιπλέον, ξεκινώντας με την έκδοση 1906 στο τρέχον κανάλι , οι ομάδες θα ***προστεθούν στις υπάρχουσες εγκαταστάσεις*** των εφαρμογών της Microsoft 365 για μεγάλες επιχειρήσεις (και εφαρμογές της Microsoft 365 για επιχειρήσεις) σε συσκευές που εκτελούν Windows όταν ενημερώνετε την υπάρχουσα εγκατάσταση στην πιο πρόσφατη έκδοση. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τι γίνεται με τις υπάρχουσες εγκαταστάσεις του Office;](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Εάν δεν θέλετε να περιμένετε αυτό το χρονοδιάγραμμα ανάπτυξης, μπορείτε να αναπτύξετε το Teams ως αυτόνομο για τους [χρήστες σας, ακολουθώντας αυτές τις οδηγίες](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ή μπορείτε να ζητήσετε από τους χρήστες σας να εγκαταστήσουν το Teams για τον εαυτό τους από  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) το .

Εάν ο οργανισμός σας δεν είναι έτοιμος να αναπτύξει ομάδες, έχουμε τα βήματα που μπορείτε να λάβετε για να ***εξαιρέσετε τις ομάδες*** από [νέες](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ή [υπάρχουσες](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) εγκαταστάσεις του Office. Εάν θέλετε να εγκατασταθούν οι ομάδες, αλλά δεν θέλετε οι ομάδες να ξεκινούν αυτόματα για το χρήστη μετά την εγκατάστασή του, ανατρέξτε στο θέμα [Αποτροπή αυτόματης εκκίνησης των ομάδων της Microsoft μετά την εγκατάσταση](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Για να ***καταργήσετε την εγκατάσταση των ομάδων*** από μια συσκευή που εκτελεί Windows, ανατρέξτε στο θέμα [Κατάργηση εγκατάστασης των ομάδων της Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Για να εκκαθαρίσετε τις ομάδες της Microsoft από πολλούς υπολογιστές ή χρήστες προορισμού, ανατρέξτε στο θέμα [Εκκαθάριση ανάπτυξης του Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Εάν χρησιμοποιείτε κοινόχρηστους υπολογιστές, υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ή υποδομή εικονικής επιφάνειας εργασίας (VDI), ανατρέξτε στο θέμα [Κοινόχρηστα περιβάλλοντα υπολογιστή και VDI με το Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Εάν χρησιμοποιείτε το Office για Mac, ανατρέξτε στο θέμα [Εγκαταστάσεις του Microsoft Teams σε Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Μετά την εγκατάσταση του Teams, [ενημερώνεται αυτόματα](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) περίπου κάθε δύο εβδομάδες με νέες δυνατότητες και ενημερώσεις ποιότητας. 