---
title: Ξεκινήστε με το SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766891"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="86866-102">Ροές εργασίας στο SharePoint</span><span class="sxs-lookup"><span data-stu-id="86866-102">Workflows in SharePoint</span></span>

<span data-ttu-id="86866-103">Εάν οι ροές εργασίας του SharePoint δεν στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου, ο οργανισμός σας ενδέχεται να έχει αντιμετωπίσει τα όρια αποστολέα του Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="86866-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="86866-104">Το μήνυμα λάθους "ροή εργασίας είναι αναστέλλεται" ενδέχεται να προκύψει, εάν έχετε ένα από τα ακόλουθα στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="86866-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="86866-105">Έχετε μια ροή εργασίας στο SharePoint Online που χρησιμοποιεί το SharePoint 2010 ή τον τύπο πλατφόρμας ροής εργασίας του SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="86866-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="86866-106">Η ροή εργασίας έχει ρυθμιστεί για να στείλετε ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερους από 200 χρήστες κάθε φορά, περισσότερους από 10.000 παραλήπτες ανά ημέρα, ή περισσότερα από 30 μηνύματα ανά λεπτό.</span><span class="sxs-lookup"><span data-stu-id="86866-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="86866-107">Όταν εκτελείτε τη ροή εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρείτε το μήνυμα λάθους, εσωτερική κατάσταση έχει οριστεί σε αναστολή ή δεν είναι δυνατή η αποστολή σε έναν παραλήπτη εμφανίζεται.</span><span class="sxs-lookup"><span data-stu-id="86866-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="86866-108">Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="86866-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

