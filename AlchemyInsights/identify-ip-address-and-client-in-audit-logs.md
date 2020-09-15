---
title: Προσδιορισμός της διεύθυνσης IP και του προγράμματος-πελάτη σε αρχεία καταγραφής ελέγχου
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668310"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="1c0e2-102">Προσδιορισμός της διεύθυνσης IP και του προγράμματος-πελάτη σε αρχεία καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="1c0e2-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="1c0e2-103">Η διεύθυνση IP που αντιστοιχεί σε μια δραστηριότητα από ένα χρήστη ή διαχειριστή του Microsoft 365 εμφανίζεται στα αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="1c0e2-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="1c0e2-104">Καταγράφονται επίσης οι πληροφορίες του προγράμματος-πελάτη.</span><span class="sxs-lookup"><span data-stu-id="1c0e2-104">The client information is also logged.</span></span> <span data-ttu-id="1c0e2-105">Εδώ θα βρείτε τα βήματα για τον εντοπισμό τέτοιων πληροφοριών</span><span class="sxs-lookup"><span data-stu-id="1c0e2-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="1c0e2-106">Συνδεθείτε στο [Κέντρο συμμόρφωσης & ασφαλείας του Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1c0e2-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1c0e2-107">Μεταβείτε στη σελίδα **Search**αναζήτησης του  >  **αρχείου καταγραφής ελέγχου** αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="1c0e2-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="1c0e2-108">Εάν σας ενδιαφέρει μια συγκεκριμένη δραστηριότητα, επιλέξτε την από τη λίστα **δραστηριότητες** .</span><span class="sxs-lookup"><span data-stu-id="1c0e2-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="1c0e2-109">Εάν όχι, όλες οι δραστηριότητες θα επιστραφούν για τον επιλεγμένο χρήστη (προεπιλεγμένη ρύθμιση).</span><span class="sxs-lookup"><span data-stu-id="1c0e2-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="1c0e2-110">**Σημείωση**: ορισμένες δραστηριότητες ενδέχεται να μην είναι διαθέσιμες στο μενού **δραστηριότητες** . Ωστόσο, αυτά τα στοιχεία ελέγχου θα επιστραφούν εάν είναι επιλεγμένο το στοιχείο **Εμφάνιση αποτελεσμάτων για όλες τις δραστηριότητες** (προεπιλεγμένη ρύθμιση).</span><span class="sxs-lookup"><span data-stu-id="1c0e2-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="1c0e2-111">Καθορίστε το όνομα χρήστη στο πεδίο **χρήστες** , επιλέξτε το κατάλληλο εύρος ημερομηνιών για τη δραστηριότητα και, στη συνέχεια, κάντε κλικ στην επιλογή **Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="1c0e2-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="1c0e2-112">Στα αποτελέσματα, μπορείτε να δείτε τη διεύθυνση IP για τη συγκεκριμένη δραστηριότητα στο παράθυρο αποτελεσμάτων.</span><span class="sxs-lookup"><span data-stu-id="1c0e2-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="1c0e2-113">Επιλέξτε την εγγραφή ελέγχου για να δείτε λεπτομερείς πληροφορίες στο αναδυόμενο στοιχείο **λεπτομερειών** (για παράδειγμα, πρόγραμμα-πελάτης, χρήστης που πραγματοποίησε ενέργεια, κ. λπ.).</span><span class="sxs-lookup"><span data-stu-id="1c0e2-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="1c0e2-114">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Εύρεση της ΔΙΕΎΘΥΝΣΗς IP του υπολογιστή που χρησιμοποιείται για την πρόσβαση σε έναν λογαριασμό σε κίνδυνο](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="1c0e2-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
