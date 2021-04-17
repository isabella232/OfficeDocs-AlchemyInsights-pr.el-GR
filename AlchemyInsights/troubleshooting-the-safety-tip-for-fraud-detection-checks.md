---
title: Αντιμετώπιση προβλημάτων με τη συμβουλή ασφαλείας για ελέγχους εντοπισμού απάτης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834731"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="32556-102">Αντιμετώπιση προβλημάτων με τη συμβουλή ασφαλείας για ελέγχους εντοπισμού απάτης</span><span class="sxs-lookup"><span data-stu-id="32556-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="32556-103">Εάν εμφανίζεται μια συμβουλή ασφαλείας που αναφέρει ότι "Ο αποστολέας απέτυχε στους ελέγχους εντοπισμού απάτης και ενδέχεται να μην είναι αυτός που φαίνεται", τότε ο αποστολέας απέτυχε να περάσει ελέγχους ελέγχου ταυτότητας DKIM ή SPF.</span><span class="sxs-lookup"><span data-stu-id="32556-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="32556-104">Η καλύτερη μέθοδος για την επίλυση αυτού του προβλήματος είναι να εξουσιοδοτήσει τον αποστολέα.</span><span class="sxs-lookup"><span data-stu-id="32556-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="32556-105">Εάν ο αποστολέας στέλνει εκ μέρους σας, πρέπει να τον εξουσιοδοτήσετε προσθέτοντας τη διεύθυνση IP του αποστολέα στην εγγραφή SPF.</span><span class="sxs-lookup"><span data-stu-id="32556-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="32556-106">Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων με την κόκκινη (ύποπτη) συμβουλή ασφαλείας για ελέγχους εντοπισμού απάτης](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="32556-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="32556-107">Ακολουθούν ορισμένες άλλες συνδέσεις που μπορούν να σας βοηθήσουν:</span><span class="sxs-lookup"><span data-stu-id="32556-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="32556-108">Πώς η Microsoft χρησιμοποιεί το πλαίσιο πολιτικής αποστολέα (SPF) για την αποτροπή πλαστογράφησης</span><span class="sxs-lookup"><span data-stu-id="32556-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="32556-109">Ρύθμιση SPF για την αποτροπή πλαστογράφησης</span><span class="sxs-lookup"><span data-stu-id="32556-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
