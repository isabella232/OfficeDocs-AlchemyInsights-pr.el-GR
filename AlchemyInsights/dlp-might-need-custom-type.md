---
title: Μπορεί να χρειαστεί προσαρμοσμένος τύπος
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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052901"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="7e017-102">Μπορεί να χρειαστεί προσαρμοσμένος τύπος</span><span class="sxs-lookup"><span data-stu-id="7e017-102">DLP might need a custom type</span></span>

<span data-ttu-id="7e017-103">Με μια πολιτική αποτροπής απώλειας δεδομένων, μπορείτε να αναγνωρίζετε και να προστατεύετε τα ευαίσθητα δεδομένα στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="7e017-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="7e017-104">Σε ορισμένα σενάρια, ίσως χρειαστεί να δημιουργήσετε τον δικό σας **Προσαρμοσμένο** τύπο ευαίσθητων πληροφοριών για να προστατεύσετε τα δεδομένα του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="7e017-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="7e017-105">Για παράδειγμα, ο οργανισμός σας μπορεί να χρειάζεται να εντοπίζει και να προστατεύει τα αναγνωριστικά των εργαζομένων ή άλλα δεδομένα σε κάποια μορφή που αφορά τον οργανισμό σας. Σε αυτήν την περίπτωση, ανατρέξτε στα ακόλουθα άρθρα για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="7e017-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="7e017-106">**Προσαρμογή ενός ενσωματωμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="7e017-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="7e017-107">Εάν ένας ενσωματωμένος τύπος ευαίσθητων πληροφοριών ανταποκρίνεται στις ανάγκες σας με λίγα μόνο τσιμπήματα, μπορείτε να [προσαρμόσετε έναν ενσωματωμένο τύπο ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="7e017-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="7e017-108">Για παράδειγμα, μπορείτε να προσθέσετε ή να καταργήσετε λέξεις-κλειδιά ή να προσθέσετε ή να καταργήσετε στοιχεία υποστήριξης, όπως μια ημερομηνία ή μια διεύθυνση.</span><span class="sxs-lookup"><span data-stu-id="7e017-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="7e017-109">**Δημιουργία ενός προσαρμοσμένου τύπου ευαίσθητων πληροφοριών**</span><span class="sxs-lookup"><span data-stu-id="7e017-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="7e017-110">Ωστόσο, αν θέλετε να εντοπίσετε και να προστατεύσετε εντελώς έναν διαφορετικό τύπο ευαίσθητων πληροφοριών, μπορείτε να [δημιουργήσετε έναν τύπο προσαρμοσμένων ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) στο περιβάλλον εργασίας χρήστη του κέντρου συμμόρφωσης & ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="7e017-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="7e017-111">**Δημιουργία ενός προσαρμοσμένου τύπου ευαίσθητων πληροφοριών στην ασφάλεια & κέντρο συμμόρφωσης PowerShell**</span><span class="sxs-lookup"><span data-stu-id="7e017-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="7e017-112">Τέλος, εάν το περιβάλλον εργασίας χρήστη δεν παρέχει όλες τις επιλογές που χρειάζεστε, μπορείτε να [δημιουργήσετε έναν τύπο προσαρμοσμένων ευαίσθητων πληροφοριών στην ασφάλεια & κέντρο συμμόρφωσης PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="7e017-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="7e017-113">Ξεκινώντας με ένα αρχείο XML, μπορείτε να χρησιμοποιήσετε κάθε διαθέσιμη επιλογή.</span><span class="sxs-lookup"><span data-stu-id="7e017-113">By starting with an XML file, you can use every option available.</span></span>
