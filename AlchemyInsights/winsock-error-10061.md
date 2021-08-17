---
title: Σφάλμα 1554 Winsock 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083230"
---
# <a name="winsock-error-10061"></a>Σφάλμα Winsock 10061

Αυτός ο κωδικός σφάλματος σημαίνει ότι η Microsoft δεν μπόρεσε να δημιουργήσει μια υποδοχή TCP (σύνδεση) με τον κεντρικό υπολογιστή προορισμού. Η πιο πιθανή αιτία αυτού του σφάλματος είναι ένα πρόβλημα με τη ρύθμιση παραμέτρων του τείχους προστασίας. Για να διορθώσετε το πρόβλημα, ελέγξτε αυτές τις ρυθμίσεις:

- Επαληθεύστε τη ρύθμιση παραμέτρων του τείχους προστασίας με [τις πληροφορίες Microsoft 365 διευθύνσεων URL και διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Εάν το σφάλμα αφορά συγκεκριμένα Exchange Online Protection (EOP), θα έπρεπε να είχατε προηγουμένως ειδοποιηθεί για μια αλλαγή στις [Exchange Online Protection IP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Βεβαιωθείτε ότι η υπηρεσία παροχής Internet (ISP) που χρησιμοποιείτε δεν αποκλείει τη θύρα.

- Επαληθεύστε τις ρυθμίσεις του έξυπνου κεντρικού υπολογιστή και του διακομιστή προορισμού στις συνδέσεις σας.

Σημειώστε ότι Microsoft 365 δεν αποκλείονται οι *εισερχόμενες συνδέσεις* με αυτόν τον τρόπο.
