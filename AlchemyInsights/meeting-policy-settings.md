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
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627574"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ffed9-102">Διαχείριση πολιτικών συσκέψεων σε ομάδες της Microsoft</span><span class="sxs-lookup"><span data-stu-id="ffed9-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ffed9-103">Οι πολιτικές συσκέψεων χρησιμοποιούνται για τον έλεγχο των δυνατοτήτων που είναι διαθέσιμες στους συμμετέχοντες στην σύσκεψη για συσκέψεις που έχουν προγραμματιστεί από τους χρήστες στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="ffed9-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ffed9-104">Ορισμένες δυνατότητες των πολιτικών συσκέψεων ενδέχεται να μην υλοποιούνται στο κέντρο διαχείρισης ομάδων ακόμα (αυτές επισημαίνονται ως "προσεχώς" στην τεκμηρίωση).</span><span class="sxs-lookup"><span data-stu-id="ffed9-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ffed9-105">Σε αυτήν την περίπτωση, ή αν λαμβάνετε ένα σφάλμα όπως "δεν μπορούμε να ενημερώσουμε την πολιτική τώρα, αλλά προσπαθήστε ξανά αργότερα" στο κέντρο διαχείρισης ομάδων της Microsoft, συνιστούμε να χρησιμοποιήσετε το PowerShell για να δημιουργήσετε ή να τροποποιήσετε πολιτικές συσκέψεων ομάδων.</span><span class="sxs-lookup"><span data-stu-id="ffed9-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ffed9-106">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές συσκέψεων, ανατρέξτε στους ακόλουθους πόρους:</span><span class="sxs-lookup"><span data-stu-id="ffed9-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ffed9-107">Για να μάθετε σχετικά με τη δημιουργία πολιτικών, την πραγματοποίηση αλλαγών και την εκχώρηση χρηστών στην πολιτική, ανατρέξτε [στο θέμα Διαχείριση πολιτικών συσκέψεων σε ομάδες](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ffed9-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ffed9-108">Για να κάνετε αλλαγές πολιτικής χρησιμοποιώντας cmdlet PowerShell, ανατρέξτε στο [ενότητα Επισκόπηση PowerShell ομάδων](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ffed9-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ffed9-109">Πρέπει να χρησιμοποιήσετε το [Skype για επιχειρηματική λειτουργική μονάδα PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) για ομάδες συσκέψεων πολιτικές.</span><span class="sxs-lookup"><span data-stu-id="ffed9-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ffed9-110">Για περισσότερες πληροφορίες, εξετάστε την [τεκμηρίωση της \*-csteamsmeetingpolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="ffed9-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="ffed9-111">**Σημείωση:** Μπορεί να χρειαστούν έως και 24 ώρες για να τεθούν σε ισχύ οι αλλαγές πολιτικής για τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="ffed9-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="ffed9-112">Ενδέχεται να μην μπορείτε να κάνετε αλλαγές αμέσως στις πολιτικές που δημιουργήθηκαν πρόσφατα. περιμένετε 4 ώρες και προσπαθήστε ξανά να τροποποιήσετε μια νέα πολιτική.</span><span class="sxs-lookup"><span data-stu-id="ffed9-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="ffed9-113">Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, δοκιμάστε το PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ffed9-113">If you're still having problems, try PowerShell.</span></span>  