---
title: Προσδιορισμός διεύθυνσης IP και προγράμματος-πελάτη στα αρχεία καταγραφής ελέγχου
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716388"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="5f4d8-102">Προσδιορισμός διεύθυνσης IP και προγράμματος-πελάτη στα αρχεία καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="5f4d8-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="5f4d8-103">Η διεύθυνση IP που αντιστοιχεί σε μια δραστηριότητα ενός χρήστη ή διαχειριστή της Microsoft 365 εμφανίζεται στα αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="5f4d8-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="5f4d8-104">Καταγράφονται επίσης οι πληροφορίες του υπολογιστή-πελάτη.</span><span class="sxs-lookup"><span data-stu-id="5f4d8-104">The client information is also logged.</span></span> <span data-ttu-id="5f4d8-105">Ακολουθούν τα βήματα για τον προσδιορισμό αυτών των πληροφοριών</span><span class="sxs-lookup"><span data-stu-id="5f4d8-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="5f4d8-106">Συνδεθείτε στο [Κέντρο & συμμόρφωσης ασφαλείας της Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="5f4d8-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="5f4d8-107">Μεταβείτε στη σελίδα**αναζήτησης αρχείου καταγραφής ελέγχου αναζήτησης.** **Search** > </span><span class="sxs-lookup"><span data-stu-id="5f4d8-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="5f4d8-108">Αν ενδιαφέρεστε για μια συγκεκριμένη δραστηριότητα, επιλέξτε την από τη λίστα **Δραστηριότητες.**</span><span class="sxs-lookup"><span data-stu-id="5f4d8-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="5f4d8-109">Εάν όχι, όλες οι δραστηριότητες θα επιστραφούν για τον επιλεγμένο χρήστη (προεπιλεγμένη ρύθμιση).</span><span class="sxs-lookup"><span data-stu-id="5f4d8-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="5f4d8-110">**Σημείωση**: Ορισμένες δραστηριότητες ενδέχεται να μην είναι διαθέσιμες στο μενού **"Δραστηριότητες".** Ωστόσο, αυτά τα στοιχεία ελέγχου θα επιστραφούν εάν είναι επιλεγμένο **το στοιχείο "Εμφάνιση αποτελεσμάτων για όλες τις δραστηριότητες"** (προεπιλεγμένη ρύθμιση).</span><span class="sxs-lookup"><span data-stu-id="5f4d8-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="5f4d8-111">Καθορίστε το όνομα χρήστη στο πεδίο **Χρήστες,** επιλέξτε το κατάλληλο εύρος ημερομηνιών για τη δραστηριότητα και, στη συνέχεια, κάντε κλικ στην επιλογή **Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="5f4d8-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="5f4d8-112">Στα αποτελέσματα, μπορείτε να δείτε τη διεύθυνση IP για αυτήν τη δραστηριότητα στο παράθυρο αποτελεσμάτων.</span><span class="sxs-lookup"><span data-stu-id="5f4d8-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="5f4d8-113">Επιλέξτε την καρτέλα ελέγχου για να δείτε **λεπτομερείς** πληροφορίες στο αναδυόμενο στοιχείο Λεπτομέρειες (για παράδειγμα, Πρόγραμμα-πελάτης, Χρήστης που εκτέλεσε ενέργεια κ.λπ.).</span><span class="sxs-lookup"><span data-stu-id="5f4d8-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="5f4d8-114">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εύρεση της διεύθυνσης IP του υπολογιστή που χρησιμοποιείται για την πρόσβαση σε λογαριασμό που έχει παραβιαστεί](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="5f4d8-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
