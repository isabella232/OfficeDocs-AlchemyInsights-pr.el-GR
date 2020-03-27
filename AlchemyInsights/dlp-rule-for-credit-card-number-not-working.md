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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977198"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="10548-102">Ζητήματα DLP με αριθμούς πιστωτικών καρτών</span><span class="sxs-lookup"><span data-stu-id="10548-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="10548-103">**Σημαντικό:** Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες – Επισκεφθείτε [τις προσωρινές προσαρμογές δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="10548-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="10548-104">**Ζητήματα DLP με αριθμούς πιστωτικών καρτών**</span><span class="sxs-lookup"><span data-stu-id="10548-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="10548-105">Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό πιστωτικής κάρτας** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365;</span><span class="sxs-lookup"><span data-stu-id="10548-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="10548-106">Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για να ενεργοποιήσετε την πολιτική DLP κατά την αξιολόγησή της.</span><span class="sxs-lookup"><span data-stu-id="10548-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="10548-107">Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:</span><span class="sxs-lookup"><span data-stu-id="10548-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="10548-108">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ψηφία που μπορούν να μορφοποιηθεί ή χωρίς μορφοποίηση (ddddddddddddddddddd) και πρέπει να περάσει τη δοκιμή Luhn.</span><span class="sxs-lookup"><span data-stu-id="10548-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="10548-109">**[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Πολύ πολύπλοκο και στιβαρό μοτίβο που ανιχνεύει κάρτες από όλες τις μεγάλες μάρκες σε όλο τον κόσμο, συμπεριλαμβανομένων των Visa, MasterCard, Discover Card, JCB, American Express, δωροκαρτών και καρτών γευματοειδών.</span><span class="sxs-lookup"><span data-stu-id="10548-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="10548-110">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn</span><span class="sxs-lookup"><span data-stu-id="10548-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="10548-111">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="10548-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="10548-112">Η συνάρτηση Func_credit_card εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="10548-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="10548-113">Ένα από τα εξής είναι αλήθεια:</span><span class="sxs-lookup"><span data-stu-id="10548-113">One of the following is true:</span></span>

  - <span data-ttu-id="10548-114">Βρέθηκε μια λέξη-κλειδί από Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="10548-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="10548-115">Βρέθηκε μια λέξη-κλειδί από Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="10548-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="10548-116">Η συνάρτηση Func_expiration_date βρίσκει μια ημερομηνία στη σωστή μορφή ημερομηνίας.</span><span class="sxs-lookup"><span data-stu-id="10548-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="10548-117">Το άθροισμα ελέγχου περνά</span><span class="sxs-lookup"><span data-stu-id="10548-117">The checksum passes</span></span>

    <span data-ttu-id="10548-118">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε για μια πολιτική αριθμού πιστωτικής κάρτας DLP:</span><span class="sxs-lookup"><span data-stu-id="10548-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="10548-119">Βίζα: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="10548-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="10548-120">Λήξη: 2/2009</span><span class="sxs-lookup"><span data-stu-id="10548-120">Expires: 2/2009</span></span>

<span data-ttu-id="10548-121">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό **ενός αριθμού πιστωτικής κάρτας** για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για την πιστωτική κάρτα#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="10548-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="10548-122">Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="10548-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  