---
title: Το μήνυμα ηλεκτρονικού ταχυδρομείου της ροής εργασίας δεν αποστέλλεται
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049373"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="1892e-102">Δεν αποστέλλεται μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας για μια λίστα ή βιβλιοθήκη του SharePoint</span><span class="sxs-lookup"><span data-stu-id="1892e-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="1892e-103">Τα μηνύματα ηλεκτρονικού ταχυδρομείου από ροές εργασίας δεν αποστέλλονται σε όλους τους χρήστες ή μόνο σε συγκεκριμένους χρήστες ή μπορείτε να δείτε το σφάλμα **δεν είναι δυνατή η αποστολή του μηνύματος ηλεκτρονικού ταχυδρομείου. Βεβαιωθείτε ότι το μήνυμα ηλεκτρονικού ταχυδρομείου έχει έγκυρο παραλήπτη**.</span><span class="sxs-lookup"><span data-stu-id="1892e-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="1892e-104">Ελέγξτε εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων **όλων των ατόμων** (λίστα πληροφοριών χρήστη) για αυτήν τη συλλογή τοποθεσιών.</span><span class="sxs-lookup"><span data-stu-id="1892e-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="1892e-105">Δείγμα άμεσης διεύθυνσης URL:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/Loot.MCA; Κράτος μέλους = 0</span><span class="sxs-lookup"><span data-stu-id="1892e-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="1892e-106">Εάν ο χρήστης δεν υπάρχει, βεβαιωθείτε ότι ο χρήστης είναι συνδεδεμένος στη σελίδα.</span><span class="sxs-lookup"><span data-stu-id="1892e-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="1892e-107">Εάν πρόκειται για εξωτερικό χρήστη, βεβαιωθείτε ότι η πρόσκλησή τους έχει γίνει δεκτή.</span><span class="sxs-lookup"><span data-stu-id="1892e-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="1892e-108">Εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων, βεβαιωθείτε ότι η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σωστή.</span><span class="sxs-lookup"><span data-stu-id="1892e-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="1892e-109">Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου των χρηστών δεν έχει οριστεί εδώ, τότε Δημιουργήστε ένα δείγμα ειδοποίησης για αυτόν το χρήστη που αναγκάζει τον συγχρονισμό αυτού του λογαριασμού χρήστη από προφίλ χρήστη του SharePoint σε αυτήν τη συλλογή τοποθεσιών.</span><span class="sxs-lookup"><span data-stu-id="1892e-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="1892e-110">Μηνύματα ηλεκτρονικού ταχυδρομείου από ροές εργασίας αποστέλλονται στους διαχειριστές συλλογής τοποθεσιών, αλλά όχι σε άλλους χρήστες και να δείτε το σφάλμα **http απαγορεύεται σε <span>https:</span>/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="1892e-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="1892e-111">Δείτε [δεν επιτρέπεται η πρόσβαση όταν στέλνετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="1892e-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="1892e-112">Επίσης, επαληθεύστε ότι η δυνατότητα συλλογής τοποθεσιών της **λειτουργίας κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης** δεν είναι ενεργή.</span><span class="sxs-lookup"><span data-stu-id="1892e-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="1892e-113">Σχετικά θέματα</span><span class="sxs-lookup"><span data-stu-id="1892e-113">Related topics</span></span>
<span data-ttu-id="1892e-114">Θέλετε να δοκιμάσετε το Microsoft Flow στο SharePoint Online;</span><span class="sxs-lookup"><span data-stu-id="1892e-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1892e-115">Δημιουργία ροής</span><span class="sxs-lookup"><span data-stu-id="1892e-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1892e-116">SharePoint και ροή</span><span class="sxs-lookup"><span data-stu-id="1892e-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


