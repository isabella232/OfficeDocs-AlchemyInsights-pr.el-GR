---
title: Επιτρέψτε σε ένα χρήστη να συγχρονίσει έναν προσωπικό λογαριασμό με τον λογαριασμό εργασίας στο Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813395"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Επιτρέψτε σε ένα χρήστη να συγχρονίσει έναν προσωπικό λογαριασμό με τον λογαριασμό εργασίας στο Microsoft Edge

Βεβαιωθείτε ότι πληροίτε αυτά τα κριτήρια:

- Η εταιρική περιαγωγή κατάστασης είναι ενεργοποιημένη στο κέντρο Azure Active Directory, το οποίο απαιτεί μια συνδρομή σε Azure Active Directory Premium ή Φορητότητα για μεγάλες επιχειρήσεις + Ασφάλεια (EMS). Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Ενεργοποίηση περιαγωγής εταιρικού Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Πληρούνται ένα ή και τα δύο από τα ακόλουθα κριτήρια:
    - Η υπηρεσία Προστασίας πληροφοριών Azure είναι ενεργοποιημένη για το μισθωτή σας. Για λεπτομέρειες, ανατρέξτε [στο θέμα Ενεργοποίηση προστασίας διαχείρισης δικαιωμάτων Azure από το Κέντρο διαχείρισης Microsoft 365.](/azure/information-protection/activate-office365)
    - Η Azure Active Directory εταιρικής κατάστασης περιαγωγής (ESR) είναι ενεργοποιημένη για οποιονδήποτε χρήστη ή μισθωτή. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Τι είναι η περιαγωγή εταιρικής κατάστασης;](/azure/active-directory/devices/enterprise-state-roaming-overview).

Εάν το AIP και το ESR είναι και τα δύο απενεργοποιημένα, ένα μήνυμα σφάλματος ενημερώνει τους χρήστες ότι ο συγχρονισμός δεν είναι διαθέσιμος για τους λογαριασμούς τους.
