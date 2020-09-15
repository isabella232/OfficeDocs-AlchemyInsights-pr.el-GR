---
title: Αντιμετώπιση προβλημάτων του άκρου ασφαλείας για τους ελέγχους εντοπισμού απάτης
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658410"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="86b9c-102">Αντιμετώπιση προβλημάτων του άκρου ασφαλείας για τους ελέγχους εντοπισμού απάτης</span><span class="sxs-lookup"><span data-stu-id="86b9c-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="86b9c-103">Εάν λαμβάνετε μια συμβουλή ασφαλείας που αναφέρει ότι "ο αποστολέας απέτυχε στους ελέγχους εντοπισμού απάτης και μπορεί να μην είναι αυτός που φαίνεται να είναι", τότε ο αποστολέας δεν κατάφερε να διαβιβάσει τους ελέγχους ελέγχου ταυτότητας DKIM ή SPF.</span><span class="sxs-lookup"><span data-stu-id="86b9c-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="86b9c-104">Η καλύτερη μέθοδος για να επιλυθεί αυτό είναι να εξουσιοδοτηθεί ο αποστολέας.</span><span class="sxs-lookup"><span data-stu-id="86b9c-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="86b9c-105">Εάν ο αποστολέας στέλνει για λογαριασμό σας, πρέπει να τον εξουσιοδοτήσετε προσθέτοντας τη διεύθυνση IP του αποστολέα στην εγγραφή SPF.</span><span class="sxs-lookup"><span data-stu-id="86b9c-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="86b9c-106">Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων με την κόκκινη (ύποπτη) συμβουλή ασφαλείας για τον έλεγχο ανίχνευσης απάτης](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="86b9c-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="86b9c-107">Ακολουθούν ορισμένες άλλες συνδέσεις που μπορούν να σας βοηθήσουν:</span><span class="sxs-lookup"><span data-stu-id="86b9c-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="86b9c-108">Πώς η Microsoft χρησιμοποιεί το πλαίσιο πολιτικής αποστολέα (SPF) για την αποτροπή της πλαστογράφησης</span><span class="sxs-lookup"><span data-stu-id="86b9c-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="86b9c-109">Ρύθμιση SPF για αποτροπή της πλαστογράφησης</span><span class="sxs-lookup"><span data-stu-id="86b9c-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
