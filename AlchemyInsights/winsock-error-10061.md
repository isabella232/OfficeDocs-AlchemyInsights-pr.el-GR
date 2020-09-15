---
title: σφάλμα 1554 Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698862"
---
# <a name="winsock-error-10061"></a>Σφάλμα Winsock 10061

Αυτός ο κωδικός σφάλματος σημαίνει ότι η Microsoft δεν μπόρεσε να δημιουργήσει μια υποδοχή TCP (σύνδεση) με τον κεντρικό υπολογιστή προορισμού. Η πιο πιθανή αιτία αυτού του σφάλματος είναι ένα πρόβλημα με τη ρύθμιση παραμέτρων του τείχους προστασίας σας. Για να διορθώσετε το πρόβλημα, ανατρέξτε σε αυτές τις ρυθμίσεις:

- Επαληθεύστε τη ρύθμιση παραμέτρων του τείχους προστασίας σας με τις πληροφορίες στις [διευθύνσεις URL και τις περιοχές διευθύνσεων IP του Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Εάν το σφάλμα αφορά συγκεκριμένα την προστασία του Exchange Online (EOP), θα έπρεπε να έχετε προηγουμένως ειδοποιηθεί για μια αλλαγή στις [ΔΙΕΥΘΎΝΣΕΙς IP του Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Βεβαιωθείτε ότι η υπηρεσία παροχής Internet (ISP) δεν αποκλείει τη θύρα.

- Επαληθεύστε τις ρυθμίσεις του έξυπνου κεντρικού υπολογιστή και του διακομιστή προορισμού στις γραμμές σύνδεσης.

Σημειώστε ότι το Microsoft 365 δεν αποκλείει τις *εισερχόμενες* συνδέσεις με αυτόν τον τρόπο.
