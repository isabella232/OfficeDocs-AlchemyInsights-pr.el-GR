---
title: Ανεπιθύμητη αλληλογραφία-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717325"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="8f2c9-102">Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23</span><span class="sxs-lookup"><span data-stu-id="8f2c9-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="8f2c9-103">Επαληθεύστε την εγγραφή DNS SPF για τον τομέα σας σε έναν δημόσια διαθέσιμο έλεγχο εγγραφής SPF ή DNS στο Web.</span><span class="sxs-lookup"><span data-stu-id="8f2c9-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="8f2c9-104">Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν αναγνωρίστηκε ως ανεπιθύμητη αλληλογραφία από τη Microsoft και ότι δρομολογείται μέσω του [χώρου συγκέντρωσης παράδοσης υψηλού κινδύνου](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="8f2c9-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="8f2c9-105">Τα μηνύματα στο χώρο συγκέντρωσης παράδοσης υψηλού κινδύνου δεν μεταβιβάζουν τους ελέγχους SPF και, επομένως, δεν θα γίνονται δεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="8f2c9-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="8f2c9-106">Εάν το πρόβλημα δεν επιλυθεί, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο επιχειρείτε να στείλετε μήνυμα ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="8f2c9-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="8f2c9-107">Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα αναπήδησης.</span><span class="sxs-lookup"><span data-stu-id="8f2c9-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="8f2c9-108">Η υποστήριξη της Microsoft ενδέχεται να μην είναι σε θέση να σας βοηθήσει περαιτέρω.</span><span class="sxs-lookup"><span data-stu-id="8f2c9-108">Microsoft support may not be able to assist further.</span></span>
