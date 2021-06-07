---
title: Διαχείριση καταχώρησης webinar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793707"
---
# <a name="manage-webinar-registration"></a>Διαχείριση καταχώρησης webinar

Διαχειρίζεστε τα άτομα που μπορούν να εγγραφούν Teams Webinars χρησιμοποιώντας Teams εντολές του Powershell. Για να εγκαταστήσετε Teams Powershell, ανατρέξτε [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Από προεπιλογή, *το WhoCanRegister είναι* ενεργοποιημένο και ορίζεται σε **EveryoneInCompany.** Για να επιτρέψετε σε οποιονδήποτε, συμπεριλαμβανομένων των ανώνυμων χρηστών, να καταχωρήσει την πολιτική σύσκεψης **σε "Όλοι",** χρησιμοποιώντας την εντολή Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Σημείωση:** Εάν η ανώνυμη συμμετοχή είναι απενεργοποιημένη στις ρυθμίσεις σύσκεψης, οι ανώνυμοι χρήστες δεν μπορούν να συμμετάσχουν σε webinars. Για να μάθετε περισσότερα και να ενεργοποιήσετε αυτήν τη ρύθμιση, [ανατρέξτε στο θέμα Διαχείριση ρυθμίσεων σύσκεψης Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Εάν θέλετε να απενεργοποιήσετε την καταχώρηση σύσκεψης, ορίστε *την τιμή AllowMeetingRegistration* σε **False.**

Για να μάθετε περισσότερα σχετικά με τη ρύθμιση παραμέτρων για άτομα που μπορούν να εγγραφούν για webinar, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων για τα άτομα που μπορούν να [εγγραφούν για webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Για περισσότερες πληροφορίες σχετικά με τις ρυθμίσεις για τις λίστες microsoft, ανατρέξτε στο [θέμα Ρυθμίσεις ελέγχου για τις λίστες της Microsoft.](/sharepoint/control-lists)
