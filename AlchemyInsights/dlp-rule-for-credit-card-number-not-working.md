---
title: Τεχνολογία DLP κανόνα για τον αριθμό της πιστωτικής κάρτας που δεν λειτουργεί
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290654"
---
<span data-ttu-id="e75b4-p101">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει έναν **Αριθμό πιστωτικής κάρτας** , όταν χρησιμοποιείτε έναν τύπο ευαίσθητες πληροφορίες DLP σε O365; Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την ενεργοποίηση της πολιτικής DLP όταν που αξιολογείται. Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** έχει ρυθμιστεί με ένα επίπεδο εμπιστοσύνης του 85%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης:</span><span class="sxs-lookup"><span data-stu-id="e75b4-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="e75b4-105">**[Μορφή:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ψηφία, τα οποία μπορούν να διαμορφωθούν ή μη μορφοποιημένο (dddddddddddddddd) και πρέπει να περάσει τη δοκιμή Luhn.</span><span class="sxs-lookup"><span data-stu-id="e75b4-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="e75b4-106">**[Μοτίβο:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Πολύ περίπλοκη και ισχυρή μοτίβο που εντοπίζει κάρτες από σε όλο τον κόσμο, συμπεριλαμβανομένης της θεώρησης, Mastercard, ανακαλύψετε κάρτα, JCB, American Express, δώρο κάρτες και κάρτες diner κύρια σήματα.</span><span class="sxs-lookup"><span data-stu-id="e75b4-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="e75b4-107">**[Αθροίσματος ελέγχου:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn</span><span class="sxs-lookup"><span data-stu-id="e75b4-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="e75b4-108">**[Ορισμός:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Μια πολιτική DLP είναι 85% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες:</span><span class="sxs-lookup"><span data-stu-id="e75b4-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="e75b4-109">Η συνάρτηση Func_credit_card εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="e75b4-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="e75b4-110">Ένα από τα παρακάτω είναι αληθές:</span><span class="sxs-lookup"><span data-stu-id="e75b4-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="e75b4-111">Μπορείτε να βρείτε μια λέξη-κλειδί από το Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="e75b4-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="e75b4-112">Βρέθηκε μια λέξη-κλειδί από το Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="e75b4-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="e75b4-113">Η συνάρτηση Func_expiration_date βρίσκει μια ημερομηνία στη μορφή ημερομηνίας δεξιά.</span><span class="sxs-lookup"><span data-stu-id="e75b4-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="e75b4-114">Μεταβιβάζει το άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="e75b4-114">The checksum passes</span></span>
    
    <span data-ttu-id="e75b4-115">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για τεχνολογία DLP πολιτική αριθμό πιστωτικής κάρτας:</span><span class="sxs-lookup"><span data-stu-id="e75b4-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="e75b4-116">Θεώρηση: 7352 3952 3647 4485</span><span class="sxs-lookup"><span data-stu-id="e75b4-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="e75b4-117">Λήξη: 2/2009</span><span class="sxs-lookup"><span data-stu-id="e75b4-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="e75b4-118">Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για έναν **Αριθμό πιστωτικής κάρτας** που θα εντοπιστούν για το περιεχόμενο, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών αναζητήστε πιστωτική κάρτα #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="e75b4-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="e75b4-119">Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e75b4-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

