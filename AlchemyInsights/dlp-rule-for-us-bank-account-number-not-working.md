---
title: Κανόνας DLP για τον αριθμό τραπεζικού λογαριασμού των ΗΠΑ που δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932534"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="d193e-102">Ζητήματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ</span><span class="sxs-lookup"><span data-stu-id="d193e-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="d193e-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="d193e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d193e-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="d193e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d193e-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d193e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d193e-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="d193e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d193e-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="d193e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d193e-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="d193e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d193e-109">**Ζητήματα DLP με αριθμούς τραπεζικών λογαριασμών των ΗΠΑ**</span><span class="sxs-lookup"><span data-stu-id="d193e-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="d193e-110">Αντιμετωπίζετε προβλήματα με **την αποτροπή απώλειας δεδομένων (DLP)** που δεν λειτουργεί για περιεχόμενο που περιέχει **έναν αριθμό τραπεζικού λογαριασμού των ΗΠΑ** όταν χρησιμοποιείτε έναν τύπο ευαίσθητων πληροφοριών DLP στο O365;</span><span class="sxs-lookup"><span data-stu-id="d193e-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d193e-111">Σε αυτήν την περίπτωση, βεβαιωθείτε ότι το περιεχόμενό σας περιέχει τις απαραίτητες πληροφορίες για αυτό που αναζητά η πολιτική DLP κατά την αξιολόγησή της.</span><span class="sxs-lookup"><span data-stu-id="d193e-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d193e-112">Για παράδειγμα, για μια πολιτική **αριθμού τραπεζικού λογαριασμού των Η.Π.Α.** που έχει ρυθμιστεί με επίπεδο εμπιστοσύνης 85%, αξιολογούνται τα ακόλουθα και πρέπει να εντοπιστούν για να ενεργοποιηθεί ο κανόνας:</span><span class="sxs-lookup"><span data-stu-id="d193e-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d193e-113">**[Μορφή:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 ψηφία</span><span class="sxs-lookup"><span data-stu-id="d193e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="d193e-114">**[Μοτίβο:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 συνεχόμενα ψηφία.</span><span class="sxs-lookup"><span data-stu-id="d193e-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="d193e-115">**[Άθροισμα ελέγχου:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Όχι, δεν υπάρχει άθροισμα ελέγχου</span><span class="sxs-lookup"><span data-stu-id="d193e-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d193e-116">**[Ορισμός:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Μια πολιτική DLP είναι 75% πεπεισμένη ότι εντόπισε αυτόν τον τύπο ευαίσθητων πληροφοριών εάν, σε κοντινή απόσταση 300 χαρακτήρων:</span><span class="sxs-lookup"><span data-stu-id="d193e-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d193e-117">Η κανονική έκφραση Regex_usa_bank_account_number βρίσκει περιεχόμενο που ταιριάζει με το μοτίβο</span><span class="sxs-lookup"><span data-stu-id="d193e-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="d193e-118">Βρέθηκε μια λέξη-κλειδί από Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="d193e-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="d193e-119">Για παράδειγμα, το ακόλουθο δείγμα θα ενεργοποιούσε την πολιτική **αριθμού τραπεζικού λογαριασμού ΗΠΑ:** Έλεγχος λογαριασμού 78344011</span><span class="sxs-lookup"><span data-stu-id="d193e-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="d193e-120">Για περισσότερες πληροφορίες σχετικά με το τι απαιτείται για τον εντοπισμό ενός **αριθμού τραπεζικού λογαριασμού των ΗΠΑ** για το περιεχόμενό σας, ανατρέξτε στην ακόλουθη ενότητα σε αυτό το άρθρο: Τι αναζητούν οι [Τύποι ευαίσθητων πληροφοριών για τον αριθμό τραπεζικού λογαριασμού ΤΩΝ ΗΠΑ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="d193e-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="d193e-121">Χρησιμοποιώντας έναν διαφορετικό ενσωματωμένο τύπο ευαίσθητων πληροφοριών, ανατρέξτε στο ακόλουθο άρθρο για πληροφορίες σχετικά με το τι απαιτείται για άλλους τύπους: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d193e-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  