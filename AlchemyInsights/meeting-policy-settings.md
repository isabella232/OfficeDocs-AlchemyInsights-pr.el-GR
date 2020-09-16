---
title: Ρυθμίσεις πολιτικής σύσκεψης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794334"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="b2c5d-102">Διαχείριση πολιτικών συσκέψεων στο Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="b2c5d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="b2c5d-103">**Σημείωση: μπορεί να χρειαστούν έως και 24 ώρες για να εφαρμοστούν οι αλλαγές πολιτικής για τους χρήστες.**</span><span class="sxs-lookup"><span data-stu-id="b2c5d-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="b2c5d-104">Ενδέχεται να μην μπορείτε να κάνετε αμέσως αλλαγές σε νέες πολιτικές που έχουν δημιουργηθεί. περιμένετε 4 ώρες και προσπαθήστε να τροποποιήσετε ξανά μια πολιτική που μόλις δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="b2c5d-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="b2c5d-105">Οι πολιτικές συσκέψεων χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες της σύσκεψης για συσκέψεις που έχουν προγραμματιστεί από τους χρήστες στην εταιρεία σας.</span><span class="sxs-lookup"><span data-stu-id="b2c5d-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="b2c5d-106">Ορισμένες δυνατότητες των πολιτικών συσκέψεων ενδέχεται να μην υλοποιούνται στο κέντρο διαχείρισης ομάδων ακόμη (αυτά είναι χαρακτηρισμένα ως "σύντομα διαθέσιμα" στην τεκμηρίωση).</span><span class="sxs-lookup"><span data-stu-id="b2c5d-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="b2c5d-107">Σε αυτή την περίπτωση, ή εάν εμφανίζεται ένα σφάλμα όπως "δεν είναι δυνατή η ενημέρωση της πολιτικής αυτή τη στιγμή, αλλά δοκιμάστε ξανά αργότερα" στο κέντρο διαχείρισης του Microsoft teams, συνιστάται να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε πολιτικές συσκέψεων ομάδων.</span><span class="sxs-lookup"><span data-stu-id="b2c5d-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="b2c5d-108">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές συσκέψεων, ανατρέξτε στους ακόλουθους πόρους:</span><span class="sxs-lookup"><span data-stu-id="b2c5d-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="b2c5d-109">Για να μάθετε πώς να δημιουργείτε πολιτικές, να κάνετε αλλαγές και να εκχωρείτε χρήστες στην πολιτική, ανατρέξτε [στο θέμα Διαχείριση πολιτικών συσκέψεων στο teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="b2c5d-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="b2c5d-110">Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlet PowerShell, ανατρέξτε στην [Επισκόπηση teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="b2c5d-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="b2c5d-111">Πρέπει να χρησιμοποιήσετε τη [λειτουργική μονάδα του Skype για Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) για τις πολιτικές συσκέψεων των ομάδων.</span><span class="sxs-lookup"><span data-stu-id="b2c5d-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="b2c5d-112">Εξετάστε την [τεκμηρίωση για τα cmdlets \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="b2c5d-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

