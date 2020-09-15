---
title: Ο κανόνας DLP για τον αριθμό πιστωτικής κάρτας δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679441"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="ae0e8-102">Θέματα DLP με αριθμούς πιστωτικών καρτών</span><span class="sxs-lookup"><span data-stu-id="ae0e8-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="ae0e8-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="ae0e8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ae0e8-104">**Θέματα DLP με αριθμούς πιστωτικών καρτών**</span><span class="sxs-lookup"><span data-stu-id="ae0e8-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="ae0e8-105">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για το περιεχόμενο που περιέχει έναν **αριθμό πιστωτικής κάρτας** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365;</span><span class="sxs-lookup"><span data-stu-id="ae0e8-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ae0e8-106">Εάν Ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαιτούμενες πληροφορίες για να ενεργοποιήσετε την πολιτική DLP όταν αξιολογείται.</span><span class="sxs-lookup"><span data-stu-id="ae0e8-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="ae0e8-107">Για παράδειγμα, για μια **πολιτική πιστωτικής κάρτας** που έχει ρυθμιστεί με επίπεδο αξιοπιστίας 85%, τα παρακάτω αξιολογούνται και πρέπει να ανιχνευθούν για να ενεργοποιείται ο κανόνας:</span><span class="sxs-lookup"><span data-stu-id="ae0e8-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="ae0e8-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 ψηφία τα οποία μπορούν να μορφοποιηθούν ή να μην μορφοποιηθούν (dddddddddddddddd) και πρέπει να περάσουν από τη δοκιμή Luhn.</span><span class="sxs-lookup"><span data-stu-id="ae0e8-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="ae0e8-109">**[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Πολύ περίπλοκο και στιβαρό μοτίβο που εντοπίζει κάρτες από όλες τις μεγάλες μάρκες παγκοσμίως, όπως βίζα, MasterCard, κάρτα Discover, JCB, American Express, δωροκάρτες και κάρτες Diner.</span><span class="sxs-lookup"><span data-stu-id="ae0e8-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="ae0e8-110">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ναι, το άθροισμα ελέγχου Luhn</span><span class="sxs-lookup"><span data-stu-id="ae0e8-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="ae0e8-111">**[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, μέσα σε μια εγγύτητα των 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="ae0e8-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ae0e8-112">Η συνάρτηση Func_credit_card εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="ae0e8-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ae0e8-113">Ισχύει ένα από τα εξής:</span><span class="sxs-lookup"><span data-stu-id="ae0e8-113">One of the following is true:</span></span>

  - <span data-ttu-id="ae0e8-114">Βρέθηκε μια λέξη-κλειδί από Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="ae0e8-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="ae0e8-115">Βρέθηκε μια λέξη-κλειδί από Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="ae0e8-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="ae0e8-116">Η συνάρτηση Func_expiration_date εντοπίζει μια ημερομηνία στη σωστή μορφή ημερομηνίας.</span><span class="sxs-lookup"><span data-stu-id="ae0e8-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="ae0e8-117">Οι φάσεις του αθροίσματος ελέγχου</span><span class="sxs-lookup"><span data-stu-id="ae0e8-117">The checksum passes</span></span>

    <span data-ttu-id="ae0e8-118">Για παράδειγμα, το ακόλουθο δείγμα θα προκαλέσει μια πολιτική αριθμών πιστωτικής κάρτας DLP:</span><span class="sxs-lookup"><span data-stu-id="ae0e8-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="ae0e8-119">Βίζα: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="ae0e8-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="ae0e8-120">Λήγει: 2/2009</span><span class="sxs-lookup"><span data-stu-id="ae0e8-120">Expires: 2/2009</span></span>

<span data-ttu-id="ae0e8-121">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για την ανίχνευση ενός **αριθμού πιστωτικής κάρτας** για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για την πιστωτική κάρτα #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="ae0e8-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="ae0e8-122">Με τη χρήση διαφορετικού ενσωματωμένου τύπου ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="ae0e8-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  