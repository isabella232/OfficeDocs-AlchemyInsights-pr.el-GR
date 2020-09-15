---
title: Γρήγορα αποτελέσματα με το SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700707"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="2f6c3-102">Ροές εργασιών στο SharePoint</span><span class="sxs-lookup"><span data-stu-id="2f6c3-102">Workflows in SharePoint</span></span>

<span data-ttu-id="2f6c3-103">Εάν οι ροές εργασίας του SharePoint δεν στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου, η εταιρεία σας ενδέχεται να αντιμετώπισε τα όρια αποστολέα του Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2f6c3-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="2f6c3-104">Το μήνυμα σφάλματος "η ροή εργασίας έχει ανασταλεί" μπορεί να προκύψει εάν έχετε ένα από τα παρακάτω στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="2f6c3-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="2f6c3-105">Έχετε μια ροή εργασίας στο SharePoint Online που χρησιμοποιεί τον τύπο πλατφόρμας ροής εργασίας του SharePoint 2010 ή του SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="2f6c3-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="2f6c3-106">Η ροή εργασίας έχει ρυθμιστεί ώστε να στέλνει ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερους από 200 χρήστες κάθε φορά, περισσότερους από 10.000 παραλήπτες ανά ημέρα ή περισσότερα από 30 μηνύματα ανά λεπτό.</span><span class="sxs-lookup"><span data-stu-id="2f6c3-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="2f6c3-107">Όταν εκτελείτε τη ροή εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρείτε ότι εμφανίζεται το μήνυμα σφάλματος, η εσωτερική κατάσταση έχει τεθεί σε αναστολή ή δεν είναι δυνατή η αποστολή σε έναν παραλήπτη.</span><span class="sxs-lookup"><span data-stu-id="2f6c3-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="2f6c3-108">Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="2f6c3-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

