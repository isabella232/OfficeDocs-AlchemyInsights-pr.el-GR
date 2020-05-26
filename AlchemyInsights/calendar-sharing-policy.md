---
title: Πολιτική κοινής χρήσης ημερολογίου 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372999"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="cd544-102">Σφάλμα πολιτικής κατά την κοινή χρήση ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="cd544-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="cd544-103">Κάντε ένα από τα εξής, ανάλογα με την περίπτωσή σας:</span><span class="sxs-lookup"><span data-stu-id="cd544-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="cd544-104">Συνδεθείτε στο Exchange Online χρησιμοποιώντας το Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cd544-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="cd544-105">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Σύνδεση στο Exchange Online με χρήση του Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="cd544-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="cd544-106">Στο διακομιστή εσωτερικής εγκατάστασης, ανοίξτε το κέλυφος διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd544-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="cd544-107">Καθορίστε την πολιτική κοινής χρήσης που έχει αντιστοιχιστεί στο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="cd544-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="cd544-108">Για να το κάνετε αυτό, εκτελέστε την ακόλουθη εντολή και σημειώστε την πολιτική που επιστράφηκε:</span><span class="sxs-lookup"><span data-stu-id="cd544-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="cd544-109">Ενημερώστε την πολιτική κοινής χρήσης για το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="cd544-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="cd544-110">Για να το κάνετε, ακολουθήστε αυτά τα βήματα:</span><span class="sxs-lookup"><span data-stu-id="cd544-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="cd544-111">Ανοίξτε το κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd544-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="cd544-112">Κάντε κλικ στην επιλογή **Οργανισμός**και, στη συνέχεια, κάντε διπλό κλικ στην πολιτική που έχει αντιστοιχιστεί στο χρήστη στην περιοχή **Μεμονωμένη κοινή χρήση**.</span><span class="sxs-lookup"><span data-stu-id="cd544-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="cd544-113">Αυτή είναι η πολιτική που επιστράφηκε στο βήμα 2.</span><span class="sxs-lookup"><span data-stu-id="cd544-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="cd544-114">Στη σελίδα "Κανόνες κοινής χρήσης", επιλέξτε το επίπεδο κοινής χρήσης ημερολογίου που θέλετε να επιτρέψετε στην περιοχή **Καθορισμός των πληροφοριών που θέλετε να μοιραστείτε.** κάντε κλικ στην επιλογή **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="cd544-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="cd544-115">Για περισσότερες πληροφορίες, ανατρέξτε: ["Η πολιτική δεν επιτρέπει την εκχώρηση δικαιωμάτων σε αυτό το επίπεδο σε έναν ή περισσότερους παραλήπτες" όταν ο χρήστης προσπαθεί να κάνει κοινή χρήση ημερολογίου](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="cd544-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
