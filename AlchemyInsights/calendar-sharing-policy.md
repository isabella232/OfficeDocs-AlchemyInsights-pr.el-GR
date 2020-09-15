---
title: Πολιτική κοινής χρήσης ημερολογίου του 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684230"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="98965-102">Σφάλμα πολιτικής κατά την κοινή χρήση ενός ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="98965-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="98965-103">Κάντε ένα από τα εξής, ανάλογα με την περίπτωσή σας:</span><span class="sxs-lookup"><span data-stu-id="98965-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="98965-104">Συνδεθείτε στο Exchange Online χρησιμοποιώντας το Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="98965-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="98965-105">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα σύνδεση στο Exchange Online με χρήση απομακρυσμένου PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="98965-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="98965-106">Στο διακομιστή εσωτερικής εγκατάστασης, ανοίξτε το κέλυφος διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="98965-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="98965-107">Προσδιορίστε την πολιτική κοινής χρήσης που έχει εκχωρηθεί στο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="98965-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="98965-108">Για να το κάνετε αυτό, εκτελέστε την ακόλουθη εντολή και σημειώστε την πολιτική που επιστράφηκε:</span><span class="sxs-lookup"><span data-stu-id="98965-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="98965-109">Ενημερώστε την πολιτική κοινής χρήσης για το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="98965-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="98965-110">Για να το κάνετε, ακολουθήστε αυτά τα βήματα:</span><span class="sxs-lookup"><span data-stu-id="98965-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="98965-111">Ανοίξτε το κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="98965-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="98965-112">Κάντε κλικ στην επιλογή **εταιρεία**και, στη συνέχεια, κάντε διπλό κλικ στην πολιτική που έχει εκχωρηθεί στο χρήστη στην περιοχή **μεμονωμένη κοινή χρήση**.</span><span class="sxs-lookup"><span data-stu-id="98965-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="98965-113">Αυτή είναι η πολιτική που επιστράφηκε στο βήμα 2.</span><span class="sxs-lookup"><span data-stu-id="98965-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="98965-114">Στη σελίδα "κανόνας κοινής χρήσης", επιλέξτε το επίπεδο κοινής χρήσης ημερολογίου που θέλετε να επιτρέψετε στην περιοχή **Καθορίστε τις πληροφορίες που θέλετε να μοιραστείτε**. Κάντε κλικ στην επιλογή **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="98965-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="98965-115">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα: "η πολιτική δεν επιτρέπει την εκχώρηση δικαιωμάτων σε αυτό το επίπεδο σε έναν ή περισσότερους από τους παραλήπτες" σφάλμα όταν ο χρήστης προσπαθήσει να κάνει κοινή χρήση του ημερολογίου](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="98965-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
