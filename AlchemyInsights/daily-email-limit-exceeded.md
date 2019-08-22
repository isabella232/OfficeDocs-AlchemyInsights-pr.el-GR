---
title: Ημερήσια ηλεκτρονικού ταχυδρομείου έγινε υπέρβαση του ορίου. Αναστολή ροής εργασίας.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514452"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="d85bf-103">Υπέρβαση του ορίου ημερήσιων ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="d85bf-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="d85bf-104">Αναστολή ροής εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d85bf-104">Workflow is suspended.</span></span>

<span data-ttu-id="d85bf-105">Αυτό το σφάλμα ενδέχεται να εμφανιστούν στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="d85bf-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="d85bf-106">Μπορείτε να έχετε μια ροή εργασίας σε ηλεκτρονική SharePoint που χρησιμοποιεί το SharePoint 2010 ή τύπος πλατφόρμας ροής εργασίας του SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d85bf-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="d85bf-107">Η ροή εργασίας έχει ρυθμιστεί για να στείλετε ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερα από 200 χρήστες κάθε φορά, περισσότερες από 10.000 παραλήπτες ανά ημέρα είτε περισσότερα από 30 μηνύματα ανά λεπτό.</span><span class="sxs-lookup"><span data-stu-id="d85bf-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="d85bf-108">Κατά την εκτέλεση της ροής εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρήσετε την ακόλουθη συμπεριφορά:</span><span class="sxs-lookup"><span data-stu-id="d85bf-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="d85bf-109">Χρήση του τύπου πλατφόρμα SharePoint 2013 μιας ροής εργασίας, μεταβείτε στη σελίδα " **Κατάσταση ροής εργασίας** ".</span><span class="sxs-lookup"><span data-stu-id="d85bf-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="d85bf-110">Στη σελίδα "Κατάσταση ροής εργασίας", η **Εσωτερική κατάσταση** έχει οριστεί σε **αποτελέσματα**και το παράθυρο πληροφοριών εμφανίζει **δεν είναι δυνατή η αποστολή σε παραλήπτη**.</span><span class="sxs-lookup"><span data-stu-id="d85bf-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="d85bf-111">Για να επιλύσετε αυτό το ζήτημα, ρυθμίστε τις παραμέτρους ροής εργασίας για να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου χωρίς να υπερβαίνουν το [Exchange Online όρια του αποστολέα](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="d85bf-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="d85bf-112">Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλετε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα Office 365, μια ομάδα διανομής ή ομάδα ασφαλείας αλληλογραφίας ενεργοποιημένη ή στείλτε το μήνυμα σε λιγότερα από 200 παραλήπτες ταυτόχρονα.</span><span class="sxs-lookup"><span data-stu-id="d85bf-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="d85bf-113">Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="d85bf-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d85bf-114">Σχετικά θέματα</span><span class="sxs-lookup"><span data-stu-id="d85bf-114">Related topics</span></span>
- [<span data-ttu-id="d85bf-115">Δημιουργία ροής</span><span class="sxs-lookup"><span data-stu-id="d85bf-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d85bf-116">Του SharePoint και ροής</span><span class="sxs-lookup"><span data-stu-id="d85bf-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 