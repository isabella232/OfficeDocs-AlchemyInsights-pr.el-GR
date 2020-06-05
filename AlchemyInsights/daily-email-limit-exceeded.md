---
title: Το ημερήσιο όριο ηλεκτρονικού ταχυδρομείου υπερέβη. Η ροή εργασίας έχει ανασταλεί.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580333"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="2c618-103">Το ημερήσιο όριο ηλεκτρονικού ταχυδρομείου έχει ξεπεραστεί.</span><span class="sxs-lookup"><span data-stu-id="2c618-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="2c618-104">Η ροή εργασίας έχει ανασταλεί.</span><span class="sxs-lookup"><span data-stu-id="2c618-104">Workflow is suspended.</span></span>

<span data-ttu-id="2c618-105">Αυτό το σφάλμα μπορεί να ληφθεί στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="2c618-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="2c618-106">Έχετε μια ροή εργασίας στο SharePoint Online που χρησιμοποιεί τον τύπο πλατφόρμας ροής εργασίας του SharePoint 2010 ή του SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="2c618-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="2c618-107">Η ροή εργασίας έχει ρυθμιστεί ώστε να στέλνει ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερους από 200 χρήστες κάθε φορά, περισσότερους από 10.000 παραλήπτες ανά ημέρα ή περισσότερα από 30 μηνύματα ανά λεπτό.</span><span class="sxs-lookup"><span data-stu-id="2c618-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="2c618-108">Όταν εκτελείτε τη ροή εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρείτε την ακόλουθη συμπεριφορά:</span><span class="sxs-lookup"><span data-stu-id="2c618-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="2c618-109">Για μια ροή εργασίας που χρησιμοποιεί τον τύπο πλατφόρμας του SharePoint 2013, μεταβείτε στη σελίδα **Κατάσταση ροής εργασίας.**</span><span class="sxs-lookup"><span data-stu-id="2c618-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="2c618-110">Στη σελίδα Κατάσταση ροής εργασίας, η **εσωτερική κατάσταση** έχει οριστεί σε **"Ξεκίνησε"** και το πλαίσιο πληροφοριών εμφανίζει την ένδειξη **Δεν είναι δυνατή η αποστολή σε παραλήπτη**.</span><span class="sxs-lookup"><span data-stu-id="2c618-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="2c618-111">Για να επιλύσετε αυτό το ζήτημα, ρυθμίστε τις παραμέτρους της ροής εργασίας σας για την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου χωρίς να υπερβαίνετε [τα όρια αποστολέα του Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="2c618-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="2c618-112">Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλτε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα Microsoft 365, μια ομάδα διανομής ή μια ομάδα ασφαλείας με δυνατότητα αλληλογραφίας ή στείλτε το μήνυμα σε λιγότερους από 200 παραλήπτες κάθε φορά.</span><span class="sxs-lookup"><span data-stu-id="2c618-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="2c618-113">Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="2c618-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="2c618-114">Σχετικά θέματα</span><span class="sxs-lookup"><span data-stu-id="2c618-114">Related topics</span></span>
- [<span data-ttu-id="2c618-115">Δημιουργία ροής</span><span class="sxs-lookup"><span data-stu-id="2c618-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2c618-116">Το SharePoint και η ροή</span><span class="sxs-lookup"><span data-stu-id="2c618-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 