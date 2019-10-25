---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682146"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f65f0-102">Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23</span><span class="sxs-lookup"><span data-stu-id="f65f0-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f65f0-103">Επαληθεύστε την εγγραφή SPF DNS για τον τομέα σας σε ένα δημόσια διαθέσιμο SPF ή ελεγκτή εγγραφών DNS στο Web.</span><span class="sxs-lookup"><span data-stu-id="f65f0-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f65f0-104">Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν αναγνωρίστηκε ως ανεπιθύμητο από το Office 365 και δρομολογείται μέσω του [χώρου συγκέντρωσης υψηλών κινδύνων](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="f65f0-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f65f0-105">Τα μηνύματα στο χώρο συγκέντρωσης υψηλού κινδύνου δεν περνούν τους ελέγχους SPF και επομένως δεν θα γίνουν αποδεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="f65f0-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f65f0-106">Εάν το πρόβλημα επιμείνει, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο επιχειρείτε να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="f65f0-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f65f0-107">Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα ανάκλασης.</span><span class="sxs-lookup"><span data-stu-id="f65f0-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="f65f0-108">Η υποστήριξη του Office 365 ενδέχεται να μην μπορεί να βοηθήσει περαιτέρω.</span><span class="sxs-lookup"><span data-stu-id="f65f0-108">Office 365 support may not be able to assist further.</span></span>