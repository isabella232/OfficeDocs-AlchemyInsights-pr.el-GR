---
title: Τεχνολογία DLP δεν λειτουργεί όπως αναμένεται
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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941068"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e4d60-102">Τεχνολογία DLP δεν λειτουργεί όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="e4d60-102">DLP not working as expected</span></span>

<span data-ttu-id="e4d60-103">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** στο Office 365 δεν λειτουργεί όπως αναμένεται;</span><span class="sxs-lookup"><span data-stu-id="e4d60-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e4d60-104">Σε αυτή την περίπτωση, βεβαιωθείτε ότι η **τεχνολογία DLP πολιτική** έχει ρυθμιστεί σωστά και ότι τα δεδομένα σας περιέχουν ποια η **τεχνολογία DLP πολιτική** αναζητά όταν έχει αξιολογηθεί.</span><span class="sxs-lookup"><span data-stu-id="e4d60-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="e4d60-105">**Ρύθμιση της τεχνολογίας DLP**</span><span class="sxs-lookup"><span data-stu-id="e4d60-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="e4d60-106">Τεχνολογία DLP πολιτικές σάς επιτρέπει την αναγνώριση και την προστασία των ευαίσθητων πληροφοριών στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="e4d60-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e4d60-107">Για την παραμετροποίηση DLP πολιτικές, χρησιμοποιήστε τις πληροφορίες [εδώ](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="e4d60-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="e4d60-108">**Αναζητήστε τις πολιτικές DLP**</span><span class="sxs-lookup"><span data-stu-id="e4d60-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e4d60-109">Όταν χρησιμοποιείτε τους **τύπους ενσωματωμένων ευαίσθητες πληροφορίες** στο Κέντρο ασφαλείας για το Office 365 και συμμόρφωση, πολιτικές DLP αναζητήστε συγκεκριμένα μοτίβα και στοιχεία κατά τον εντοπισμό αυτών των τύπων διάκριση πεζών-κεφαλαίων.</span><span class="sxs-lookup"><span data-stu-id="e4d60-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e4d60-110">**Τύποι ενσωματωμένη ευαίσθητες πληροφορίες**</span><span class="sxs-lookup"><span data-stu-id="e4d60-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e4d60-111">Για πληροφορίες σχετικά με τους τύπους ενσωματωμένων διάκριση πεζών-κεφαλαίων και τι μια πολιτική DLP αναζητά κατά τον εντοπισμό του τύπου διάκριση πεζών-κεφαλαίων, ανατρέξτε στο θέμα: [Αναζητήστε το ποιους τύπους ευαίσθητες πληροφορίες](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="e4d60-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="e4d60-112">**Τύποι προσαρμοσμένων ευαίσθητες πληροφορίες**</span><span class="sxs-lookup"><span data-stu-id="e4d60-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e4d60-113">Εάν προσπαθείτε να δημιουργήσετε τύπους προσαρμοσμένων ευαίσθητες πληροφορίες, χρησιμοποιήστε το ακόλουθο άρθρο για πληροφορίες σχετικά με τον τρόπο για να δημιουργήσετε έναν προσαρμοσμένο τύπο διάκριση πεζών-κεφαλαίων: [Δημιουργία προσαρμοσμένου ευαίσθητες πληροφορίες τύπου](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="e4d60-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e4d60-114">**Δοκιμή μιας πολιτικής DLP**</span><span class="sxs-lookup"><span data-stu-id="e4d60-114">**Test a DLP policy**</span></span>

<span data-ttu-id="e4d60-115">Για να ελέγξετε τα δεδομένα σας με έναν τύπο ενσωματωμένα ή προσαρμοσμένα ευαίσθητες πληροφορίες, να χρησιμοποιήσετε την επιλογή **Τύπος ελέγχου** υπό **ταξινομήσεις** > **τύποι ευαίσθητων πληροφοριών**.</span><span class="sxs-lookup"><span data-stu-id="e4d60-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e4d60-116">Για περισσότερες πληροφορίες, δείτε [τύπους προσαρμοσμένων ευαίσθητες πληροφορίες δοκιμής](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="e4d60-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e4d60-117">**Αναφορές**</span><span class="sxs-lookup"><span data-stu-id="e4d60-117">**Reports**</span></span>
  
- <span data-ttu-id="e4d60-118">Λήψη ευαίσθητων δεδομένων ιδέες με [αναφορές DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e4d60-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e4d60-119">Δείτε συγκεκριμένες λεπτομέρειες του συμβάντος με μια [Αναφορά περιστατικού](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="e4d60-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
