---
title: Ρυθμίσεις πολιτικής σύσκεψης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042844"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="21bfe-102">Διαχείριση πολιτικών σύσκεψης στις ομάδες της Microsoft</span><span class="sxs-lookup"><span data-stu-id="21bfe-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="21bfe-103">**Σημείωση: μπορεί να χρειαστούν έως και 24 ώρες για να εφαρμοστούν οι αλλαγές πολιτικής για τους χρήστες.**</span><span class="sxs-lookup"><span data-stu-id="21bfe-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="21bfe-104">Ενδέχεται να μην μπορείτε να κάνετε αμέσως αλλαγές σε νέες πολιτικές που δημιουργήθηκαν. περιμένετε 4 ώρες και προσπαθήστε να τροποποιήσετε ξανά μια πολιτική που δημιουργήθηκε πρόσφατα.</span><span class="sxs-lookup"><span data-stu-id="21bfe-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="21bfe-105">Οι πολιτικές σύσκεψης χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες σε σύσκεψη για συσκέψεις που προγραμματίζονται από χρήστες στην εταιρεία σας.</span><span class="sxs-lookup"><span data-stu-id="21bfe-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="21bfe-106">Ορισμένες δυνατότητες των πολιτικών σύσκεψης μπορεί να μην υλοποιηθεί στο κέντρο διαχείρισης ομάδων ακόμα (αυτά είναι χαρακτηρισμένα "Coming σύντομα" στην τεκμηρίωση).</span><span class="sxs-lookup"><span data-stu-id="21bfe-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="21bfe-107">Σε αυτήν την περίπτωση, ή εάν λαμβάνετε ένα σφάλμα όπως "δεν είναι δυνατή η ενημέρωση της πολιτικής αυτή τη στιγμή, αλλά δοκιμάστε ξανά αργότερα" στο κέντρο διαχείρισης ομάδων της Microsoft, συνιστούμε να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε ομάδες πολιτικές σύσκεψης.</span><span class="sxs-lookup"><span data-stu-id="21bfe-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="21bfe-108">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές σύσκεψης, ανατρέξτε στους παρακάτω πόρους:</span><span class="sxs-lookup"><span data-stu-id="21bfe-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="21bfe-109">Για να μάθετε σχετικά με τη δημιουργία πολιτικών, την πραγματοποίηση αλλαγών και την εκχώρηση χρηστών στην πολιτική, ανατρέξτε [στο θέμα Διαχείριση πολιτικών σύσκεψης σε ομάδες](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="21bfe-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="21bfe-110">Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlets PowerShell, δείτε την [Επισκόπηση ομάδων PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="21bfe-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="21bfe-111">Πρέπει να χρησιμοποιήσετε το [Skype για επαγγελματική PowerShell λειτουργική μονάδα](https://www.microsoft.com/download/details.aspx?id=39366) για πολιτικές σύσκεψης ομάδων.</span><span class="sxs-lookup"><span data-stu-id="21bfe-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="21bfe-112">Εξετάστε το [\*-CsTeamsMeetingPolicy cmdlets τεκμηρίωση](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="21bfe-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

