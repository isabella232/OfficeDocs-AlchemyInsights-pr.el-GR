---
title: Αντιστοίχιση χαρακτηριστικού παροχής χρήστη
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949762"
---
# <a name="user-provisioning-attribute-mapping"></a>Αντιστοίχιση χαρακτηριστικού παροχής χρήστη

1. Για να αντιμετωπίσετε γνωστά προβλήματα αντιστοίχισης χαρακτηριστικών, ανατρέξτε στο θέμα [αντιστοιχίσεις χαρακτηριστικών](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Ο Microsoft Azure Active Directory (AD) παρέχει υποστήριξη για την προμήθεια χρηστών σε εφαρμογές SaaS τρίτων κατασκευαστών, όπως το Salesforce, το G Suite και άλλα. Εάν ενεργοποιήσετε την παροχή χρήστη για μια εφαρμογή SaaS άλλου κατασκευαστή, η πύλη Azure ελέγχει τις τιμές των χαρακτηριστικών του μέσω αντιστοιχίσεων χαρακτηριστικών. Για να μάθετε πώς μπορείτε να προσαρμόσετε το προεπιλεγμένο χαρακτηριστικό-αντιστοιχίσεις, ανατρέξτε στο θέμα [Προσαρμογή χαρακτηριστικού παροχής χρήστη-αντιστοιχίσεις για εφαρμογές SaaS στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Για να μάθετε περισσότερα σχετικά με την προμήθεια εφαρμογών SaaS, ανατρέξτε [στο θέμα Τι είναι η αυτοματοποιημένη προμήθεια εφαρμογών SaaS για χρήστες στο Azure AD;](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Κατά την προσαρμογή των αντιστοιχίσεων χαρακτηριστικών για την προμήθεια του χρήστη, μπορεί να διαπιστώσετε ότι το χαρακτηριστικό που θέλετε να αντιστοιχίσετε δεν εμφανίζεται στη λίστα χαρακτηριστικών προέλευσης. Ο [Συγχρονισμός ενός χαρακτηριστικού από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης στο Azure AD για προμήθεια σε ένα](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) άρθρο της εφαρμογής σάς δείχνει πώς μπορείτε να προσθέσετε το χαρακτηριστικό που λείπει, πραγματοποιώντας συγχρονισμό του από τη διαφήμισή σας εσωτερικής εγκατάστασης στο Azure AD.
