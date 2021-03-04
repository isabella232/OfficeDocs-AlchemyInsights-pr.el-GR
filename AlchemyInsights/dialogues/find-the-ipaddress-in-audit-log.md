---
title: Εύρεση της διεύθυνσης IP στο αρχείο καταγραφής ελέγχου
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429505"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="786f6-102">Εύρεση της διεύθυνσης IP στο αρχείο καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="786f6-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="786f6-103">Η διεύθυνση IP που αντιστοιχεί σε μια δραστηριότητα που εκτελείται από ένα χρήστη ή διαχειριστή εμφανίζεται στα αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="786f6-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="786f6-104">Καταγράφονται επίσης οι πληροφορίες του προγράμματος-πελάτη.</span><span class="sxs-lookup"><span data-stu-id="786f6-104">The client information is also logged.</span></span> <span data-ttu-id="786f6-105">Δείτε πώς μπορείτε να προσδιορίσετε τη διεύθυνση IP:</span><span class="sxs-lookup"><span data-stu-id="786f6-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="786f6-106">Μεταβείτε στο [Κέντρο συμμόρφωσης ασφάλειας και συμμόρφωσης & του Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="786f6-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="786f6-107">Επιλέξτε **"Αναζήτηση**  >  **[αρχείου καταγραφής ελέγχου".](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="786f6-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="786f6-108">Εάν δείτε μια ειδοποίηση ότι πρέπει να ενεργοποιήσετε τον έλεγχο, προχωρήστε και ενεργοποιήστε τον τώρα.</span><span class="sxs-lookup"><span data-stu-id="786f6-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="786f6-109">Εάν αυτή η δυνατότητα δεν είναι ενεργοποιημένη, τα αποτελέσματα αναζήτησης δεν θα είναι σε θέση να τραβήξει δεδομένα από προηγούμενες ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="786f6-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="786f6-110">Εάν σας ενδιαφέρει μια συγκεκριμένη δραστηριότητα, επιλέξτε την από τη λίστα **"Δραστηριότητες".** Διαφορετικά, από προεπιλογή, όλες οι δραστηριότητες θα επιστρέφονται για τον επιλεγμένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="786f6-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="786f6-111">Σημειώστε ότι ορισμένες δραστηριότητες ενδέχεται να μην είναι διαθέσιμες για επιλογή από το **μενού "Δραστηριότητες".** Ωστόσο, αυτά τα στοιχεία ελέγχου θα επιστρέφονται εάν είναι **ενεργοποιημένη η επιλογή "Εμφάνιση αποτελεσμάτων για όλες** τις δραστηριότητες" (προεπιλεγμένη ρύθμιση).</span><span class="sxs-lookup"><span data-stu-id="786f6-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="786f6-112">Καθορίστε το εύρος ημερομηνιών και, στο **πεδίο "Χρήστες",** επιλέξτε το όνομα χρήστη για το χρήστη που θέλετε να διερευνήσετε.</span><span class="sxs-lookup"><span data-stu-id="786f6-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="786f6-113">Επιλέξτε **"Αναζήτηση".**</span><span class="sxs-lookup"><span data-stu-id="786f6-113">Select **Search**.</span></span> <span data-ttu-id="786f6-114">Οι δραστηριότητες εμφανίζονται στην περιοχή **"Αποτελέσματα".**</span><span class="sxs-lookup"><span data-stu-id="786f6-114">The activities appear under **Results**.</span></span> <span data-ttu-id="786f6-115">Μπορείτε να δείτε τη διεύθυνση IP για κάθε δραστηριότητα.</span><span class="sxs-lookup"><span data-stu-id="786f6-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="786f6-116">Για να προβάλετε λεπτομέρειες, επιλέξτε μια δραστηριότητα και, στη συνέχεια, επιλέξτε **"Περισσότερες πληροφορίες".**</span><span class="sxs-lookup"><span data-stu-id="786f6-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="786f6-117">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα "Αναζήτηση στο [αρχείο καταγραφής ελέγχου του Office 365" για να αντιμετωπίσετε συνηθισμένα σενάρια.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="786f6-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>