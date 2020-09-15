---
title: Παράκαμψη λόμπι
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684950"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="28826-102">Έλεγχος των ρυθμίσεων του λόμπι και του επιπέδου συμμετοχής σε ομάδες</span><span class="sxs-lookup"><span data-stu-id="28826-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="28826-103">Εάν θέλετε να επιτρέψετε σε όλους, συμπεριλαμβανομένης της σύνδεσης, των εξωτερικών και των ανώνυμων χρηστών, να **παρακάμπτουν το λόμπι**, χρησιμοποιήστε το PowerShell για να ολοκληρώσετε αυτή την εργασία.</span><span class="sxs-lookup"><span data-stu-id="28826-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="28826-104">Ακολουθεί ένα παράδειγμα τροποποίησης της πολιτικής καθολικής σύσκεψης για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="28826-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="28826-105">Αυτό το cmdlet απαιτεί αυτήν τη στιγμή τη χρήση της λειτουργικής μονάδας του Skype για Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28826-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="28826-106">Για να λάβετε ρύθμιση για να χρησιμοποιήσετε αυτό το cmdlet, ανατρέξτε στο θέμα [Διαχείριση πολιτικών μέσω PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="28826-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="28826-107">Αφού ρυθμίσετε μια πολιτική, πρέπει να την εφαρμόσετε στους χρήστες. Εναλλακτικά, εάν έχετε τροποποιήσει την καθολική πολιτική, αυτό θα ισχύει αυτόματα για τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="28826-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="28826-108">Για οποιαδήποτε αλλαγή πολιτικής, πρέπει να περιμένετε τουλάχιστον **4 ώρες έως και 24 ώρες** για να τεθούν σε ισχύ οι πολιτικές.</span><span class="sxs-lookup"><span data-stu-id="28826-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="28826-109">Φροντίστε να εξετάσετε την τεκμηρίωση παρακάτω πριν κάνετε αυτές τις αλλαγές για να καταλάβετε ακριβώς τι επιτρέπει αυτό.</span><span class="sxs-lookup"><span data-stu-id="28826-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="28826-110">Κατανόηση των στοιχείων ελέγχου πολιτικής λόμπι της σύσκεψης ομάδων</span><span class="sxs-lookup"><span data-stu-id="28826-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="28826-111">Αυτές οι ρυθμίσεις ελέγχουν ποιοι συμμετέχοντες στη σύσκεψη περιμένουν στο λόμπι πριν γίνουν δεκτοί στη σύσκεψη και το επίπεδο συμμετοχής που τους επιτρέπεται σε μια σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="28826-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="28826-112">Μπορείτε να χρησιμοποιήσετε το PowerShell για να ενημερώσετε τις ρυθμίσεις πολιτικής σύσκεψης που δεν έχουν υλοποιηθεί ακόμη (με την ετικέτα "σύντομα διαθέσιμο") στο κέντρο διαχείρισης ομάδων.</span><span class="sxs-lookup"><span data-stu-id="28826-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="28826-113">Δείτε παρακάτω για ένα παράδειγμα cmdlet PowerShell που επιτρέπει σε όλους τους χρήστες να παρακάμπτουν το λόμπι.</span><span class="sxs-lookup"><span data-stu-id="28826-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="28826-114">Η αυτόματη αποδοχή των [ατόμων](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) είναι μια πολιτική ανά διοργανωτή που ελέγχει εάν τα άτομα συμμετέχουν απευθείας σε μια σύσκεψη ή εάν περιμένουν στο λόμπι μέχρι να γίνουν δεκτοί από έναν εξουσιοδοτημένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="28826-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="28826-115">[Να επιτρέπεται στους ανώνυμους χρήστες να ξεκινούν μια σύσκεψη](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) είναι μια πολιτική ανά διοργανωτή που ελέγχει εάν τα ανώνυμα άτομα, συμπεριλαμβανομένων των χρηστών B2B και ομόσπονδη, μπορούν να συμμετέχουν στη σύσκεψη του χρήστη χωρίς εξουσιοδοτημένο χρήστη από τον οργανισμό παρουσίας του.</span><span class="sxs-lookup"><span data-stu-id="28826-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="28826-116">[Επιτρέψτε στους χρήστες με κλήση σύνδεσης να παρακάμπτουν το λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**σύντομα διαθέσιμο**) είναι μια πολιτική ανά διοργανωτή που ελέγχει εάν τα άτομα που καλούν μέσω τηλεφώνου συμμετέχουν στη σύσκεψη απευθείας ή περιμένουν στο λόμπι ανεξάρτητα από τη ρύθμιση **Αυτόματη αποδοχή ατόμων** .</span><span class="sxs-lookup"><span data-stu-id="28826-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="28826-117">[Επιτρέψτε στους διοργανωτές να παρακάμπτουν τις ρυθμίσεις του λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**σύντομα**) είναι μια πολιτική ανά διοργανωτή που ελέγχει εάν ο διοργανωτής της σύσκεψης μπορεί να παρακάμψει τις ρυθμίσεις του λόμπι που ένας διαχειριστής έχει ρυθμίσει **αυτόματα να δέχεται άτομα** και **να επιτρέπει στους χρήστες με κλήση σύνδεσης να παρακάμπτουν το λόμπι** όταν προγραμματίζουν μια νέα σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="28826-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="28826-118">**Σημείωση:** Διαβάστε [το άρθρο Διαχείριση πολιτικών συσκέψεων στο teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) για μια ολοκληρωμένη επισκόπηση των πολιτικών σύσκεψης του Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="28826-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
