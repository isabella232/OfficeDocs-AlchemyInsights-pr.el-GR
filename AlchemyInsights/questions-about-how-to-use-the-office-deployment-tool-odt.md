---
title: Ερωτήσεις σχετικά με τον τρόπο χρήσης του Εργαλείου ανάπτυξης office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790332"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="0962d-102">Ερωτήσεις σχετικά με τον τρόπο χρήσης του Εργαλείου ανάπτυξης office (ODT)</span><span class="sxs-lookup"><span data-stu-id="0962d-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="0962d-103">Κάντε λήψη του Εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης αρχείων της Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="0962d-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="0962d-104">Μετά τη λήψη του αρχείου, εκτελέστε το εκτελέσιμο αρχείο αυτο-εξαγωγής, το οποίο περιέχει το εκτελέσιμο εργαλείο ανάπτυξης του Office (setup.exe) και ένα δείγμα αρχείου ρύθμισης παραμέτρων (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="0962d-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="0962d-105">**Για να εξαιρέσετε ή να καταργήσετε τις Εφαρμογές Microsoft 365 για εταιρικά προϊόντα από υπολογιστές-πελάτες:**</span><span class="sxs-lookup"><span data-stu-id="0962d-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="0962d-106">Κατά την εγκατάσταση των Εφαρμογών Microsoft 365 για μεγάλες επιχειρήσεις, μπορείτε να εξαιρέσετε συγκεκριμένα προϊόντα.</span><span class="sxs-lookup"><span data-stu-id="0962d-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="0962d-107">Για να το κάνετε αυτό, ακολουθήστε τα βήματα για την εγκατάσταση του Office με το ODT, αλλά συμπεριλάβετε το στοιχείο ExcludeApp στο αρχείο ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="0962d-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="0962d-108">Για παράδειγμα, αυτό το αρχείο ρύθμισης παραμέτρων εγκαθιστά όλες τις εφαρμογές Microsoft 365 για εταιρικά προϊόντα εκτός από τον Publisher:</span><span class="sxs-lookup"><span data-stu-id="0962d-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="0962d-109">Επισκόπηση του Εργαλείου ανάπτυξης του Office</span><span class="sxs-lookup"><span data-stu-id="0962d-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

