---
title: Κανόνας DLP για τον αριθμό πιστωτικής κάρτας που δεν λειτουργεί
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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932443"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="cca33-102">Ζητήματα DLP με αριθμούς πιστωτικών καρτών</span><span class="sxs-lookup"><span data-stu-id="cca33-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="cca33-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="cca33-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="cca33-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="cca33-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="cca33-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="cca33-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="cca33-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="cca33-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="cca33-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="cca33-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="cca33-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="cca33-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="cca33-109">**Ζητήματα DLP με αριθμούς πιστωτικών καρτών**</span><span class="sxs-lookup"><span data-stu-id="cca33-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="cca33-110">Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό πιστωτικής κάρτας** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365;</span><span class="sxs-lookup"><span data-stu-id="cca33-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="cca33-111">Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για να ενεργοποιήσετε την πολιτική DLP κατά την αξιολόγησή της.</span><span class="sxs-lookup"><span data-stu-id="cca33-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="cca33-112">Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:</span><span class="sxs-lookup"><span data-stu-id="cca33-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="cca33-113">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ψηφία που μπορούν να μορφοποιηθεί ή χωρίς μορφοποίηση (ddddddddddddddddddd) και πρέπει να περάσει τη δοκιμή Luhn.</span><span class="sxs-lookup"><span data-stu-id="cca33-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="cca33-114">**[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Πολύ πολύπλοκο και στιβαρό μοτίβο που ανιχνεύει κάρτες από όλες τις μεγάλες μάρκες σε όλο τον κόσμο, συμπεριλαμβανομένων των Visa, MasterCard, Discover Card, JCB, American Express, δωροκαρτών και καρτών γευματοειδών.</span><span class="sxs-lookup"><span data-stu-id="cca33-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="cca33-115">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn</span><span class="sxs-lookup"><span data-stu-id="cca33-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="cca33-116">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="cca33-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="cca33-117">Η συνάρτηση Func_credit_card εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="cca33-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="cca33-118">Ένα από τα εξής είναι αλήθεια:</span><span class="sxs-lookup"><span data-stu-id="cca33-118">One of the following is true:</span></span>

  - <span data-ttu-id="cca33-119">Βρέθηκε μια λέξη-κλειδί από Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="cca33-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="cca33-120">Βρέθηκε μια λέξη-κλειδί από Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="cca33-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="cca33-121">Η συνάρτηση Func_expiration_date βρίσκει μια ημερομηνία στη σωστή μορφή ημερομηνίας.</span><span class="sxs-lookup"><span data-stu-id="cca33-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="cca33-122">Το άθροισμα ελέγχου περνά</span><span class="sxs-lookup"><span data-stu-id="cca33-122">The checksum passes</span></span>

    <span data-ttu-id="cca33-123">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε για μια πολιτική αριθμού πιστωτικής κάρτας DLP:</span><span class="sxs-lookup"><span data-stu-id="cca33-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="cca33-124">Βίζα: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="cca33-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="cca33-125">Λήξη: 2/2009</span><span class="sxs-lookup"><span data-stu-id="cca33-125">Expires: 2/2009</span></span>

<span data-ttu-id="cca33-126">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό **ενός αριθμού πιστωτικής κάρτας** για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για την πιστωτική κάρτα#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="cca33-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="cca33-127">Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="cca33-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  