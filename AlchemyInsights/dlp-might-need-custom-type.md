---
title: Το DLP ενδέχεται να χρειάζεται έναν προσαρμοσμένο τύπο
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507514"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="c3002-102">Το DLP ενδέχεται να χρειάζεται έναν προσαρμοσμένο τύπο</span><span class="sxs-lookup"><span data-stu-id="c3002-102">DLP might need a custom type</span></span>

<span data-ttu-id="c3002-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="c3002-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c3002-104">**Το DLP ενδέχεται να απαιτεί έναν προσαρμοσμένο τύπο πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="c3002-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="c3002-105">Με μια πολιτική αποτροπής απώλειας δεδομένων (DLP), μπορείτε να εντοπίσετε και να προστατεύσετε ευαίσθητα δεδομένα στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="c3002-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="c3002-106">Σε ορισμένα σενάρια, ίσως χρειαστεί να δημιουργήσετε τον δικό σας **προσαρμοσμένο** τύπο ευαίσθητων πληροφοριών για να προστατεύσετε τα δεδομένα της εταιρείας σας.</span><span class="sxs-lookup"><span data-stu-id="c3002-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="c3002-107">Για παράδειγμα, ο οργανισμός σας ίσως χρειαστεί να αναγνωρίσει και να προστατεύσει αναγνωριστικά υπαλλήλων ή άλλα δεδομένα σε κάποια μορφή ειδικά για τον οργανισμό σας. Σε αυτήν την περίπτωση, ανατρέξτε στα ακόλουθα άρθρα για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="c3002-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="c3002-108">**Προσαρμογή ενσωματωμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="c3002-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="c3002-109">Εάν ένας ενσωματωμένος ευαίσθητος τύπος πληροφοριών θα ικανοποιούσε τις ανάγκες σας με ακριβώς μερικά τσιμπήματα, μπορείτε να [προσαρμόσετε έναν ενσωματωμένο ευαίσθητο τύπο πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c3002-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="c3002-110">Για παράδειγμα, μπορείτε να προσθέσετε ή να καταργήσετε λέξεις-κλειδιά ή να προσθέσετε ή να καταργήσετε αποδεικτικά στοιχεία, όπως μια ημερομηνία ή μια διεύθυνση.</span><span class="sxs-lookup"><span data-stu-id="c3002-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="c3002-111">**Δημιουργία προσαρμοσμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="c3002-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="c3002-112">Ωστόσο, εάν πρέπει να εντοπίσετε και να προστατεύσετε εντελώς έναν διαφορετικό τύπο ευαίσθητων πληροφοριών, μπορείτε να [δημιουργήσετε έναν προσαρμοσμένο τύπο ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) στο χρήστη του Κέντρου συμμόρφωσης & ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="c3002-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="c3002-113">**Δημιουργία προσαρμοσμένου τύπου ευαίσθητων πληροφοριών στο PowerShell του Κέντρου συμμόρφωσης security &**</span><span class="sxs-lookup"><span data-stu-id="c3002-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="c3002-114">Τέλος, εάν το περιβάλλον ασφαλείας δεν παρέχει όλες τις επιλογές που χρειάζεστε, μπορείτε να [δημιουργήσετε έναν προσαρμοσμένο τύπο ευαίσθητων πληροφοριών στο Θέμα Ασφάλεια & Κέντρο συμμόρφωσης PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="c3002-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="c3002-115">Ξεκινώντας με ένα αρχείο XML, μπορείτε να χρησιμοποιήσετε κάθε διαθέσιμη επιλογή.</span><span class="sxs-lookup"><span data-stu-id="c3002-115">By starting with an XML file, you can use every option available.</span></span>
