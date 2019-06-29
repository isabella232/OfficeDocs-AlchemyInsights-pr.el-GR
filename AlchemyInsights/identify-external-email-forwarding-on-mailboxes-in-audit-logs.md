---
title: Προσδιορισμός προώθησης ηλεκτρονικού ταχυδρομείου εξωτερικών σε γραμματοκιβώτια στα αρχεία καταγραφής ελέγχου
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383097"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c0460-102">Προσδιορισμός κατά τη ρύθμιση παραμέτρων σε γραμματοκιβώτια προώθησης ηλεκτρονικού ταχυδρομείου εξωτερικό</span><span class="sxs-lookup"><span data-stu-id="c0460-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c0460-103">Όταν ο χρήστης ρυθμίζει τις παραμέτρους προώθησης εξωτερικό μήνυμα ηλεκτρονικού ταχυδρομείου σε ένα γραμματοκιβώτιο, ελέγχεται η δραστηριότητα ως μέρος της το cmdlet **Σύνολο γραμματοκιβωτίου** .</span><span class="sxs-lookup"><span data-stu-id="c0460-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c0460-104">Μπορείτε να δείτε τη δραστηριότητα χρησιμοποιώντας αναζήτηση αρχείου καταγραφής ελέγχου στο το & ασφαλείας κέντρο συμμόρφωσης.</span><span class="sxs-lookup"><span data-stu-id="c0460-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c0460-105">Συνδεθείτε με το [Κέντρο συμμόρφωσης του Office 365 ασφαλείας &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c0460-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c0460-106">Κάντε κλικ στο κουμπί **Αναζήτηση και έρευνα** και επιλέξτε **Αναζήτηση αρχείου καταγραφής ελέγχου**.</span><span class="sxs-lookup"><span data-stu-id="c0460-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c0460-107">Επιλέξτε την περιοχή ημερομηνιών στα πεδία **ημερομηνία έναρξης** και **ημερομηνία λήξης** .</span><span class="sxs-lookup"><span data-stu-id="c0460-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c0460-108">Δεν χρειάζεται να καθορίσετε ένα όνομα χρήστη.</span><span class="sxs-lookup"><span data-stu-id="c0460-108">You don't need to specify a username.</span></span> <span data-ttu-id="c0460-109">Επαληθεύστε το πεδίο " **δραστηριότητες** " έχει οριστεί σε **Εμφάνιση αποτελεσμάτων για όλες τις δραστηριότητες**.</span><span class="sxs-lookup"><span data-stu-id="c0460-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c0460-110">Κάντε κλικ στο κουμπί **Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="c0460-110">Click **Search**.</span></span>

<span data-ttu-id="c0460-111">Στα αποτελέσματα, **Αποτελέσματα του φίλτρου** , κάντε κλικ και πληκτρολογήστε **Σύνολο γραμματοκιβωτίου** στο πλαίσιο φίλτρο δραστηριότητας.</span><span class="sxs-lookup"><span data-stu-id="c0460-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c0460-112">Επιλέξτε μια καρτέλα ελέγχου στα αποτελέσματα.</span><span class="sxs-lookup"><span data-stu-id="c0460-112">Select an audit record in the results.</span></span> <span data-ttu-id="c0460-113">Με την Ανάδυση **Λεπτομέρειες** , κάντε κλικ στο κουμπί **περισσότερες πληροφορίες**.</span><span class="sxs-lookup"><span data-stu-id="c0460-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c0460-114">Θα πρέπει να ελέγχετε τις λεπτομέρειες κάθε ελέγχου καρτέλας για να προσδιορίσετε εάν η δραστηριότητα έχει σχέση με ηλεκτρονικό ταχυδρομείο προώθησης.</span><span class="sxs-lookup"><span data-stu-id="c0460-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c0460-115">**ObjectId**: Η τιμή το ψευδώνυμο του γραμματοκιβωτίου που έχει τροποποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="c0460-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c0460-116">**Παράμετροι**: _ForwardingSmtpAddress_ υποδεικνύει τη διεύθυνση ηλεκτρονικού ταχυδρομείου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="c0460-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c0460-117">**Αναγνωριστικό χρήστη**: Ο χρήστης που έχει ρυθμιστεί προώθησης ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο στο πεδίο **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="c0460-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c0460-118">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Καθορισμός που εγκατέστησε ηλεκτρονικού ταχυδρομείου προώθησης για ένα γραμματοκιβώτιο](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c0460-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
