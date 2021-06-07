---
title: Ενεργοποίηση Teams Webinar
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793649"
---
# <a name="enable-teams-webinars"></a>Ενεργοποίηση Teams Webinar

Τα webinar είναι ενεργοποιημένα από προεπιλογή. Μπορείτε να διαχειριστείτε ποιος μπορεί να προγραμματίσει και να εγγραφεί Teams webinar χρησιμοποιώντας Teams powerShell.

- Όλοι οι χρήστες που μπορούν να δημιουργήσουν μια σύσκεψη μπορούν επίσης να δημιουργήσουν μια σύσκεψη webinar. Εάν θέλετε να διαχειριστείτε ποιος μπορεί να προγραμματίσει Teams Webinar, χρησιμοποιήστε *το AllowMeetingRegistration.* 
- Από προεπιλογή, *το WhoCanRegister είναι* ενεργοποιημένο και έχει οριστεί σε **"Όλοι".** Εάν θέλετε να απενεργοποιήσετε την καταχώρηση σύσκεψης, ορίστε *την τιμή AllowMeetingRegistration* σε **False.**

Για να αλλάξετε αυτές τις ρυθμίσεις, πρέπει να [εγκαταστήσετε Teams PowerShell.](/microsoftteams/teams-powershell-install) Επίσης, οι πολιτικές σύσκεψης επιβάλλονται σε Teams Web. Για παράδειγμα, εάν η ανώνυμη συμμετοχή είναι απενεργοποιημένη στις ρυθμίσεις σύσκεψης, οι ανώνυμοι χρήστες δεν μπορούν να συμμετάσχουν σε webinars.

Για να μάθετε περισσότερα σχετικά με τη ρύθμιση παραμέτρων για άτομα που μπορούν να εγγραφούν για webinar, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων για τα άτομα που μπορούν να [εγγραφούν για webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Για περισσότερες πληροφορίες σχετικά με τις ρυθμίσεις για τις λίστες microsoft, ανατρέξτε στο [θέμα Ρυθμίσεις ελέγχου για τις λίστες της Microsoft.](/sharepoint/control-lists)