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
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784342"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="0ab19-102">Έναν κανόνα εισερχομένων δεν λειτουργεί όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="0ab19-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="0ab19-103">Επαληθεύστε τις παρακάτω ρυθμίσεις:</span><span class="sxs-lookup"><span data-stu-id="0ab19-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="0ab19-104">Ένα μήνυμα μπορεί να ανακατευθυνθεί, προωθούνται ή αποστέλλεται απάντηση σε αυτόματα, με βάση κανόνες εισερχομένων μόνο μία φορά.</span><span class="sxs-lookup"><span data-stu-id="0ab19-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="0ab19-105">Ανακατεύθυνση κανόνα (έναν κανόνα εισερχομένων ή κανόνα ροής αλληλογραφίας, γνωστή και ως έναν κανόνα μεταφοράς) να προσθέσετε έως και δέκα προώθησης παραλήπτες σε ένα μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="0ab19-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="0ab19-106">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Εισερχόμενα εγγραφών, μεταφορά, και τα όρια του κανόνα](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="0ab19-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="0ab19-107">Κανόνες εισερχομένων δεν λειτουργούν στο γραμματοκιβώτιο εναλλακτική καταγραφή στο χρονικό.</span><span class="sxs-lookup"><span data-stu-id="0ab19-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="0ab19-108">Για περισσότερες πληροφορίες σχετικά με το γραμματοκιβώτιο του εναλλακτικού καταγραφή στο χρονικό, δείτε [εναλλακτικό καταγραφή στο χρονικό γραμματοκιβώτιο](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="0ab19-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="0ab19-109">Για να διορθώσετε αυτά τα ζητήματα, ανατρέξτε στην ενότητα [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="0ab19-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="0ab19-110">Εάν δεν εφαρμόσετε τα προηγούμενα θέματα, εκτέλεση της διαγνωστικής έκθεσης κανόνα εισερχομένων πριν προωθήσετε το ζήτημα στην υποστήριξη της Microsoft:</span><span class="sxs-lookup"><span data-stu-id="0ab19-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="0ab19-111">Ανοίξτε το γραμματοκιβώτιο στο Outlook στο web και κάντε κλικ στην επιλογή **Ρυθμίσεις** \> **Επιλογές** \> **Οργάνωση ηλεκτρονικού ταχυδρομείου** \> **κανόνες για τα εισερχόμενα**.</span><span class="sxs-lookup"><span data-stu-id="0ab19-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="0ab19-112">Στο κάτω μέρος της σελίδας, κάντε κλικ στο κουμπί **Εάν τους κανόνες σας δεν λειτουργούν κάντε κλικ εδώ για να δημιουργήσετε μια διαγνωστική έκθεση**.</span><span class="sxs-lookup"><span data-stu-id="0ab19-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

