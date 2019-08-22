---
title: Τεχνολογία DLP κανόνα για Ασφάλισης δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529853"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="81921-102">Τεχνολογία DLP ζητήματα με αριθμούς κοινωνικής ασφάλισης</span><span class="sxs-lookup"><span data-stu-id="81921-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="81921-103">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** δεν λειτουργεί για περιεχόμενο που περιέχει έναν **Αριθμό κοινωνικής ασφάλισης (SSN)** κατά τη χρήση ενός τύπου ευαίσθητων πληροφοριών στο Office 365;</span><span class="sxs-lookup"><span data-stu-id="81921-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="81921-104">Σε αυτή την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για την πολιτική DLP που αναζήτηση.</span><span class="sxs-lookup"><span data-stu-id="81921-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="81921-105">Για παράδειγμα, για μια πολιτική Ασφάλισης που έχει ρυθμιστεί με ένα επίπεδο εμπιστοσύνης του 85%, τα ακόλουθα αξιολογούνται και πρέπει να εντοπίζονται για τον κανόνα ενεργοποίησης:</span><span class="sxs-lookup"><span data-stu-id="81921-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="81921-106">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ψηφία, η οποία μπορεί να βρίσκεται σε μια διαμορφωμένη ή μη διαμορφωμένη μοτίβο</span><span class="sxs-lookup"><span data-stu-id="81921-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="81921-107">**[Μοτίβο:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Τέσσερις λειτουργίες αναζήτηση για SSNs σε τέσσερα διαφορετικά μοτίβα:</span><span class="sxs-lookup"><span data-stu-id="81921-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="81921-108">Func_ssn εντοπίζει SSNs με 2011 πριν από έντονη μορφοποίηση που είναι μορφοποιημένα με παύλες ή κενά διαστήματα (dddd ηη ηηη OR ηηη-ηη-dddd)</span><span class="sxs-lookup"><span data-stu-id="81921-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="81921-109">Func_unformatted_ssn εντοπίζει SSNs με 2011 πριν από έντονη μορφοποίηση που είναι μορφοποιημένο με εννέα συνεχόμενα ψηφία (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="81921-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="81921-110">Func_randomized_formatted_ssn εντοπίζει post 2011 SSNs που είναι μορφοποιημένα με παύλες ή κενά διαστήματα (dddd ηη ηηη OR ηηη-ηη-dddd)</span><span class="sxs-lookup"><span data-stu-id="81921-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="81921-111">Func_randomized_unformatted_ssn εντοπίζει post 2011 SSNs που είναι μορφοποιημένο με εννέα συνεχόμενα ψηφία (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="81921-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="81921-112">**[Αθροίσματος ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Όχι, δεν υπάρχει καμία άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="81921-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="81921-113">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Μια πολιτική DLP είναι 85% βέβαιος ότι έχει εντοπίσει αυτόν τον τύπο των ευαίσθητων πληροφοριών εάν, μέσα σε μια απόσταση 300 χαρακτήρες:</span><span class="sxs-lookup"><span data-stu-id="81921-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="81921-114">Η [συνάρτηση Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) εντοπίζει περιεχομένου που ταιριάζει με το μοτίβο.</span><span class="sxs-lookup"><span data-stu-id="81921-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="81921-115">Μπορείτε να βρείτε μια λέξη-κλειδί από το [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="81921-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="81921-116">Περιλαμβάνει παραδείγματα των λέξεων-κλειδιών: *κοινωνικής ασφάλισης, κοινωνική ασφάλιση #, Soc δευτ., αριθμού κοινωνικής Ασφάλισης* .</span><span class="sxs-lookup"><span data-stu-id="81921-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="81921-117">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιήσει για την πολιτική DLP Ασφάλισης: **Ασφάλισης: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="81921-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="81921-118">Για περισσότερες πληροφορίες σχετικά με τι απαιτείται για SSNs να εντοπιστεί για το περιεχόμενό σας, ανατρέξτε στην ενότητα παρακάτω σε αυτό το άρθρο: [Τι η διάκριση πεζών-κεφαλαίων τύπους πληροφοριών αναζητούν SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="81921-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="81921-119">Χρησιμοποιώντας έναν τύπο διαφορετική ενσωματωμένη ευαίσθητες πληροφορίες, ανατρέξτε στο παρακάτω άρθρο για πληροφορίες σχετικά με τι απαιτείται για άλλους τύπους: [Αναζητήστε τι η διάκριση πεζών-κεφαλαίων τύπων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="81921-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  