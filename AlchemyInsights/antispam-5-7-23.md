---
title: Αντιανεπιθύμητη αλληλογραφία - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676497"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="9d5ca-102">Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23</span><span class="sxs-lookup"><span data-stu-id="9d5ca-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="9d5ca-103">Επαληθεύστε την εγγραφή SPF DNS για τον τομέα σας σε έναν δημόσια διαθέσιμο έλεγχο εγγραφής SPF ή DNS στο web.</span><span class="sxs-lookup"><span data-stu-id="9d5ca-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="9d5ca-104">Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν προσδιορίστηκε ως ανεπιθύμητο από τη Microsoft και δρομολογήθηκε μέσω του [χώρου συγκέντρωσης παράδοσης υψηλού κινδύνου](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="9d5ca-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="9d5ca-105">Τα μηνύματα στο χώρο συγκέντρωσης παράδοσης υψηλού κινδύνου δεν θα περάσουν τους ελέγχους SPF και, επομένως, δεν θα γίνονται αποδεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="9d5ca-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="9d5ca-106">Εάν το πρόβλημα παραμένει, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο προσπαθείτε να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="9d5ca-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="9d5ca-107">Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα αναπήδησης.</span><span class="sxs-lookup"><span data-stu-id="9d5ca-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="9d5ca-108">Η υποστήριξη της Microsoft ενδέχεται να μην είναι σε θέση να βοηθήσει περαιτέρω.</span><span class="sxs-lookup"><span data-stu-id="9d5ca-108">Microsoft support may not be able to assist further.</span></span>
