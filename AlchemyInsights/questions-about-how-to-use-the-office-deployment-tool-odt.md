---
title: Ερωτήσεις σχετικά με τον τρόπο χρήσης του εργαλείου ανάπτυξης του Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774891"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Ερωτήσεις σχετικά με τον τρόπο χρήσης του εργαλείου ανάπτυξης του Office (ODT)

Κάντε λήψη του εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης αρχείων της Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Μετά τη λήψη του αρχείου, εκτελέστε το εκτελέσιμο αρχείο αυτόματης εξαγωγής, το οποίο περιέχει το εκτελέσιμο εργαλείο ανάπτυξης του Office (setup.exe) και ένα δείγμα αρχείου ρύθμισης παραμέτρων (configuration.xml).
  
 **Για να εξαιρέσετε ή να καταργήσετε εφαρμογές του Microsoft 365 για εταιρικά προϊόντα από υπολογιστές-πελάτες:**
  
Κατά την εγκατάσταση των εφαρμογών Microsoft 365 για επιχειρήσεις, μπορείτε να εξαιρέσετε συγκεκριμένα προϊόντα. Για να το κάνετε αυτό, ακολουθήστε τα βήματα για την εγκατάσταση του Office με το ODT, αλλά συμπεριλάβετε το στοιχείο ExcludeApp στο αρχείο ρύθμισης παραμέτρων. Για παράδειγμα, αυτό το αρχείο ρύθμισης παραμέτρων εγκαθιστά όλες τις εφαρμογές του Microsoft 365 για εταιρικά προϊόντα εκτός από τον Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Επισκόπηση του εργαλείου ανάπτυξης του Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

