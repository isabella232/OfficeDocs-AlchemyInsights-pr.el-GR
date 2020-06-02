---
title: Κανόνας DLP για τον αριθμό τραπεζικού λογαριασμού των ΗΠΑ που δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507334"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="b2970-102">Ζητήματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ</span><span class="sxs-lookup"><span data-stu-id="b2970-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="b2970-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="b2970-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b2970-104">**Ζητήματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ**</span><span class="sxs-lookup"><span data-stu-id="b2970-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="b2970-105">Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **έναν αριθμό τραπεζικού λογαριασμού των ΗΠΑ** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365;</span><span class="sxs-lookup"><span data-stu-id="b2970-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b2970-106">Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για αυτό που αναζητά η πολιτική DLP κατά την αξιολόγησή της.</span><span class="sxs-lookup"><span data-stu-id="b2970-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="b2970-107">Για παράδειγμα, για μια πολιτική **αριθμού τραπεζικού λογαριασμού των Η.Π.Α.** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:</span><span class="sxs-lookup"><span data-stu-id="b2970-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b2970-108">**[Μορφή:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 ψηφία</span><span class="sxs-lookup"><span data-stu-id="b2970-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="b2970-109">**[Μοτίβο:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 συνεχόμενα ψηφία.</span><span class="sxs-lookup"><span data-stu-id="b2970-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="b2970-110">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="b2970-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="b2970-111">**[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="b2970-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b2970-112">Η κανονική έκφραση Regex_usa_bank_account_number βρίσκει περιεχόμενο που ταιριάζει με το μοτίβο</span><span class="sxs-lookup"><span data-stu-id="b2970-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="b2970-113">Βρέθηκε μια λέξη-κλειδί από Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="b2970-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="b2970-114">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική **αριθμού τραπεζικού λογαριασμού ΗΠΑ:** Έλεγχος λογαριασμού 78344011</span><span class="sxs-lookup"><span data-stu-id="b2970-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="b2970-115">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό ενός **αριθμού τραπεζικού λογαριασμού των ΗΠΑ** για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: Τι αναζητούν οι [Τύποι ευαίσθητων πληροφοριών για τον αριθμό τραπεζικού λογαριασμού ΤΩΝ ΗΠΑ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="b2970-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="b2970-116">Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="b2970-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  