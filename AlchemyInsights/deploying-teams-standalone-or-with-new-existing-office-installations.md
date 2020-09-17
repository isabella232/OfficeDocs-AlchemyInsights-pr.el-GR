---
title: Ανάπτυξη ομάδων ως αυτόνομων ή με νέες ή υπάρχουσες εγκαταστάσεις του Office
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806759"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Ανάπτυξη ομάδων ως αυτόνομων ή με νέες ή υπάρχουσες εγκαταστάσεις του Office

Το Microsoft teams περιλαμβάνεται πλέον ως μέρος των ***νέων εγκαταστάσεων*** των εφαρμογών Microsoft 365 για επιχειρήσεις, των εφαρμογών Microsoft 365 για επιχειρήσεις και του Office για Mac. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Πότε θα αρχίσουν να συμπεριλαμβάνονται οι Microsoft teams με νέες εγκαταστάσεις του Office;](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Επιπλέον, ξεκινώντας από την έκδοση 1906 στο τρέχον κανάλι, οι ομάδες θα ***προστεθούν στις υπάρχουσες εγκαταστάσεις*** των εφαρμογών Microsoft 365 για επιχειρήσεις (και στις εφαρμογές Microsoft 365 για επιχειρήσεις) σε συσκευές που εκτελούν Windows, όταν ενημερώνετε την υπάρχουσα εγκατάσταση στην πιο πρόσφατη έκδοση. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Τι γίνεται με τις υπάρχουσες εγκαταστάσεις του Office;](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Εάν δεν θέλετε να περιμένετε για αυτό το χρονοδιάγραμμα ανάπτυξης, μπορείτε να αναπτύξετε τις ομάδες ως μεμονωμένες για τους χρήστες σας, [ακολουθώντας αυτές τις οδηγίες](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ή μπορείτε να κάνετε τους χρήστες να εγκαταστήσουν ομάδες για τον εαυτό τους από το  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Εάν η εταιρεία σας δεν είναι έτοιμη για την ανάπτυξη ομάδων, έχουμε τα βήματα που μπορείτε να ακολουθήσετε για να ***εξαιρέσετε ομάδες*** από [νέες](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ή [υπάρχουσες](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) εγκαταστάσεις του Office. Εάν θέλετε να εγκατασταθούν οι ομάδες, αλλά δεν θέλετε οι ομάδες να ξεκινούν αυτόματα για το χρήστη μετά την εγκατάστασή του, ανατρέξτε στο θέμα [Αποτροπή της αυτόματης εκκίνησης του Microsoft teams μετά την εγκατάσταση](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Για να ***καταργήσετε την εγκατάσταση ομάδων*** από μια συσκευή που εκτελεί Windows, ανατρέξτε στο θέμα [Κατάργηση εγκατάστασης του Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Για να κάνετε εκκαθάριση του Microsoft teams από πολλούς υπολογιστές-στόχους ή χρήστες, ανατρέξτε στο [θέμα εκκαθάριση ανάπτυξης του Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Εάν χρησιμοποιείτε κοινόχρηστους υπολογιστές, υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ή υποδομή εικονικής επιφάνειας εργασίας (VDI), ανατρέξτε [στο θέμα κοινόχρηστα περιβάλλοντα υπολογιστή και VDI με το Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Εάν χρησιμοποιείτε το Office για Mac, ανατρέξτε [στο θέμα εγκαταστάσεις του Microsoft teams σε Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Μετά την εγκατάσταση των ομάδων, [ενημερώνονται αυτόματα](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) περίπου κάθε δύο εβδομάδες με νέες δυνατότητες και ενημερώσεις ποιότητας. 