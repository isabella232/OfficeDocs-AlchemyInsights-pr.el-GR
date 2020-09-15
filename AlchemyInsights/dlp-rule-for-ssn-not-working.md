---
title: Ο κανόνας DLP για το SSN δεν λειτουργεί
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679369"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="6b3c7-102">Θέματα DLP με αριθμούς κοινωνικής ασφάλισης</span><span class="sxs-lookup"><span data-stu-id="6b3c7-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="6b3c7-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="6b3c7-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6b3c7-104">**Θέματα DLP με το SSNs**</span><span class="sxs-lookup"><span data-stu-id="6b3c7-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="6b3c7-105">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για το περιεχόμενο που περιέχει έναν **αριθμό ΚΟΙΝΩΝΙΚΉς ασφάλισης (SSN)** κατά τη χρήση ενός ευαίσθητου τύπου πληροφοριών στο Microsoft 365;</span><span class="sxs-lookup"><span data-stu-id="6b3c7-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="6b3c7-106">Εάν Ναι, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαιτούμενες πληροφορίες για το τι αναζητά η πολιτική DLP.</span><span class="sxs-lookup"><span data-stu-id="6b3c7-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="6b3c7-107">Για παράδειγμα, για μια πολιτική SSN που έχει ρυθμιστεί με επίπεδο αξιοπιστίας 85%, τα παρακάτω αξιολογούνται και πρέπει να ανιχνευθούν για να ενεργοποιείται ο κανόνας:</span><span class="sxs-lookup"><span data-stu-id="6b3c7-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="6b3c7-108">**[Μορφοποίηση:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 ψηφία, τα οποία μπορεί να βρίσκονται σε μορφοποιημένο ή μη μορφοποιημένο μοτίβο</span><span class="sxs-lookup"><span data-stu-id="6b3c7-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="6b3c7-109">**[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις συναρτήσεις αναζητήστε το SSNs σε τέσσερα διαφορετικά μοτίβα:</span><span class="sxs-lookup"><span data-stu-id="6b3c7-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="6b3c7-110">Func_ssn εντοπίζει το SSNs με ισχυρή μορφοποίηση pre-2011 που είναι μορφοποιημένη με παύλες ή κενά διαστήματα (DDD-DD-ηηηη ή DDD DD ηηηη)</span><span class="sxs-lookup"><span data-stu-id="6b3c7-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="6b3c7-111">Func_unformatted_ssn εντοπίζει το SSNs με την προ-2011 ισχυρή μορφοποίηση που δεν έχει μορφοποιηθεί ως εννέα διαδοχικά ψηφία (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="6b3c7-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="6b3c7-112">Func_randomized_formatted_ssn εντοπίζει την καταχώρηση-2011 SSNs που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (DDD-DD-ηηηη ή DDD DD ηηηη)</span><span class="sxs-lookup"><span data-stu-id="6b3c7-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="6b3c7-113">Func_randomized_unformatted_ssn εντοπίζει τη δημοσίευση-2011 SSNs που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="6b3c7-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="6b3c7-114">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Όχι, δεν υπάρχει άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="6b3c7-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="6b3c7-115">**[Ορισμός:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, μέσα σε μια εγγύτητα των 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="6b3c7-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6b3c7-116">Η [συνάρτηση Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="6b3c7-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="6b3c7-117">Βρέθηκε μια λέξη-κλειδί από [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="6b3c7-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="6b3c7-118">Παραδείγματα λέξεων-κλειδιών περιλαμβάνουν:  *κοινωνική ασφάλιση, κοινωνική ασφάλιση #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="6b3c7-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="6b3c7-119">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει την πολιτική DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="6b3c7-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="6b3c7-120">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για την ανίχνευση του SSNs για το περιεχόμενό σας, ανατρέξτε στην παρακάτω ενότητα σε αυτό το άρθρο: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για το SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="6b3c7-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="6b3c7-121">Με τη χρήση διαφορετικού ενσωματωμένου τύπου ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="6b3c7-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  