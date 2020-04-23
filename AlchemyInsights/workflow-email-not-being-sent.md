---
title: Το μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας δεν αποστέλλεται
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766133"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="32810-102">Το μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας δεν αποστέλλεται για λίστα ή βιβλιοθήκη του SharePoint</span><span class="sxs-lookup"><span data-stu-id="32810-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="32810-103">Το ηλεκτρονικό ταχυδρομείο από ροές εργασίας δεν αποστέλλεται σε όλους τους χρήστες ή μόνο σε συγκεκριμένους χρήστες ή βλέπετε το σφάλμα Δεν είναι δυνατή η αποστολή του **μηνύματος ηλεκτρονικού ταχυδρομείου. Βεβαιωθείτε ότι το μήνυμα ηλεκτρονικού ταχυδρομείου έχει έγκυρο παραλήπτη**.</span><span class="sxs-lookup"><span data-stu-id="32810-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="32810-104">Ελέγξτε εάν ο χρήστης υπάρχει στην ομάδα **"Όλα τα άτομα"** (λίστα πληροφοριών χρήστη) για αυτήν τη συλλογή τοποθεσιών.</span><span class="sxs-lookup"><span data-stu-id="32810-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="32810-105">Δείγμα άμεσης<tenant>διεύθυνσης<sitename>URL: https:// .sharepoint.com/sites/ /_layouts/15/people.aspx; Αναγνωριστικό ομάδας μελών=0</span><span class="sxs-lookup"><span data-stu-id="32810-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="32810-106">Εάν ο χρήστης δεν υπάρχει, βεβαιωθείτε ότι ο χρήστης είναι συνδεδεμένος στη σελίδα.</span><span class="sxs-lookup"><span data-stu-id="32810-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="32810-107">Εάν πρόκειται για εξωτερικό χρήστη, βεβαιωθείτε ότι η πρόσκλησή του έχει γίνει αποδεκτή.</span><span class="sxs-lookup"><span data-stu-id="32810-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="32810-108">Εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων, βεβαιωθείτε ότι η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σωστή.</span><span class="sxs-lookup"><span data-stu-id="32810-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="32810-109">Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου των χρηστών δεν έχει οριστεί εδώ, δημιουργήστε ένα δείγμα ειδοποίησης για αυτόν το χρήστη, το οποίο επιβάλλει το συγχρονισμό αυτού του λογαριασμού χρήστη από προφίλ χρηστών του SharePoint σε αυτήν τη συλλογή τοποθεσιών.</span><span class="sxs-lookup"><span data-stu-id="32810-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="32810-110">Το ηλεκτρονικό ταχυδρομείο από ροές εργασίας αποστέλλεται στους διαχειριστές συλλογής τοποθεσιών, αλλά όχι σε άλλους χρήστες και δείτε το σφάλμα **HTTP Απαγορεύεται να <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="32810-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="32810-111">Ανατρέξτε [στο θέμα Δεν επιτρέπεται η πρόσβαση όταν στέλνετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="32810-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="32810-112">Επίσης, βεβαιωθείτε ότι η δυνατότητα συλλογής τοποθεσιών **λειτουργίας κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης** δεν είναι ενεργή.</span><span class="sxs-lookup"><span data-stu-id="32810-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="32810-113">Σχετικά θέματα</span><span class="sxs-lookup"><span data-stu-id="32810-113">Related topics</span></span>
<span data-ttu-id="32810-114">Θέλετε να δοκιμάσετε το Microsoft Flow στο SharePoint Online;</span><span class="sxs-lookup"><span data-stu-id="32810-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="32810-115">Δημιουργία ροής</span><span class="sxs-lookup"><span data-stu-id="32810-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="32810-116">Το SharePoint και η ροή</span><span class="sxs-lookup"><span data-stu-id="32810-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


