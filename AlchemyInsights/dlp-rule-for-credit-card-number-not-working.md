---
title: Τεχνολογία DLP κανόνα για τον αριθμό της πιστωτικής κάρτας που δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389577"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="b962e-102">Τεχνολογία DLP ζητήματα με αριθμούς πιστωτικών καρτών</span><span class="sxs-lookup"><span data-stu-id="b962e-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="b962e-103">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει έναν **Αριθμό πιστωτικής κάρτας** , όταν χρησιμοποιείτε έναν τύπο ευαίσθητες πληροφορίες DLP σε O365;</span><span class="sxs-lookup"><span data-stu-id="b962e-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b962e-104">Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την ενεργοποίηση της πολιτικής DLP όταν που αξιολογείται.</span><span class="sxs-lookup"><span data-stu-id="b962e-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="b962e-105">Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** έχει ρυθμιστεί με ένα επίπεδο εμπιστοσύνης του 85%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης:</span><span class="sxs-lookup"><span data-stu-id="b962e-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b962e-106">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ψηφία, τα οποία μπορούν να διαμορφωθούν ή μη μορφοποιημένο (dddddddddddddddd) και πρέπει να περάσει τη δοκιμή Luhn.</span><span class="sxs-lookup"><span data-stu-id="b962e-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="b962e-107">**[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Πολύ περίπλοκη και ισχυρή μοτίβο που εντοπίζει κάρτες από σε όλο τον κόσμο, συμπεριλαμβανομένης της θεώρησης, MasterCard, ανακαλύψετε κάρτα, JCB, American Express, δώρο κάρτες και κάρτες diner κύρια σήματα.</span><span class="sxs-lookup"><span data-stu-id="b962e-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="b962e-108">**[Αθροίσματος ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn</span><span class="sxs-lookup"><span data-stu-id="b962e-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="b962e-109">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Μια πολιτική DLP είναι 85% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες:</span><span class="sxs-lookup"><span data-stu-id="b962e-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b962e-110">Η συνάρτηση Func_credit_card εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="b962e-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b962e-111">Ένα από τα παρακάτω είναι αληθές:</span><span class="sxs-lookup"><span data-stu-id="b962e-111">One of the following is true:</span></span>

  - <span data-ttu-id="b962e-112">Μπορείτε να βρείτε μια λέξη-κλειδί από το Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="b962e-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="b962e-113">Βρέθηκε μια λέξη-κλειδί από το Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="b962e-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="b962e-114">Η συνάρτηση Func_expiration_date βρίσκει μια ημερομηνία στη μορφή ημερομηνίας δεξιά.</span><span class="sxs-lookup"><span data-stu-id="b962e-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="b962e-115">Μεταβιβάζει το άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="b962e-115">The checksum passes</span></span>

    <span data-ttu-id="b962e-116">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για τεχνολογία DLP πολιτική αριθμό πιστωτικής κάρτας:</span><span class="sxs-lookup"><span data-stu-id="b962e-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="b962e-117">Θεώρηση: 7352 3952 3647 4485</span><span class="sxs-lookup"><span data-stu-id="b962e-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="b962e-118">Λήξη: 2/2009</span><span class="sxs-lookup"><span data-stu-id="b962e-118">Expires: 2/2009</span></span>

<span data-ttu-id="b962e-119">Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για έναν **Αριθμό πιστωτικής κάρτας** που θα εντοπιστούν για το περιεχόμενο, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών αναζητήστε πιστωτική κάρτα #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="b962e-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="b962e-120">Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b962e-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  