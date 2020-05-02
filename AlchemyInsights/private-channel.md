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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="bbb2b-102">Ιδιωτικά κανάλια στις ομάδες της Microsoft</span><span class="sxs-lookup"><span data-stu-id="bbb2b-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="bbb2b-103">Τα ιδιωτικά κανάλια είναι μια νέα δυνατότητα στο Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bbb2b-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="bbb2b-104">Σημειώστε ότι τα ιδιωτικά κανάλια δεν μπορούν να μετατραπούν από τυπικά κανάλια ή αντίστροφα.</span><span class="sxs-lookup"><span data-stu-id="bbb2b-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="bbb2b-105">Για λεπτομέρειες σχετικά με τα ιδιωτικά κανάλια, όπως πληροφορίες σχετικά με [τη δημιουργία ιδιωτικών καναλιών και την ιδιότητα μέλους](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) και [τοποθεσίες του Ιδιωτικού καναλιού sharepoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), ανατρέξτε στο θέμα [Ιδιωτικά κανάλια στο Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="bbb2b-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="bbb2b-106">**Σημείωση:** Επειδή οι παράμετροι για τη διατήρηση μηνυμάτων ιδιωτικού καναλιού δεν υποστηρίζονται ακόμα, οι μισθωτές με ενεργοποιημένες τις πολιτικές διατήρησης δεν θα έχουν ενεργοποιημένο τα ιδιωτικά κανάλια από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="bbb2b-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="bbb2b-107">Τα ιδιωτικά κανάλια μπορούν να ενεργοποιηθούν στο κέντρο διαχείρισης ομάδων.</span><span class="sxs-lookup"><span data-stu-id="bbb2b-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="bbb2b-108">Επίσης, σημειώστε ότι ενώ δεν υποστηρίζεται η διατήρηση μηνυμάτων ιδιωτικού καναλιού, υποστηρίζεται η διατήρηση αρχείων που είναι κοινόχρηστα σε ιδιωτικά κανάλια.</span><span class="sxs-lookup"><span data-stu-id="bbb2b-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="bbb2b-109">**Χρειάζεστε νέο ιδιοκτήτη ομάδας;**</span><span class="sxs-lookup"><span data-stu-id="bbb2b-109">**Need a new team owner?**</span></span>

<span data-ttu-id="bbb2b-110">Αν ο κάτοχος του ιδιωτικού καναλιού σας φύγει, μπορείτε να προσθέσετε έναν νέο κάτοχο ομάδας μέσω του Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="bbb2b-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="bbb2b-111">Μεταβείτε [εδώ](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) για να εγκαταστήσετε το Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="bbb2b-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="bbb2b-112">Εδώ είναι το cmdlet που θα χρειαστείτε:</span><span class="sxs-lookup"><span data-stu-id="bbb2b-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="bbb2b-113">Για περισσότερες πληροφορίες σχετικά με τις ομάδες Powershell, ανατρέξτε στο θέμα [Επισκόπηση PowerShell ομάδων](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="bbb2b-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
