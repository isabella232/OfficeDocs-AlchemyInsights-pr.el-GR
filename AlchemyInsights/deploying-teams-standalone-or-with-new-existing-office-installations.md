---
title: Ανάπτυξη Teams ως αυτόνομων ή με νέες ή υπάρχουσες Office εγκατάστασης
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320122"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Ανάπτυξη Teams ως αυτόνομων ή με νέες ή υπάρχουσες Office εγκατάστασης

Microsoft Teams τώρα περιλαμβάνεται ως μέρος  των νέων εγκαταστάσεων Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις, Εφαρμογές Microsoft 365 για επιχειρήσεις και Office για Mac. Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα Microsoft Teams θα αρχίσετε να συμπεριλαμβάνεταιτε στις νέες εγκαταστάσεις Office;](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Επιπλέον, ξεκινώντας με την Έκδοση 1906 στο κανάλι  τρεχουσών ενημερώσεων, το Teams θα προστεθεί σε υπάρχουσες εγκαταστάσεις του Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις (και του Εφαρμογές Microsoft 365 για επιχειρήσεις) σε συσκευές που εκτελούν το Windows όταν ενημερώνετε την υπάρχουσα εγκατάσταση στην πιο πρόσφατη έκδοση. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Τι γίνεται με τις υπάρχουσες εγκαταστάσεις Office;](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Σημείωση:** Εάν δεν θέλετε να περιμένετε για αυτό το χρονοδιάγραμμα ανάπτυξης, μπορείτε να αναπτύξετε το Teams ως αυτόνομο για τους χρήστες σας, ακολουθώντας αυτές τις οδηγίες ή μπορείτε να κάνετε τους χρήστες σας να εγκαταστήσουν το Teams για τους ίδιους από το [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Εάν η εταιρεία σας δεν είναι έτοιμη για Teams, έχουμε τα βήματα που [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) μπορείτε [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) να κάνετε για ***να αποκλείσετε Teams από*** νέες ή υπάρχουσες εγκαταστάσεις Office. Εάν θέλετε Teams εγκατασταθεί, αλλά δεν θέλετε το Teams να ξεκινά αυτόματα για το χρήστη μετά την εγκατάστασή του, ανατρέξτε στο θέμα Αποτροπή της αυτόματης εκκίνησης του Microsoft Teams μετά [την εγκατάσταση.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Για να ***καταργήσετε Teams από*** μια συσκευή που εκτελεί Windows, ανατρέξτε στο θέμα [Κατάργηση Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Για να κάνετε εκκαθάριση Microsoft Teams από πολλούς υπολογιστές προορισμού ή χρήστες, ανατρέξτε [στο θέμα Microsoft Teams εκκαθάρισης ανάπτυξης.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Εάν χρησιμοποιείτε κοινόχρηστους υπολογιστές, υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ή υποδομή εικονικής επιφάνειας εργασίας (VDI), ανατρέξτε στο θέμα Κοινόχρηστα περιβάλλοντα υπολογιστή και [VDI με Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Εάν χρησιμοποιείτε το Office για Mac, [ανατρέξτε Microsoft Teams εγκαταστάσεις σε Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Σημείωση:** Αφού Teams, ενημερώνεται αυτόματα [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) περίπου κάθε δύο εβδομάδες με νέες δυνατότητες και ενημερώσεις ποιότητας. 