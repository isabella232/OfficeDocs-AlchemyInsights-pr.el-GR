---
title: Τεχνολογία DLP κανόνα για ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου δεν λειτουργεί
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912097"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="62ba6-102">Προβλήματα με τεχνολογία DLP - ΗΠΑ / Ηνωμένο Βασίλειο Passport αριθμών</span><span class="sxs-lookup"><span data-stu-id="62ba6-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="62ba6-p101">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει ένα **ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου** κατά τη χρήση ενός τύπου ευαίσθητες πληροφορίες DLP σε O365; Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για το τι είναι αναζητούν την πολιτική DLP όταν που αξιολογείται.</span><span class="sxs-lookup"><span data-stu-id="62ba6-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="62ba6-105">Για παράδειγμα, για μια **ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου** πολιτική είναι ρυθμισμένη με επίπεδο εμπιστοσύνης του 75%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης</span><span class="sxs-lookup"><span data-stu-id="62ba6-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="62ba6-106">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Εννέα ψηφία</span><span class="sxs-lookup"><span data-stu-id="62ba6-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="62ba6-107">**[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Εννέα ψηφία διαδοχικά</span><span class="sxs-lookup"><span data-stu-id="62ba6-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="62ba6-108">**[Αθροίσματος ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Όχι, δεν υπάρχει καμία άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="62ba6-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="62ba6-109">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Μια πολιτική DLP είναι 75% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες:</span><span class="sxs-lookup"><span data-stu-id="62ba6-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="62ba6-110">Η συνάρτηση Func_usa_uk_passport εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="62ba6-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="62ba6-111">Μπορείτε να βρείτε μια λέξη-κλειδί από το Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="62ba6-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="62ba6-112">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για την **των η.π.α. / αριθμός διαβατηρίου UK** πολιτικής: αριθμός διαβατηρίου ΗΠΑ 123456789</span><span class="sxs-lookup"><span data-stu-id="62ba6-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="62ba6-113">Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για ένα ΗΠΑ / Ηνωμένο Βασίλειο αριθμός διαβατηρίου που θα εντοπιστούν για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι οι ευαίσθητες πληροφορίες τύπους αναζητήστε η.π.α. / αριθμός διαβατηρίου Ηνωμένο Βασίλειο](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="62ba6-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="62ba6-114">Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="62ba6-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

