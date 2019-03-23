---
title: Σφάλμα Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772442"
---
# <a name="winsock-error-10061"></a>Σφάλμα Winsock 10061

Αυτός ο κωδικός σφάλματος σημαίνει ότι το Office 365 δεν ήταν δυνατό να δημιουργήσει μια υποδοχή TCP (σύνδεση) με τον κεντρικό υπολογιστή προορισμού. Η πιο πιθανή αιτία αυτού του σφάλματος είναι κάποιο πρόβλημα με τις ρυθμίσεις παραμέτρων του τείχους προστασίας. Για να διορθώσετε το πρόβλημα, ελέγξτε αυτές τις ρυθμίσεις:
  
- Επαληθεύστε τις ρυθμίσεις του τείχους προστασίας σας με τις πληροφορίες [διευθύνσεων URL του Office 365 και περιοχές διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Εάν το σφάλμα αφορά σε Exchange Online προστασίας (EOP), πρέπει να έχετε προηγουμένως ειδοποιηθεί για μια αλλαγή στις [διευθύνσεις Exchange Online προστασίας IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Βεβαιωθείτε ότι η υπηρεσία παροχής Internet (ISP) δεν εμποδίζει τη θύρα.
    
- Επαληθεύστε τις Έξυπνες ρυθμίσεις διακομιστή κεντρικού υπολογιστή και του προορισμού σε σας γραμμές σύνδεσης.
    
Σημειώστε ότι Office 365 δεν αποκλειστούν οι *εισερχόμενες* συνδέσεις με αυτόν τον τρόπο. 
  

