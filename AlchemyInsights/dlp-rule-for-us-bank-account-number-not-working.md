---
title: Τεχνολογία DLP κανόνα για ΕΜΆΣ αριθμός τραπεζικού λογαριασμού δεν λειτουργεί
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9fd5d4736c5209f85e235dc6a0846f65f1b5f624
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656999"
---
<span data-ttu-id="8455b-p101">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει έναν **Αριθμό τραπεζικού λογαριασμού η.π.α.** κατά τη χρήση ενός τύπου ευαίσθητες πληροφορίες DLP σε O365; Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για το τι είναι αναζητούν την πολιτική DLP όταν που αξιολογείται.</span><span class="sxs-lookup"><span data-stu-id="8455b-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="8455b-104">Για παράδειγμα, για μια πολιτική **Η.π.α. αριθμός τραπεζικού λογαριασμού** που έχει ρυθμιστεί με ένα επίπεδο εμπιστοσύνης του 85%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης:</span><span class="sxs-lookup"><span data-stu-id="8455b-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="8455b-105">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 ψηφία</span><span class="sxs-lookup"><span data-stu-id="8455b-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="8455b-106">**[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 συνεχείς αριθμούς.</span><span class="sxs-lookup"><span data-stu-id="8455b-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="8455b-107">**[Αθροίσματος ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Όχι, δεν υπάρχει καμία άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="8455b-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="8455b-108">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Μια πολιτική DLP είναι 75% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες:</span><span class="sxs-lookup"><span data-stu-id="8455b-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="8455b-109">Η κανονική έκφραση Regex_usa_bank_account_number εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο</span><span class="sxs-lookup"><span data-stu-id="8455b-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="8455b-110">Μπορείτε να βρείτε μια λέξη-κλειδί από το Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="8455b-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="8455b-111">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για την πολιτική **Των η.π.α. αριθμός τραπεζικού λογαριασμού** : λογαριασμός όψεως 78344011</span><span class="sxs-lookup"><span data-stu-id="8455b-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="8455b-112">Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για έναν **Αριθμό τραπεζικού λογαριασμού η.π.α.** έως ότου ανιχνευθούν για το περιεχόμενο, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών αναζήτηση για τον αριθμό τραπεζικού λογαριασμού η.π.α.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="8455b-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="8455b-113">Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="8455b-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

