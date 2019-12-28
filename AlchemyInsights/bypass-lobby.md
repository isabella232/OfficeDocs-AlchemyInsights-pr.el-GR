---
title: Παράκαμψη λόμπι
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889082"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="6197e-102">Έλεγχος των ρυθμίσεων του λόμπι και του επιπέδου συμμετοχής σε ομάδες</span><span class="sxs-lookup"><span data-stu-id="6197e-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="6197e-103">Αν θέλετε να επιτρέψετε σε όλους, συμπεριλαμβανομένων των τηλεφωνικών κλήσεων, των εξωτερικών και των ανώνυμων χρηστών, να **παρακάμπτουν το λόμπι**, χρησιμοποιήστε το PowerShell για να ολοκληρώσετε αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="6197e-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="6197e-104">Ακολουθούν ένα παράδειγμα τροποποίησης της καθολικής σύσκεψης πολιτικής για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="6197e-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="6197e-105">Αυτό το cmdlet απαιτεί αυτήν τη στιγμή τη χρήση του Skype για επαγγελματική PowerShell λειτουργική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="6197e-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="6197e-106">Για να ρυθμίσετε για να χρησιμοποιήσετε αυτό το cmdlet, ελέγξτε τη [Διαχείριση πολιτικών μέσω PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="6197e-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="6197e-107">Αφού ορίσετε μια πολιτική, θα πρέπει να την εφαρμόσετε στους χρήστες. ή, εάν τροποποιήσατε την καθολική πολιτική, θα ισχύει αυτόματα για τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="6197e-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="6197e-108">Για οποιαδήποτε αλλαγή πολιτικής, πρέπει να περιμένετε τουλάχιστον **4 ώρες έως και 24 ώρες** για να ισχύσουν οι πολιτικές.</span><span class="sxs-lookup"><span data-stu-id="6197e-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="6197e-109">Βεβαιωθείτε ότι έχετε επανεξετάσει την τεκμηρίωση παρακάτω πριν κάνετε αυτές τις αλλαγές για να καταλάβετε ακριβώς τι επιτρέπει αυτό.</span><span class="sxs-lookup"><span data-stu-id="6197e-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="6197e-110">Κατανόηση των ομάδων που πληρούν τους ελέγχους πολιτικής του λόμπι</span><span class="sxs-lookup"><span data-stu-id="6197e-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="6197e-111">Αυτές οι ρυθμίσεις ελέγχουν ποιοι συμμετέχοντες στη σύσκεψη περιμένουν στο λόμπι πριν γίνουν δεκτοί στη σύσκεψη και το επίπεδο συμμετοχής που τους επιτρέπεται σε μια σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="6197e-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="6197e-112">Μπορείτε να χρησιμοποιήσετε το PowerShell για να ενημερώσετε τις ρυθμίσεις πολιτικής σύσκεψης που δεν έχουν ακόμη υλοποιηθεί (με την ένδειξη "προσεχώς") στο κέντρο διαχείρισης ομάδων.</span><span class="sxs-lookup"><span data-stu-id="6197e-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="6197e-113">Δείτε παρακάτω για ένα παράδειγμα cmdlet PowerShell που επιτρέπει σε όλους τους χρήστες να παρακάμψετε το λόμπι.</span><span class="sxs-lookup"><span data-stu-id="6197e-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="6197e-114">Η αυτόματη ένταξη των [ατόμων](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα συμμετέχουν σε μια σύσκεψη απευθείας ή περιμένουν στο λόμπι μέχρι να εισαχθούν από έναν εξουσιοδοτημένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="6197e-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="6197e-115">[Να επιτρέψετε σε ανώνυμους χρήστες να ξεκινήσουν μια σύσκεψη](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα ανώνυμα άτομα, συμπεριλαμβανομένων των χρηστών Β2Β και ομόσπονδων, μπορούν να ενταχθούν στη σύσκεψη του χρήστη χωρίς έλεγχο ταυτότητας χρήστη από τον οργανισμό στην παρουσία.</span><span class="sxs-lookup"><span data-stu-id="6197e-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="6197e-116">[Να επιτρέπεται στους χρήστες τηλεφωνικών κλήσεων να παρακάμπτουν το λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα που κάνουν κλήση μέσω τηλεφώνου συμμετέχουν στη σύσκεψη απευθείας ή περιμένουν στο λόμπι, ανεξάρτητα από την **Αυτόματη** αποδοχή των χρηστών.</span><span class="sxs-lookup"><span data-stu-id="6197e-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="6197e-117">[Επιτρέψτε στους διοργανωτές να παρακάμπτουν τις ρυθμίσεις του λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν ο οργανωτής της σύσκεψης μπορεί να παρακάμψει τις ρυθμίσεις του λόμπι που ένας διαχειριστής έχει ορίσει να δέχεται **αυτόματα άτομα** και **να επιτρέπει στους χρήστες εισερχόμενων κλήσεων να παρακάμπτουν το λόμπι** όταν προγραμματίσουν μια νέα σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="6197e-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="6197e-118">**Σημείωση:** Διαβάστε την [ενότητα Διαχείριση πολιτικών συσκέψεων στις ομάδες](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) για μια πλήρη επισκόπηση των πολιτικών συσκέψεων των ομάδων της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6197e-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
