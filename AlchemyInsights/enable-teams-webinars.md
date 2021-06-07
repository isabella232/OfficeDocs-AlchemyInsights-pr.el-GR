---
title: Ενεργοποίηση Teams Webinar
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793649"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="b7dc4-102">Ενεργοποίηση Teams Webinar</span><span class="sxs-lookup"><span data-stu-id="b7dc4-102">Enable Teams Webinars</span></span>

<span data-ttu-id="b7dc4-103">Τα webinar είναι ενεργοποιημένα από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="b7dc4-103">Webinars are enabled by default.</span></span> <span data-ttu-id="b7dc4-104">Μπορείτε να διαχειριστείτε ποιος μπορεί να προγραμματίσει και να εγγραφεί Teams webinar χρησιμοποιώντας Teams powerShell.</span><span class="sxs-lookup"><span data-stu-id="b7dc4-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="b7dc4-105">Όλοι οι χρήστες που μπορούν να δημιουργήσουν μια σύσκεψη μπορούν επίσης να δημιουργήσουν μια σύσκεψη webinar.</span><span class="sxs-lookup"><span data-stu-id="b7dc4-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="b7dc4-106">Εάν θέλετε να διαχειριστείτε ποιος μπορεί να προγραμματίσει Teams Webinar, χρησιμοποιήστε *το AllowMeetingRegistration.*</span><span class="sxs-lookup"><span data-stu-id="b7dc4-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="b7dc4-107">Από προεπιλογή, *το WhoCanRegister είναι* ενεργοποιημένο και έχει οριστεί σε **"Όλοι".**</span><span class="sxs-lookup"><span data-stu-id="b7dc4-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="b7dc4-108">Εάν θέλετε να απενεργοποιήσετε την καταχώρηση σύσκεψης, ορίστε *την τιμή AllowMeetingRegistration* σε **False.**</span><span class="sxs-lookup"><span data-stu-id="b7dc4-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="b7dc4-109">Για να αλλάξετε αυτές τις ρυθμίσεις, πρέπει να [εγκαταστήσετε Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="b7dc4-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="b7dc4-110">Επίσης, οι πολιτικές σύσκεψης επιβάλλονται σε Teams Web.</span><span class="sxs-lookup"><span data-stu-id="b7dc4-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="b7dc4-111">Για παράδειγμα, εάν η ανώνυμη συμμετοχή είναι απενεργοποιημένη στις ρυθμίσεις σύσκεψης, οι ανώνυμοι χρήστες δεν μπορούν να συμμετάσχουν σε webinars.</span><span class="sxs-lookup"><span data-stu-id="b7dc4-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="b7dc4-112">Για να μάθετε περισσότερα σχετικά με τη ρύθμιση παραμέτρων για άτομα που μπορούν να εγγραφούν για webinar, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων για τα άτομα που μπορούν να [εγγραφούν για webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="b7dc4-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="b7dc4-113">Για περισσότερες πληροφορίες σχετικά με τις ρυθμίσεις για τις λίστες microsoft, ανατρέξτε στο [θέμα Ρυθμίσεις ελέγχου για τις λίστες της Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="b7dc4-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>