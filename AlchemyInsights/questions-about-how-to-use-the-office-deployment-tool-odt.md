---
title: Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959683"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης (ODT)

Κάντε λήψη του Office ανάπτυξης από το [Κέντρο λήψης αρχείων της Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Μετά τη λήψη του αρχείου, εκτελέστε το εκτελέσιμο αρχείο αυτο-εξαγωγής, το οποίο περιέχει το εκτελέσιμο αρχείο του Εργαλείου ανάπτυξης Office (setup.exe) και ένα δείγμα αρχείου ρύθμισης παραμέτρων (configuration.xml).
  
 **Για να εξαιρέσετε ή να καταργήσετε Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις από υπολογιστές-πελάτες:**
  
Κατά την εγκατάσταση Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις, μπορείτε να εξαιρέσετε συγκεκριμένα προϊόντα. Για να το κάνετε αυτό, ακολουθήστε τα βήματα για την Office με το ODT, αλλά συμπεριλάβετε το στοιχείο ExcludeApp στο αρχείο ρύθμισης παραμέτρων. Για παράδειγμα, αυτό το αρχείο ρύθμισης παραμέτρων εγκαθιστά όλα τα Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις εκτός από Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Επισκόπηση του εργαλείου Office ανάπτυξης](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

