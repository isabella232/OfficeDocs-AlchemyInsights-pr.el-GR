---
title: 1332 OWA - κανόνες εισερχομένων δεν εκτελούνται για ένα γραμματοκιβώτιο
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915804"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="c9aee-102">Έναν κανόνα εισερχομένων δεν λειτουργεί όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="c9aee-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="c9aee-103">Επαληθεύστε τις παρακάτω ρυθμίσεις:</span><span class="sxs-lookup"><span data-stu-id="c9aee-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="c9aee-p101">Ένα μήνυμα μπορεί να ανακατευθυνθεί, προωθούνται ή αποστέλλεται απάντηση σε αυτόματα, με βάση κανόνες εισερχομένων μόνο μία φορά. Ανακατεύθυνση κανόνα (έναν κανόνα εισερχομένων ή κανόνα ροής αλληλογραφίας, γνωστή και ως έναν κανόνα μεταφοράς) να προσθέσετε έως και δέκα προώθησης παραλήπτες σε ένα μήνυμα. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Εισερχόμενα εγγραφών, μεταφορά, και τα όρια του κανόνα](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="c9aee-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="c9aee-p102">Κανόνες εισερχομένων δεν λειτουργούν στο γραμματοκιβώτιο εναλλακτική καταγραφή στο χρονικό. Για περισσότερες πληροφορίες σχετικά με το γραμματοκιβώτιο του εναλλακτικού καταγραφή στο χρονικό, δείτε [εναλλακτικό καταγραφή στο χρονικό γραμματοκιβώτιο](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c9aee-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="c9aee-109">Για να διορθώσετε αυτά τα ζητήματα, ανατρέξτε στην ενότητα [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="c9aee-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="c9aee-110">Εάν δεν εφαρμόσετε τα προηγούμενα θέματα, εκτέλεση της διαγνωστικής έκθεσης κανόνα εισερχομένων πριν προωθήσετε το ζήτημα στην υποστήριξη της Microsoft:</span><span class="sxs-lookup"><span data-stu-id="c9aee-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="c9aee-111">Ανοίξτε το γραμματοκιβώτιο στο Outlook στο web και κάντε κλικ στην επιλογή **Ρυθμίσεις** \> **Επιλογές** \> **Οργάνωση ηλεκτρονικού ταχυδρομείου** \> **κανόνες για τα εισερχόμενα**.</span><span class="sxs-lookup"><span data-stu-id="c9aee-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="c9aee-112">Στο κάτω μέρος της σελίδας, κάντε κλικ στο κουμπί **Εάν τους κανόνες σας δεν λειτουργούν κάντε κλικ εδώ για να δημιουργήσετε μια διαγνωστική έκθεση**.</span><span class="sxs-lookup"><span data-stu-id="c9aee-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

