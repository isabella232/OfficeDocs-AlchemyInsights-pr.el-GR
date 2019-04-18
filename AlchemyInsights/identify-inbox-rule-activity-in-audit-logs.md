---
title: Προσδιορισμός δραστηριότητας κανόνα εισερχομένων αρχείων καταγραφής ελέγχου
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909262"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="e5ab4-102">Προσδιορισμός δραστηριότητας κανόνα εισερχομένων αρχείων καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="e5ab4-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="e5ab4-103">Μπορείτε να χρησιμοποιήσετε αναζήτησης αρχείου καταγραφής ελέγχου σε το & ασφαλείας κέντρο συμμόρφωσης, για να προβάλετε συμβάντα κανόνα εισερχομένων (δημιουργία, τροποποίηση και διαγραφή κανόνες εισερχομένων).</span><span class="sxs-lookup"><span data-stu-id="e5ab4-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="e5ab4-104">Συνδεθείτε με το [Κέντρο συμμόρφωσης του Office 365 ασφαλείας &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="e5ab4-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="e5ab4-105">Κάντε κλικ στο κουμπί **Αναζήτηση και έρευνα** και επιλέξτε **Αναζήτηση αρχείου καταγραφής ελέγχου**.</span><span class="sxs-lookup"><span data-stu-id="e5ab4-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="e5ab4-106">Επιλέξτε την περιοχή ημερομηνιών στα πεδία **ημερομηνία έναρξης** και **ημερομηνία λήξης** .</span><span class="sxs-lookup"><span data-stu-id="e5ab4-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="e5ab4-107">Στην περιοχή **Δραστηριότητες του γραμματοκιβωτίου Exchange**, επαληθεύστε το πεδίο **δραστηριοτήτων** έχει οριστεί σε **Δημιουργία InboxRule δημιουργία/τροποποίηση/ενεργοποίηση/απενεργοποίηση κανόνα εισερχομένων**.</span><span class="sxs-lookup"><span data-stu-id="e5ab4-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="e5ab4-108">Κάντε κλικ στο κουμπί **Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="e5ab4-108">Click **Search**.</span></span>

<span data-ttu-id="e5ab4-109">Στα αποτελέσματα, επιλέξτε μια καρτέλα ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="e5ab4-109">In the results, select an audit record.</span></span> <span data-ttu-id="e5ab4-110">Με την Ανάδυση λεπτομέρειες, κάντε κλικ στο κουμπί **Περισσότερες πληροφορίες**.</span><span class="sxs-lookup"><span data-stu-id="e5ab4-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e5ab4-111">Πληροφορίες σχετικά με τις ρυθμίσεις του κανόνα "Εισερχόμενα" εμφανίζεται στο πεδίο " **παράμετροι** ".</span><span class="sxs-lookup"><span data-stu-id="e5ab4-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="e5ab4-112">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Καθορισμός εάν ένας χρήστης δημιούργησε έναν κανόνα εισερχομένων](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="e5ab4-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
