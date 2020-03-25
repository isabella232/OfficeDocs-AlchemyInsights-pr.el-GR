---
title: DLP δεν λειτουργεί όπως αναμένεται
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932622"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="6ddb9-102">DLP δεν λειτουργεί όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="6ddb9-102">DLP not working as expected</span></span>

<span data-ttu-id="6ddb9-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6ddb9-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6ddb9-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6ddb9-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6ddb9-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6ddb9-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="6ddb9-109">**Ρύθμιση του DLP**</span><span class="sxs-lookup"><span data-stu-id="6ddb9-109">**Setting up DLP**</span></span>

<span data-ttu-id="6ddb9-110">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** στο Office 365 που δεν λειτουργεί όπως αναμένεται;</span><span class="sxs-lookup"><span data-stu-id="6ddb9-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="6ddb9-111">Σε αυτήν την περίπτωση, βεβαιωθείτε ότι η **πολιτική DLP** έχει ρυθμιστεί σωστά και ότι τα δεδομένα σας περιέχουν αυτό που αναζητά η **πολιτική DLP** κατά την αξιολόγησή της.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="6ddb9-112">Οι πολιτικές DLP σάς επιτρέπουν να αναγνωρίζετε και να προστατεύετε ευαίσθητες πληροφορίες στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="6ddb9-113">Για να ρυθμίσετε τις πολιτικές DLP, χρησιμοποιήστε τις πληροφορίες [εδώ](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="6ddb9-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="6ddb9-114">**Τι αναζητούν οι πολιτικές DLP**</span><span class="sxs-lookup"><span data-stu-id="6ddb9-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="6ddb9-115">Όταν χρησιμοποιείτε **τους ενσωματωμένους τύπους ευαίσθητων πληροφοριών** στο Κέντρο ασφάλειας και συμμόρφωσης του Office 365, οι πολιτικές DLP αναζητούν συγκεκριμένα μοτίβα και στοιχεία κατά τον εντοπισμό αυτών των ευαίσθητων τύπων.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="6ddb9-116">**Ενσωματωμένοι ευαίσθητοι τύποι πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="6ddb9-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="6ddb9-117">Για πληροφορίες σχετικά με τους ενσωματωμένους τύπους ευαίσθητων και τι αναζητά μια πολιτική DLP κατά τον εντοπισμό του τύπου "Ευαίσθητος", ανατρέξτε στο θέμα: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="6ddb9-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="6ddb9-118">**Προσαρμοσμένοι τύποι ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="6ddb9-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="6ddb9-119">Εάν προσπαθείτε να δημιουργήσετε προσαρμοσμένους τύπους ευαίσθητων πληροφοριών, χρησιμοποιήστε το ακόλουθο άρθρο για πληροφορίες σχετικά με τον τρόπο δημιουργίας ενός προσαρμοσμένου ευαίσθητου τύπου: [Δημιουργήστε έναν προσαρμοσμένο τύπο ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6ddb9-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="6ddb9-120">**Δοκιμή πολιτικής DLP**</span><span class="sxs-lookup"><span data-stu-id="6ddb9-120">**Test a DLP policy**</span></span>

<span data-ttu-id="6ddb9-121">Για να ελέγξετε τα δεδομένα σας με ενσωματωμένο ή προσαρμοσμένο τύπο ευαίσθητων πληροφοριών, χρησιμοποιήστε την επιλογή **Τύπος δοκιμής** στην περιοχή **Ταξινομήσεις Ευαίσθητοι** > **τύποι πληροφοριών**.</span><span class="sxs-lookup"><span data-stu-id="6ddb9-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="6ddb9-122">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δοκιμή προσαρμοσμένων τύπων ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="6ddb9-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="6ddb9-123">**Εκθέσεις**</span><span class="sxs-lookup"><span data-stu-id="6ddb9-123">**Reports**</span></span>
  
- <span data-ttu-id="6ddb9-124">Λάβετε ευαίσθητες πληροφορίες δεδομένων με [τις αναφορές DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="6ddb9-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="6ddb9-125">Δείτε συγκεκριμένες λεπτομέρειες του συμβάντος με μια [αναφορά περιστατικού](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="6ddb9-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
