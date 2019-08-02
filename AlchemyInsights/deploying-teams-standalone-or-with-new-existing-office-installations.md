---
title: Ανάπτυξη ομάδων ως αυτόνομο ή με νέες ή υπάρχουσες εγκαταστάσεις του Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054231"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Ανάπτυξη ομάδων ως αυτόνομο ή με νέες ή υπάρχουσες εγκαταστάσεις του Office

Ομάδες της Microsoft είναι τώρα συμπεριλαμβάνεται ως τμήμα των ***νέων εγκαταστάσεων*** του Office 365 ProPlus, Office 365 επαγγελματική και Office για Mac. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [όταν θα ομάδες της Microsoft ξεκινούν τη συμπερίληψη με νέες εγκαταστάσεις του Office;](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Επιπλέον, ξεκινώντας με την έκδοση 1906 του καναλιού κάθε μήνα, ομάδες θα ***προστεθούν στις υφιστάμενες εγκαταστάσεις*** του Office 365 ProPlus (και Office 365 Business) σε συσκευές που εκτελούν Windows κατά την ενημέρωση στην πιο πρόσφατη έκδοση της υπάρχουσας εγκατάστασης. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τι συμβαίνει με τις υπάρχουσες εγκαταστάσεις του Office;](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Εάν δεν θέλετε να περιμένετε για αυτό το χρονοδιάγραμμα ανάπτυξης, μπορείτε να αναπτύξετε ομάδες ως αυτόνομο για τους χρήστες σας, [ακολουθώντας αυτές τις οδηγίες](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ή μπορείτε να επιτρέψετε στους χρήστες σας να εγκαταστήσουν ομάδες οι ίδιοι από [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Εάν ο οργανισμός σας δεν είναι έτοιμοι να αναπτύξετε τις ομάδες, έχουμε τα βήματα που μπορείτε να ακολουθήσετε για να ***εξαιρέσετε ομάδες*** από [νέες](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) ή [υπάρχουσες](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) εγκαταστάσεις του Office. Εάν θέλετε οι ομάδες να εγκατασταθεί, αλλά οι δεν θέλετε ομάδες ώστε να ξεκινά αυτόματα για το χρήστη, μετά την εγκατάστασή του, ανατρέξτε στο θέμα [Αποτροπή ομάδες της Microsoft ξεκινήσει αυτόματα μετά την εγκατάσταση](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Για να ***καταργήσετε την εγκατάσταση ομάδων*** από μια συσκευή που λειτουργεί με Windows, ανατρέξτε στην ενότητα [Απεγκατάσταση ομάδες της Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Για εκκαθάριση ομάδες της Microsoft από πολλούς υπολογιστές προορισμού ή οι χρήστες, ανατρέξτε στην ενότητα [Εκκαθάριση ανάπτυξης ομάδες της Microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Αν χρησιμοποιείτε κοινόχρηστους υπολογιστές, υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ή υποδομή εικονικής επιφάνειας εργασίας (VDI), ανατρέξτε στην ενότητα [κοινή χρήση υπολογιστή και VDI περιβάλλοντα με ομάδες της Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Εάν χρησιμοποιείτε το Office για Mac, ανατρέξτε στο θέμα [εγκαταστάσεις ομάδες της Microsoft σε έναν υπολογιστή Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Μετά την εγκατάσταση ομάδων, είναι [ενημερώνεται αυτόματα](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) περίπου κάθε δύο εβδομάδες με νέες δυνατότητες και ενημερωμένες εκδόσεις ποιότητας. 