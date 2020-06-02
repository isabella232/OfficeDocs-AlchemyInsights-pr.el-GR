---
title: Αντιμετώπιση προβλημάτων του άκρου ασφαλείας για ελέγχους εντοπισμού απάτης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504983"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="0e746-102">Αντιμετώπιση προβλημάτων του άκρου ασφαλείας για ελέγχους εντοπισμού απάτης</span><span class="sxs-lookup"><span data-stu-id="0e746-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="0e746-103">Εάν παίρνετε μια συμβουλή ασφαλείας που λέει "Ο αποστολέας απέτυχε ελέγχους ανίχνευσης απάτης μας και δεν μπορεί να είναι αυτό που φαίνεται να είναι", τότε ο αποστολέας απέτυχε να περάσει είτε DKIM ή SPF ελέγχους ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="0e746-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="0e746-104">Η καλύτερη μέθοδος για την επίλυση αυτού είναι ο αποστολέας να εξουσιοδοτήσει τον εαυτό του.</span><span class="sxs-lookup"><span data-stu-id="0e746-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="0e746-105">Εάν ο αποστολέας στέλνει για λογαριασμό σας, πρέπει να τον εξουσιοδοτήσετε προσθέτοντας τη διεύθυνση IP του αποστολέα στην εγγραφή SPF.</span><span class="sxs-lookup"><span data-stu-id="0e746-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="0e746-106">Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων της κόκκινης (ύποπτης) συμβουλής ασφαλείας για ελέγχους εντοπισμού απάτης](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="0e746-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="0e746-107">Ακολουθούν ορισμένες άλλες συνδέσεις που μπορούν να σας βοηθήσουν:</span><span class="sxs-lookup"><span data-stu-id="0e746-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="0e746-108">Τρόπος με τον οποίο η Microsoft χρησιμοποιεί το πλαίσιο πολιτικής αποστολέα (SPF) για την αποτροπή πλαστογραφίας</span><span class="sxs-lookup"><span data-stu-id="0e746-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="0e746-109">Ρύθμιση spf για την αποτροπή πλαστοπλασιασμός</span><span class="sxs-lookup"><span data-stu-id="0e746-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
