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
ms.openlocfilehash: 3d8316502b4e51a101197a908cf691f0ab7f845a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389613"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="911aa-102">Τεχνολογία DLP δεν λειτουργεί όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="911aa-102">DLP not working as expected</span></span>

<span data-ttu-id="911aa-103">Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** στο Office 365 δεν λειτουργεί όπως αναμένεται;</span><span class="sxs-lookup"><span data-stu-id="911aa-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="911aa-104">Σε αυτή την περίπτωση, βεβαιωθείτε ότι η **τεχνολογία DLP πολιτική** έχει ρυθμιστεί σωστά και ότι τα δεδομένα σας περιέχουν ποια η **τεχνολογία DLP πολιτική** αναζητά όταν έχει αξιολογηθεί.</span><span class="sxs-lookup"><span data-stu-id="911aa-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="911aa-105">**Ορισμός DLP:**</span><span class="sxs-lookup"><span data-stu-id="911aa-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="911aa-106">Τεχνολογία DLP πολιτικές σάς επιτρέπει την αναγνώριση και την προστασία των ευαίσθητων πληροφοριών στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="911aa-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="911aa-107">Για την παραμετροποίηση DLP πολιτικές, χρησιμοποιήστε τις πληροφορίες [εδώ](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="911aa-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="911aa-108">**Ποιες πολιτικές DLP αναζήτηση για:**</span><span class="sxs-lookup"><span data-stu-id="911aa-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="911aa-109">Όταν χρησιμοποιείτε τους **τύπους ενσωματωμένων ευαίσθητες πληροφορίες** στο Κέντρο ασφαλείας για το Office 365 και συμμόρφωση, πολιτικές DLP αναζητήστε συγκεκριμένα μοτίβα και στοιχεία κατά τον εντοπισμό αυτών των τύπων διάκριση πεζών-κεφαλαίων.</span><span class="sxs-lookup"><span data-stu-id="911aa-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="911aa-110">**Τύποι ενσωματωμένη ευαίσθητες πληροφορίες:**</span><span class="sxs-lookup"><span data-stu-id="911aa-110">**Built-in Sensitive Information Types:**</span></span>

    <span data-ttu-id="911aa-111">Για πληροφορίες σχετικά με τους τύπους ενσωματωμένων διάκριση πεζών-κεφαλαίων και τι μια πολιτική DLP αναζητά κατά τον εντοπισμό του τύπου διάκριση πεζών-κεφαλαίων, ανατρέξτε στο θέμα: [Αναζητήστε το ποιους τύπους ευαίσθητες πληροφορίες](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="911aa-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="911aa-112">**Τύποι προσαρμοσμένων ευαίσθητες πληροφορίες:**</span><span class="sxs-lookup"><span data-stu-id="911aa-112">**Custom Sensitive Information Types:**</span></span>

    <span data-ttu-id="911aa-113">Εάν προσπαθείτε να δημιουργήσετε τύπους προσαρμοσμένων ευαίσθητες πληροφορίες, χρησιμοποιήστε το ακόλουθο άρθρο για πληροφορίες σχετικά με τον τρόπο για να δημιουργήσετε έναν προσαρμοσμένο τύπο διάκριση πεζών-κεφαλαίων: [Δημιουργία προσαρμοσμένου ευαίσθητες πληροφορίες τύπου](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="911aa-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

 <span data-ttu-id="911aa-114">**Εκθέσεις:**</span><span class="sxs-lookup"><span data-stu-id="911aa-114">**Reports:**</span></span>
  
- <span data-ttu-id="911aa-115">Λήψη ευαίσθητων δεδομένων ιδέες με [αναφορές DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="911aa-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="911aa-116">Δείτε συγκεκριμένες λεπτομέρειες του συμβάντος με μια [Αναφορά περιστατικού](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="911aa-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
