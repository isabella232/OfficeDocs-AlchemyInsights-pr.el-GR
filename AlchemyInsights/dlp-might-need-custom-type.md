---
title: Το DLP μπορεί να χρειάζεται έναν προσαρμοσμένο τύπο
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712184"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="5efdd-102">Το DLP μπορεί να χρειάζεται έναν προσαρμοσμένο τύπο</span><span class="sxs-lookup"><span data-stu-id="5efdd-102">DLP might need a custom type</span></span>

<span data-ttu-id="5efdd-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="5efdd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5efdd-104">**Το DLP μπορεί να απαιτήσει έναν προσαρμοσμένο τύπο πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="5efdd-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="5efdd-105">Με μια πολιτική αποτροπής απώλειας δεδομένων (DLP), μπορείτε να αναγνωρίζετε και να προστατεύετε ευαίσθητα δεδομένα στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="5efdd-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="5efdd-106">Σε ορισμένα σενάρια, ίσως χρειαστεί να δημιουργήσετε τον δικό σας **Προσαρμοσμένο** ευαίσθητο τύπο πληροφοριών για να προστατεύσετε τα δεδομένα του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="5efdd-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="5efdd-107">Για παράδειγμα, ο οργανισμός σας ίσως χρειαστεί να προσδιορίσει και να προστατεύσει τα αναγνωριστικά των εργαζομένων ή άλλα δεδομένα σε κάποια μορφή που αφορά ειδικά το org. Εάν Ναι, ανατρέξτε στα παρακάτω άρθρα για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="5efdd-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="5efdd-108">**Προσαρμογή ενός ενσωματωμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="5efdd-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="5efdd-109">Εάν ένας ενσωματωμένος τύπος ευαίσθητων πληροφοριών θα ικανοποιήσει τις ανάγκες σας με λίγα μόνο τσιμπήματα, μπορείτε να [προσαρμόσετε έναν ενσωματωμένο τύπο ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5efdd-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="5efdd-110">Για παράδειγμα, μπορείτε να προσθέσετε ή να καταργήσετε λέξεις-κλειδιά ή να προσθέσετε ή να καταργήσετε στοιχεία υποστήριξης, όπως μια ημερομηνία ή διεύθυνση.</span><span class="sxs-lookup"><span data-stu-id="5efdd-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="5efdd-111">**Δημιουργία προσαρμοσμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="5efdd-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="5efdd-112">Ωστόσο, εάν πρέπει να προσδιορίσετε και να προστατεύσετε εντελώς έναν διαφορετικό τύπο ευαίσθητων πληροφοριών, μπορείτε να [δημιουργήσετε έναν προσαρμοσμένο τύπο ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) στο περιβάλλον εργασίας χρήστη του κέντρου συμμόρφωσης & ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="5efdd-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="5efdd-113">**Δημιουργία προσαρμοσμένου τύπου ευαίσθητων πληροφοριών στο κέντρο συμμόρφωσης του κέντρου συμμόρφωσης για την ασφάλεια &**</span><span class="sxs-lookup"><span data-stu-id="5efdd-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="5efdd-114">Τέλος, εάν το περιβάλλον εργασίας χρήστη δεν παρέχει όλες τις επιλογές που χρειάζεστε, μπορείτε να [δημιουργήσετε έναν προσαρμοσμένο τύπο ευαίσθητων πληροφοριών στο κέντρο συμμόρφωσης του PowerShell για & ασφαλείας](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="5efdd-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="5efdd-115">Ξεκινώντας με ένα αρχείο XML, μπορείτε να χρησιμοποιήσετε κάθε διαθέσιμη επιλογή.</span><span class="sxs-lookup"><span data-stu-id="5efdd-115">By starting with an XML file, you can use every option available.</span></span>
