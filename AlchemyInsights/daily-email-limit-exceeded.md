---
title: Έγινε υπέρβαση του ημερήσιου ορίου ηλεκτρονικού ταχυδρομείου. Η ροή εργασίας έχει ανασταλεί.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053117"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="a45c9-103">Έγινε υπέρβαση του ορίου ημερήσιων μηνυμάτων ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="a45c9-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="a45c9-104">Η ροή εργασίας έχει ανασταλεί.</span><span class="sxs-lookup"><span data-stu-id="a45c9-104">Workflow is suspended.</span></span>

<span data-ttu-id="a45c9-105">Αυτό το σφάλμα μπορεί να παραληφθεί στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="a45c9-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="a45c9-106">Έχετε μια ροή εργασίας στο SharePoint Online που χρησιμοποιεί το SharePoint 2010 ή τον τύπο πλατφόρμας ροής εργασίας του SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="a45c9-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="a45c9-107">Η ροή εργασίας έχει ρυθμιστεί για να στείλετε ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερους από 200 χρήστες κάθε φορά, περισσότερους από 10.000 παραλήπτες ανά ημέρα, ή περισσότερα από 30 μηνύματα ανά λεπτό.</span><span class="sxs-lookup"><span data-stu-id="a45c9-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="a45c9-108">Όταν εκτελείτε τη ροή εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρείτε την ακόλουθη συμπεριφορά:</span><span class="sxs-lookup"><span data-stu-id="a45c9-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="a45c9-109">Για μια ροή εργασίας χρησιμοποιώντας τον τύπο πλατφόρμας του SharePoint 2013, μεταβείτε στη σελίδα **κατάσταση ροής εργασίας** .</span><span class="sxs-lookup"><span data-stu-id="a45c9-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="a45c9-110">Στη σελίδα "κατάσταση ροής εργασίας", η **εσωτερική κατάσταση** έχει οριστεί σε **Έναρξη**και το πλαίσιο πληροφοριών εμφανίζει **δεν είναι δυνατή η αποστολή σε έναν παραλήπτη**.</span><span class="sxs-lookup"><span data-stu-id="a45c9-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="a45c9-111">Για να επιλύσετε αυτό το ζήτημα, ρυθμίστε τη ροή εργασίας σας για να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου χωρίς να υπερβαίνει τα [όρια αποστολέα του Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="a45c9-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="a45c9-112">Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλτε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα Office 365, μια ομάδα διανομής ή μια υπηρεσία ασφαλείας με δυνατότητα αλληλογραφίας ή στείλτε το μήνυμά σας σε λιγότερους από 200 παραλήπτες κάθε φορά.</span><span class="sxs-lookup"><span data-stu-id="a45c9-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="a45c9-113">Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="a45c9-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="a45c9-114">Σχετικά θέματα</span><span class="sxs-lookup"><span data-stu-id="a45c9-114">Related topics</span></span>
- [<span data-ttu-id="a45c9-115">Δημιουργία ροής</span><span class="sxs-lookup"><span data-stu-id="a45c9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a45c9-116">SharePoint και ροή</span><span class="sxs-lookup"><span data-stu-id="a45c9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 