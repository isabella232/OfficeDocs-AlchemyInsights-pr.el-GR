---
title: Παράκαμψη αίθουσας αναμονής
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820034"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="cc128-102">Έλεγχος ρυθμίσεων του αναμονής και του επιπέδου συμμετοχής στο Teams</span><span class="sxs-lookup"><span data-stu-id="cc128-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="cc128-103">Εάν θέλετε να επιτρέψετε σε όλους, συμπεριλαμβανομένων των χρηστών με κλήση σύνδεσης, εξωτερικούς και ανώνυμους χρήστες, να παρακάμψουν το χώρο αναμονής, χρησιμοποιήστε το PowerShell για να επιτύχετε αυτή την εργασία.</span><span class="sxs-lookup"><span data-stu-id="cc128-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="cc128-104">Ακολουθεί ένα παράδειγμα τροποποίησης της πολιτικής καθολικής σύσκεψης για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="cc128-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="cc128-105">Προς το παρόν, αυτό το cmdlet απαιτεί τη χρήση της λειτουργικής μονάδας PowerShell του Skype για επιχειρήσεις.</span><span class="sxs-lookup"><span data-stu-id="cc128-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="cc128-106">Για να ρυθμίσετε τη χρήση αυτού του cmdlet, ανατρέξτε στο θέμα [Διαχείριση πολιτικών μέσω του PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="cc128-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="cc128-107">Αφού ρυθμίσετε μια πολιτική, πρέπει να την εφαρμόσετε στους χρήστες. ή, εάν τροποποιήσατε την καθολική πολιτική, θα εφαρμοστεί αυτόματα στους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="cc128-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="cc128-108">Για οποιαδήποτε αλλαγή πολιτικής, πρέπει να περιμένετε τουλάχιστον **4 ώρες έως και 24 ώρες για** να ισχύουν οι πολιτικές.</span><span class="sxs-lookup"><span data-stu-id="cc128-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="cc128-109">Φροντίστε να εξετάσετε την τεκμηρίωση παρακάτω πριν κάνετε αυτές τις αλλαγές για να κατανοήσετε ακριβώς τι επιτρέπει αυτό.</span><span class="sxs-lookup"><span data-stu-id="cc128-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="cc128-110">Κατανόηση των στοιχείων ελέγχου πολιτικής ομάδων αναμονής συσκέψεων του Teams</span><span class="sxs-lookup"><span data-stu-id="cc128-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="cc128-111">Αυτές οι ρυθμίσεις ελέγχουν ποιοι συμμετέχοντες της σύσκεψης περιμένουν στο χώρο αναμονής πριν από την εισαγωγή τους στη σύσκεψη και το επίπεδο συμμετοχής που επιτρέπεται σε μια σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="cc128-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="cc128-112">Μπορείτε να χρησιμοποιήσετε το PowerShell για να ενημερώσετε τις ρυθμίσεις πολιτικής σύσκεψης που δεν έχουν εφαρμοστεί ακόμη (με την ετικέτα "σύντομα σύντομα") στο κέντρο διαχείρισης του Teams.</span><span class="sxs-lookup"><span data-stu-id="cc128-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="cc128-113">Δείτε παρακάτω ένα παράδειγμα cmdlet του PowerShell που επιτρέπει σε όλους τους χρήστες να παρακάμπτουν το χώρο αναμονής.</span><span class="sxs-lookup"><span data-stu-id="cc128-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="cc128-114">[Η αυτόματη αποδοχή ατόμων](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) είναι μια πολιτική ανά διοργανωτή που ελέγχει εάν τα άτομα συμμετέχουν απευθείας σε μια σύσκεψη ή περιμένουν στο χώρο αναμονής μέχρι να παραδεχθούν από έναν χρήστη με έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="cc128-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="cc128-115">Η [δυνατότητα](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ανώνυμων ατόμων να ξεκινούν μια σύσκεψη είναι μια πολιτική ανά διοργανωτή που ελέγχει εάν οι ανώνυμοι χρήστες, συμπεριλαμβανομένων των B2B και των ομόσπονδων χρηστών, μπορούν να συμμετάσχουν στη σύσκεψη του χρήστη χωρίς να έχει υποβληθεί σε έλεγχο ταυτότητας χρήστης από την εταιρεία.</span><span class="sxs-lookup"><span data-stu-id="cc128-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="cc128-116">[Η δυνατότητα των](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) χρηστών με κλήση σύνδεσης να παρακάμπτουν το χώρο αναμονής **(σύντομα** σύντομα) είναι μια πολιτική ανά διοργανωτή που ελέγχει εάν τα άτομα που κάνουν κλήση μέσω τηλεφώνου συμμετέχουν απευθείας στη σύσκεψη ή περιμένουν στο χώρο αναμονής, ανεξάρτητα από τη ρύθμιση "Αυτόματη **αποδοχή** ατόμων".</span><span class="sxs-lookup"><span data-stu-id="cc128-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="cc128-117">Η δυνατότητα [των διοργανωτών](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) να παρακάμπτουν τις ρυθμίσεις του αναμονής (σύντομα σύντομα) είναι  μια πολιτική  ανά διοργανωτή που ελέγχει εάν ο διοργανωτής της σύσκεψης μπορεί να παρακάμψει τις ρυθμίσεις αναμονής που έχει ορίσει ένας διαχειριστής στο πλαίσιο "Αυτόματη αποδοχή ατόμων" και "Να επιτρέπεται στους χρήστες με κλήση σύνδεσης" να παρακάμπτουν το χώρο αναμονής όταν προγραμματούν μια νέα σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="cc128-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="cc128-118">**Σημείωση:** Διαβάστε [το άρθρο Διαχείριση πολιτικών σύσκεψης στο Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) για μια πλήρη επισκόπηση των πολιτικών σύσκεψης του Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cc128-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
