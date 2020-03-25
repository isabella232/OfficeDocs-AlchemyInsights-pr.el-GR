---
title: Το DLP ενδέχεται να χρειάζεται έναν προσαρμοσμένο τύπο
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932658"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="a54af-102">Το DLP ενδέχεται να χρειάζεται έναν προσαρμοσμένο τύπο</span><span class="sxs-lookup"><span data-stu-id="a54af-102">DLP might need a custom type</span></span>

<span data-ttu-id="a54af-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="a54af-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a54af-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="a54af-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a54af-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="a54af-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a54af-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="a54af-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a54af-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="a54af-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a54af-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="a54af-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a54af-109">**Το DLP ενδέχεται να απαιτεί έναν προσαρμοσμένο τύπο πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="a54af-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="a54af-110">Με μια πολιτική αποτροπής απώλειας δεδομένων (DLP), μπορείτε να εντοπίσετε και να προστατεύσετε ευαίσθητα δεδομένα στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="a54af-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="a54af-111">Σε ορισμένα σενάρια, ίσως χρειαστεί να δημιουργήσετε τον δικό σας **προσαρμοσμένο** τύπο ευαίσθητων πληροφοριών για να προστατεύσετε τα δεδομένα της εταιρείας σας.</span><span class="sxs-lookup"><span data-stu-id="a54af-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="a54af-112">Για παράδειγμα, ο οργανισμός σας ίσως χρειαστεί να αναγνωρίσει και να προστατεύσει αναγνωριστικά υπαλλήλων ή άλλα δεδομένα σε κάποια μορφή ειδικά για τον οργανισμό σας. Σε αυτήν την περίπτωση, ανατρέξτε στα ακόλουθα άρθρα για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="a54af-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="a54af-113">**Προσαρμογή ενσωματωμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="a54af-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="a54af-114">Εάν ένας ενσωματωμένος ευαίσθητος τύπος πληροφοριών θα ικανοποιούσε τις ανάγκες σας με ακριβώς μερικά τσιμπήματα, μπορείτε να [προσαρμόσετε έναν ενσωματωμένο ευαίσθητο τύπο πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="a54af-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="a54af-115">Για παράδειγμα, μπορείτε να προσθέσετε ή να καταργήσετε λέξεις-κλειδιά ή να προσθέσετε ή να καταργήσετε αποδεικτικά στοιχεία, όπως μια ημερομηνία ή μια διεύθυνση.</span><span class="sxs-lookup"><span data-stu-id="a54af-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="a54af-116">**Δημιουργία προσαρμοσμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="a54af-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="a54af-117">Ωστόσο, εάν πρέπει να εντοπίσετε και να προστατεύσετε εντελώς έναν διαφορετικό τύπο ευαίσθητων πληροφοριών, μπορείτε να [δημιουργήσετε έναν προσαρμοσμένο τύπο ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) στο χρήστη του Κέντρου συμμόρφωσης & ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="a54af-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="a54af-118">**Δημιουργία προσαρμοσμένου τύπου ευαίσθητων πληροφοριών στο PowerShell του Κέντρου συμμόρφωσης security &**</span><span class="sxs-lookup"><span data-stu-id="a54af-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="a54af-119">Τέλος, εάν το περιβάλλον ασφαλείας δεν παρέχει όλες τις επιλογές που χρειάζεστε, μπορείτε να [δημιουργήσετε έναν προσαρμοσμένο τύπο ευαίσθητων πληροφοριών στο Θέμα Ασφάλεια & Κέντρο συμμόρφωσης PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a54af-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="a54af-120">Ξεκινώντας με ένα αρχείο XML, μπορείτε να χρησιμοποιήσετε κάθε διαθέσιμη επιλογή.</span><span class="sxs-lookup"><span data-stu-id="a54af-120">By starting with an XML file, you can use every option available.</span></span>
