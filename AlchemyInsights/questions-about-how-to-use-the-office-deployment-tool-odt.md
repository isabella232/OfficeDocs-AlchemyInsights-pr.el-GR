---
title: Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553540"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης Tool (ODT)

Κάντε λήψη του εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης της Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Μετά τη λήψη του αρχείου, εκτελέστε το αυτοαποσυμπιεζόμενο εκτελέσιμο αρχείο, που περιέχει το Office εργαλείο ανάπτυξης εκτελέσιμο (setup.exe) και ένα αρχείο ρύθμισης παραμέτρων δείγματος (configuration.xml).
  
 **Για να αποκλείσετε ή να καταργήσετε τα προϊόντα του Office 365 ProPlus από υπολογιστές-πελάτες:**
  
Κατά την εγκατάσταση του Office 365 ProPlus, μπορείτε να εξαιρέσετε συγκεκριμένα προϊόντα. Για να γίνει αυτό, ακολουθήστε τα βήματα για την εγκατάσταση του Office με το ODT, αλλά περιλαμβάνει το στοιχείο ExcludeApp στο αρχείο ρύθμισης παραμέτρων. Για παράδειγμα, αυτό το αρχείο παραμέτρων εγκαθιστά όλα τα προϊόντα του Office 365 ProPlus εκτός από το Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Επισκόπηση του εργαλείου ανάπτυξης του Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

