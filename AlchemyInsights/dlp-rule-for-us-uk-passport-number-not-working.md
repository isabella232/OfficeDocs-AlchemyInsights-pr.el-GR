---
title: Ο κανόνας DLP για τον αριθμό διαβατηρίων ΗΠΑ/ΗΒ δεν λειτουργεί
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679224"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="1fde5-102">Προβλήματα με τους αριθμούς διαβατηρίων DLP-US/UK</span><span class="sxs-lookup"><span data-stu-id="1fde5-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="1fde5-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="1fde5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1fde5-104">**Θέματα DLP με αριθμούς διαβατηρίων ΗΠΑ/ΗΒ**</span><span class="sxs-lookup"><span data-stu-id="1fde5-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="1fde5-105">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό διαβατηρίου ΗΠΑ/ΗΒ** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών DLP στο O365;</span><span class="sxs-lookup"><span data-stu-id="1fde5-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="1fde5-106">Εάν Ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαιτούμενες πληροφορίες για όσα αναζητά η πολιτική DLP όταν αξιολογείται.</span><span class="sxs-lookup"><span data-stu-id="1fde5-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="1fde5-107">Για παράδειγμα, για μια πολιτική **αριθμών διαβατηρίων ΗΠΑ/ΗΒ** που έχει ρυθμιστεί με επίπεδο αξιοπιστίας 75%, τα παρακάτω αξιολογούνται και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας</span><span class="sxs-lookup"><span data-stu-id="1fde5-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="1fde5-108">**[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Εννέα ψηφία</span><span class="sxs-lookup"><span data-stu-id="1fde5-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="1fde5-109">**[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Εννέα διαδοχικά ψηφία</span><span class="sxs-lookup"><span data-stu-id="1fde5-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="1fde5-110">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="1fde5-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="1fde5-111">**[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, μέσα σε μια εγγύτητα των 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="1fde5-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1fde5-112">Η συνάρτηση Func_usa_uk_passport εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="1fde5-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="1fde5-113">Βρέθηκε μια λέξη-κλειδί από Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="1fde5-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="1fde5-114">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει την πολιτική **αριθμών διαβατηρίων ΗΠΑ/ΗΒ** : αριθμός διαβατηρίου 123456789</span><span class="sxs-lookup"><span data-stu-id="1fde5-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="1fde5-115">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για την ανίχνευση ενός αριθμού διαβατηρίου ΗΠΑ/ΗΒ για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για τον αριθμό διαβατηρίων ΗΠΑ/ΗΒ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="1fde5-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="1fde5-116">Με τη χρήση διαφορετικού ενσωματωμένου τύπου ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="1fde5-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  