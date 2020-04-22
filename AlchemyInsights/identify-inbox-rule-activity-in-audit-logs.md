---
title: Προσδιορισμός δραστηριότητας κανόνα εισερχομένων στα αρχεία καταγραφής ελέγχου
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716424"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="87c40-102">Προσδιορισμός δραστηριότητας κανόνα εισερχομένων στα αρχεία καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="87c40-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="87c40-103">Μπορείτε να χρησιμοποιήσετε την αναζήτηση αρχείου καταγραφής ελέγχου στο Κέντρο συμμόρφωσης microsoft 365 Security & για να προβάλετε συμβάντα κανόνων εισερχομένων (δημιουργία, τροποποίηση και διαγραφή κανόνων εισερχομένων).</span><span class="sxs-lookup"><span data-stu-id="87c40-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="87c40-104">Συνδεθείτε στο [Κέντρο & συμμόρφωσης ασφαλείας της Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="87c40-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="87c40-105">Μεταβείτε στη σελίδα**αναζήτησης αρχείου καταγραφής ελέγχου αναζήτησης.** **Search** > </span><span class="sxs-lookup"><span data-stu-id="87c40-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="87c40-106">Επιλέξτε το εύρος ημερομηνιών στα πεδία **Ημερομηνία έναρξης** και **Ημερομηνία λήξης.**</span><span class="sxs-lookup"><span data-stu-id="87c40-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="87c40-107">Στην περιοχή **Δραστηριότητες γραμματοκιβωτίου του Exchange**, βεβαιωθείτε ότι το πεδίο **"Δραστηριότητες"** έχει οριστεί σε **Κανόνας δημιουργίας/τροποποίησης/ενεργοποίησης/απενεργοποίησης εισερχομένων "Νέος κανόνας εισερχομένων "**.</span><span class="sxs-lookup"><span data-stu-id="87c40-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="87c40-108">Κάντε κλικ στην **επιλογή Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="87c40-108">Click **Search**.</span></span>

<span data-ttu-id="87c40-109">Στα αποτελέσματα, επιλέξτε μια καρτέλα ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="87c40-109">In the results, select an audit record.</span></span> <span data-ttu-id="87c40-110">Στο αναδυόμενο στοιχείο λεπτομερειών, κάντε κλικ στην επιλογή **Περισσότερες πληροφορίες**.</span><span class="sxs-lookup"><span data-stu-id="87c40-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="87c40-111">Οι πληροφορίες σχετικά με τις ρυθμίσεις κανόνα εισερχομένων εμφανίζονται στο πεδίο **Παράμετροι.**</span><span class="sxs-lookup"><span data-stu-id="87c40-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="87c40-112">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Προσδιορισμός εάν ένας χρήστης δημιούργησε έναν κανόνα εισερχομένων](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="87c40-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
