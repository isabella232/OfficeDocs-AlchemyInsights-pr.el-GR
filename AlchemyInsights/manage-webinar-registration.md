---
title: Διαχείριση καταχώρησης webinar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793707"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="4c16d-102">Διαχείριση καταχώρησης webinar</span><span class="sxs-lookup"><span data-stu-id="4c16d-102">Manage webinar registration</span></span>

<span data-ttu-id="4c16d-103">Διαχειρίζεστε τα άτομα που μπορούν να εγγραφούν Teams Webinars χρησιμοποιώντας Teams εντολές του Powershell.</span><span class="sxs-lookup"><span data-stu-id="4c16d-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="4c16d-104">Για να εγκαταστήσετε Teams Powershell, ανατρέξτε [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="4c16d-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="4c16d-105">Από προεπιλογή, *το WhoCanRegister είναι* ενεργοποιημένο και ορίζεται σε **EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="4c16d-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="4c16d-106">Για να επιτρέψετε σε οποιονδήποτε, συμπεριλαμβανομένων των ανώνυμων χρηστών, να καταχωρήσει την πολιτική σύσκεψης **σε "Όλοι",** χρησιμοποιώντας την εντολή Powershell:</span><span class="sxs-lookup"><span data-stu-id="4c16d-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="4c16d-107">**Σημείωση:** Εάν η ανώνυμη συμμετοχή είναι απενεργοποιημένη στις ρυθμίσεις σύσκεψης, οι ανώνυμοι χρήστες δεν μπορούν να συμμετάσχουν σε webinars.</span><span class="sxs-lookup"><span data-stu-id="4c16d-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="4c16d-108">Για να μάθετε περισσότερα και να ενεργοποιήσετε αυτήν τη ρύθμιση, [ανατρέξτε στο θέμα Διαχείριση ρυθμίσεων σύσκεψης Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="4c16d-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="4c16d-109">Εάν θέλετε να απενεργοποιήσετε την καταχώρηση σύσκεψης, ορίστε *την τιμή AllowMeetingRegistration* σε **False.**</span><span class="sxs-lookup"><span data-stu-id="4c16d-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="4c16d-110">Για να μάθετε περισσότερα σχετικά με τη ρύθμιση παραμέτρων για άτομα που μπορούν να εγγραφούν για webinar, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων για τα άτομα που μπορούν να [εγγραφούν για webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="4c16d-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="4c16d-111">Για περισσότερες πληροφορίες σχετικά με τις ρυθμίσεις για τις λίστες microsoft, ανατρέξτε στο [θέμα Ρυθμίσεις ελέγχου για τις λίστες της Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="4c16d-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
