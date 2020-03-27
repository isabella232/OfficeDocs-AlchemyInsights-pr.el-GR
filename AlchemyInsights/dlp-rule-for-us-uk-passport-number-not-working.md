---
title: DLP κανόνας για ηπα / UK αριθμός διαβατηρίου δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977106"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="4a0e0-102">Προβλήματα με DLP - ΗΠΑ / Ηνωμένο Βασίλειο αριθμούς διαβατηρίων</span><span class="sxs-lookup"><span data-stu-id="4a0e0-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="4a0e0-103">**Σημαντικό:** Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες – Επισκεφθείτε [τις προσωρινές προσαρμογές δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="4a0e0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4a0e0-104">**DLP θέματα με τις ΗΠΑ / Ηνωμένο Βασίλειο αριθμούς διαβατηρίων**</span><span class="sxs-lookup"><span data-stu-id="4a0e0-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="4a0e0-105">Αντιμετωπίζετε προβλήματα με **την Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό διαβατηρίου ΗΠΑ/Ηνωμένου Βασιλείου** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών DLP στο O365;</span><span class="sxs-lookup"><span data-stu-id="4a0e0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="4a0e0-106">Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για αυτό που αναζητά η πολιτική DLP κατά την αξιολόγησή της.</span><span class="sxs-lookup"><span data-stu-id="4a0e0-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="4a0e0-107">Για παράδειγμα, για μια πολιτική **αριθμού διαβατηρίου ΗΠΑ/Ηνωμένου Βασιλείου** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 75%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπίζονται για να ενεργοποιηθεί ο κανόνας</span><span class="sxs-lookup"><span data-stu-id="4a0e0-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="4a0e0-108">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Εννέα ψηφία</span><span class="sxs-lookup"><span data-stu-id="4a0e0-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="4a0e0-109">**[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Εννέα συνεχόμενα ψηφία</span><span class="sxs-lookup"><span data-stu-id="4a0e0-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="4a0e0-110">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="4a0e0-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="4a0e0-111">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="4a0e0-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4a0e0-112">Η συνάρτηση Func_usa_uk_passport εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="4a0e0-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4a0e0-113">Βρέθηκε μια λέξη-κλειδί από Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="4a0e0-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="4a0e0-114">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική **αριθμού διαβατηρίου ΗΠΑ/Ηνωμένου Βασιλείου:** Αριθμός διαβατηρίου 123456789</span><span class="sxs-lookup"><span data-stu-id="4a0e0-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="4a0e0-115">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό ενός αριθμού διαβατηρίου Η.Π.Α./ΗΒ για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για τον αριθμό διαβατηρίου Η.Π.Α./Uk](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="4a0e0-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="4a0e0-116">Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4a0e0-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  