---
title: Αναγνώριση δραστηριότητας κανόνα εισερχομένων σε αρχεία καταγραφής ελέγχου
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779051"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="cc5e5-102">Αναγνώριση δραστηριότητας κανόνα εισερχομένων σε αρχεία καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="cc5e5-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="cc5e5-103">Μπορείτε να χρησιμοποιήσετε την αναζήτηση του αρχείου καταγραφής ελέγχου στο κέντρο συμμόρφωσης του Microsoft 365 Security & για να προβάλετε συμβάντα κανόνων εισερχομένων (δημιουργία, τροποποίηση και διαγραφή κανόνων εισερχομένων).</span><span class="sxs-lookup"><span data-stu-id="cc5e5-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="cc5e5-104">Συνδεθείτε στο [Κέντρο συμμόρφωσης & ασφαλείας του Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="cc5e5-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="cc5e5-105">Μεταβείτε στη σελίδα **Search**αναζήτησης του  >  **αρχείου καταγραφής ελέγχου** αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="cc5e5-106">Επιλέξτε την περιοχή ημερομηνιών στα πεδία ημερομηνία **έναρξης** και **ημερομηνία λήξης** .</span><span class="sxs-lookup"><span data-stu-id="cc5e5-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="cc5e5-107">Στην περιοχή **δραστηριότητες γραμματοκιβωτίου του Exchange**, επαληθεύστε ότι το πεδίο **δραστηριότητες** έχει την τιμή **Νέα-InboxRule Create/Modify/enable/disable Inbox Rule**.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="cc5e5-108">Κάντε κλικ στην επιλογή **Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-108">Click **Search**.</span></span>

<span data-ttu-id="cc5e5-109">Στα αποτελέσματα, επιλέξτε μια εγγραφή ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-109">In the results, select an audit record.</span></span> <span data-ttu-id="cc5e5-110">Στο αναδυόμενο στοιχείο λεπτομερειών, κάντε κλικ στην επιλογή **περισσότερες πληροφορίες**.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="cc5e5-111">Οι πληροφορίες σχετικά με τις ρυθμίσεις του κανόνα εισερχομένων εμφανίζονται στο πεδίο **Παράμετροι** .</span><span class="sxs-lookup"><span data-stu-id="cc5e5-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="cc5e5-112">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Καθορισμός εάν ένας χρήστης δημιούργησε έναν κανόνα εισερχομένων](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="cc5e5-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
