---
title: Κανόνας DLP για ssn δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788702"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="d2627-102">DLP θέματα με αριθμούς κοινωνικής ασφάλισης</span><span class="sxs-lookup"><span data-stu-id="d2627-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="d2627-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="d2627-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d2627-104">**Ζητήματα DLP με τα SSN**</span><span class="sxs-lookup"><span data-stu-id="d2627-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="d2627-105">Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **αριθμό κοινωνικής ασφάλισης (SSN)** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών στο Microsoft 365;</span><span class="sxs-lookup"><span data-stu-id="d2627-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="d2627-106">Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την αναζήτηση της πολιτικής DLP.</span><span class="sxs-lookup"><span data-stu-id="d2627-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="d2627-107">Για παράδειγμα, για μια πολιτική SSN που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:</span><span class="sxs-lookup"><span data-stu-id="d2627-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d2627-108">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ψηφία, τα οποία μπορεί να είναι σε μορφοποιημένο ή μη μορφοποιημένο μοτίβο</span><span class="sxs-lookup"><span data-stu-id="d2627-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="d2627-109">**[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις συναρτήσεις αναζητούν SSNs σε τέσσερα διαφορετικά μοτίβα:</span><span class="sxs-lookup"><span data-stu-id="d2627-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="d2627-110">Func_ssn εντοπίζει SSN με ισχυρή μορφοποίηση πριν από το 2011 που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (dd-dd-dddd ή ddd ddd ddd dddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="d2627-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d2627-111">Func_unformatted_ssn εντοπίζει SSN με ισχυρή μορφοποίηση πριν από το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="d2627-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="d2627-112">Func_randomized_formatted_ssn εντοπίζει ssns μετά το 2011 που έχουν μορφοποιηθεί με παύλες ή κενά διαστήματα (ddd-dd-dddd ή ddd ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="d2627-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d2627-113">Func_randomized_unformatted_ssn εντοπίζει ssns μετά το 2011 που δεν έχουν μορφοποιηθεί ως εννέα διαδοχικά ψηφία (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="d2627-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="d2627-114">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Όχι, δεν υπάρχει άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="d2627-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="d2627-115">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Μια πολιτική DLP είναι 85% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="d2627-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d2627-116">Η [συνάρτηση Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) εντοπίζει περιεχόμενο που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="d2627-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d2627-117">Βρέθηκε μια λέξη-κλειδί από [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="d2627-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="d2627-118">Παραδείγματα λέξεων-κλειδιών περιλαμβάνουν: *Κοινωνική Ασφάλιση, Κοινωνική Ασφάλιση#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="d2627-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="d2627-119">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="d2627-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="d2627-120">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό των SSN για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα αυτού του άρθρου: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών για ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="d2627-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="d2627-121">Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d2627-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  