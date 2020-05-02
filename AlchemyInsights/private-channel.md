---
title: Ιδιωτικό κανάλι
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005438"
---
# <a name="private-channels-in-microsoft-teams"></a>Ιδιωτικά κανάλια στις ομάδες της Microsoft

Τα ιδιωτικά κανάλια είναι μια νέα δυνατότητα στο Microsoft Teams. Σημειώστε ότι τα ιδιωτικά κανάλια δεν μπορούν να μετατραπούν από τυπικά κανάλια ή αντίστροφα.

Για λεπτομέρειες σχετικά με τα ιδιωτικά κανάλια, όπως πληροφορίες σχετικά με [τη δημιουργία ιδιωτικών καναλιών και την ιδιότητα μέλους](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) και [τοποθεσίες του Ιδιωτικού καναλιού sharepoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), ανατρέξτε στο θέμα [Ιδιωτικά κανάλια στο Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Σημείωση:** Επειδή οι παράμετροι για τη διατήρηση μηνυμάτων ιδιωτικού καναλιού δεν υποστηρίζονται ακόμα, οι μισθωτές με ενεργοποιημένες τις πολιτικές διατήρησης δεν θα έχουν ενεργοποιημένο τα ιδιωτικά κανάλια από προεπιλογή. Τα ιδιωτικά κανάλια μπορούν να ενεργοποιηθούν στο κέντρο διαχείρισης ομάδων. Επίσης, σημειώστε ότι ενώ δεν υποστηρίζεται η διατήρηση μηνυμάτων ιδιωτικού καναλιού, υποστηρίζεται η διατήρηση αρχείων που είναι κοινόχρηστα σε ιδιωτικά κανάλια.

**Χρειάζεστε νέο ιδιοκτήτη ομάδας;**

Αν ο κάτοχος του ιδιωτικού καναλιού σας φύγει, μπορείτε να προσθέσετε έναν νέο κάτοχο ομάδας μέσω του Teams Powershell.


- Μεταβείτε [εδώ](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) για να εγκαταστήσετε το Teams Powershell.

Εδώ είναι το cmdlet που θα χρειαστείτε:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Για περισσότερες πληροφορίες σχετικά με τις ομάδες Powershell, ανατρέξτε στο θέμα [Επισκόπηση PowerShell ομάδων](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
