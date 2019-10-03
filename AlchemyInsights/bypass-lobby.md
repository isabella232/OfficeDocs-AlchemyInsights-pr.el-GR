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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376657"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="7706b-102">Έλεγχος των ρυθμίσεων του λόμπι και του επιπέδου συμμετοχής</span><span class="sxs-lookup"><span data-stu-id="7706b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="7706b-103">Αυτές οι ρυθμίσεις ελέγχουν ποιοι συμμετέχοντες στη σύσκεψη περιμένουν στο λόμπι πριν γίνουν δεκτοί στη σύσκεψη και το επίπεδο συμμετοχής που τους επιτρέπεται σε μια σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="7706b-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="7706b-104">Μπορείτε να χρησιμοποιήσετε το PowerShell για να ενημερώσετε τις ρυθμίσεις πολιτικής σύσκεψης που δεν έχουν ακόμη υλοποιηθεί (με την ένδειξη "προσεχώς") στο κέντρο διαχείρισης ομάδων.</span><span class="sxs-lookup"><span data-stu-id="7706b-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="7706b-105">Δείτε παρακάτω για ένα παράδειγμα cmdlet PowerShell που επιτρέπει σε όλους τους χρήστες να παρακάμψετε το λόμπι.</span><span class="sxs-lookup"><span data-stu-id="7706b-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="7706b-106">Η αυτόματη ένταξη των [ατόμων](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα συμμετέχουν σε μια σύσκεψη απευθείας ή περιμένουν στο λόμπι μέχρι να εισαχθούν από έναν εξουσιοδοτημένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="7706b-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7706b-107">[Να επιτρέψετε σε ανώνυμους χρήστες να ξεκινήσουν μια σύσκεψη](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα ανώνυμα άτομα, συμπεριλαμβανομένων των χρηστών Β2Β και ομόσπονδων, μπορούν να ενταχθούν στη σύσκεψη του χρήστη χωρίς έλεγχο ταυτότητας χρήστη από τον οργανισμό στην παρουσία.</span><span class="sxs-lookup"><span data-stu-id="7706b-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7706b-108">[Να επιτρέπεται στους χρήστες τηλεφωνικών κλήσεων να παρακάμπτουν το λόμπι](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα που κάνουν κλήση μέσω τηλεφώνου συμμετέχουν στη σύσκεψη απευθείας ή περιμένουν στο λόμπι, ανεξάρτητα από την **Αυτόματη** αποδοχή των χρηστών.</span><span class="sxs-lookup"><span data-stu-id="7706b-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7706b-109">[Να επιτρέπεται στους διοργανωτές να παρακάμπτουν τις ρυθμίσεις του λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν ο οργανωτής της σύσκεψης μπορεί να παρακάμψει τις ρυθμίσεις του λόμπι που ένας διαχειριστής έχει ορίσει να δέχεται **αυτόματα άτομα** και να **επιτρέπει τη σύνδεση μέσω τηλεφώνου τους χρήστες να παρακάμψουν το λόμπι** όταν προγραμματίσουν μια νέα σύσκεψη.</span><span class="sxs-lookup"><span data-stu-id="7706b-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7706b-110">**Σημείωση:** Διαβάστε την [ενότητα Διαχείριση πολιτικών συσκέψεων στις ομάδες](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) για μια πλήρη επισκόπηση των πολιτικών συσκέψεων των ομάδων της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7706b-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="7706b-111">**Παράδειγμα PowerShell**</span><span class="sxs-lookup"><span data-stu-id="7706b-111">**PowerShell example**</span></span>

<span data-ttu-id="7706b-112">Αν θέλετε να επιτρέψετε σε όλους, συμπεριλαμβανομένων των εξωτερικών ή ανώνυμων χρηστών, να παρακάμπτουν το λόμπι, μπορείτε επίσης να χρησιμοποιήσετε το PowerShell για να ολοκληρώσετε αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="7706b-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="7706b-113">Ακολουθούν ένα παράδειγμα τροποποίησης της καθολικής σύσκεψης πολιτικής για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="7706b-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="7706b-114">(Φροντίστε να αναθεωρήσετε την παραπάνω τεκμηρίωση πριν κάνετε αυτές τις αλλαγές για να κατανοήσετε ακριβώς τι επιτρέπει αυτό.)</span><span class="sxs-lookup"><span data-stu-id="7706b-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="7706b-115">Σύνολο-ασφάλεια-ταυτότητα global-Αυτοπαραδεχτηθείχρήστες "όλοι"-επιτρέπεται η χρήση $True</span><span class="sxs-lookup"><span data-stu-id="7706b-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="7706b-116">Για περισσότερες πληροφορίες, δείτε το [σύνολο](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="7706b-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
