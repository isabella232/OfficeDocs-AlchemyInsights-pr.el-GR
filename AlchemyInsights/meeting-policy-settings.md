---
title: Ρυθμίσεις πολιτικής σύσκεψης
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825443"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="4c66d-102">Διαχείριση πολιτικών σύσκεψης στο Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4c66d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="4c66d-103">**Σημείωση: Μπορεί να διαρκέσει έως και 24 ώρες για να εφαρμοστούν οι αλλαγές πολιτικής για τους χρήστες.**</span><span class="sxs-lookup"><span data-stu-id="4c66d-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="4c66d-104">Ενδέχεται να μην μπορείτε να κάνετε αμέσως αλλαγές στις πολιτικές που μόλις δημιουργήσατε. περιμένετε 4 ώρες και προσπαθήστε να τροποποιήσετε ξανά μια πολιτική που μόλις δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="4c66d-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="4c66d-105">Οι πολιτικές σύσκεψης χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες στη σύσκεψη για συσκέψεις που έχουν προγραμματιστεί από τους χρήστες στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="4c66d-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="4c66d-106">Ορισμένες δυνατότητες των πολιτικών σύσκεψης ενδέχεται να μην εφαρμόζονται ακόμη στο κέντρο διαχείρισης του Teams (αυτές επισημαίνονται ως "σύντομα σύντομα" στην τεκμηρίωση).</span><span class="sxs-lookup"><span data-stu-id="4c66d-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="4c66d-107">Σε αυτή την περίπτωση ή εάν εμφανίζεται ένα σφάλμα όπως "Δεν μπορούμε να ενημερώσουμε την πολιτική αυτήν τη στιγμή, αλλά να την δοκιμάσουμε ξανά αργότερα" στο κέντρο διαχείρισης του Microsoft Teams, συνιστάται να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε πολιτικές σύσκεψης του Teams.</span><span class="sxs-lookup"><span data-stu-id="4c66d-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="4c66d-108">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές σύσκεψης, ανατρέξτε στους ακόλουθους πόρους:</span><span class="sxs-lookup"><span data-stu-id="4c66d-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="4c66d-109">Για να μάθετε περισσότερα σχετικά με τη δημιουργία πολιτικών, την πραγματοποίηση αλλαγών και την εκχώρηση χρηστών στην πολιτική, ανατρέξτε στο θέμα [Διαχείριση πολιτικών σύσκεψης στο Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="4c66d-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="4c66d-110">Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlet του PowerShell, ανατρέξτε στο [θέμα Επισκόπηση του Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="4c66d-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="4c66d-111">Πρέπει να χρησιμοποιήσετε τη λειτουργική [μονάδα PowerShell του Skype για](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) επιχειρήσεις για τις πολιτικές σύσκεψης του Teams.</span><span class="sxs-lookup"><span data-stu-id="4c66d-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="4c66d-112">Ανατρέξτε [στην τεκμηρίωση cmdlets \*-CsTeamsMeetingPolicy για](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="4c66d-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

