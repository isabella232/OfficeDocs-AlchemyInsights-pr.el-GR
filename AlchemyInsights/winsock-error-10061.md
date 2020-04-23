---
title: 1554 Σφάλμα Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766169"
---
# <a name="winsock-error-10061"></a>Σφάλμα Winsock 10061

Αυτός ο κωδικός σφάλματος σημαίνει ότι η Microsoft δεν ήταν δυνατή η δημιουργία μιας υποδοχής TCP (σύνδεση) με τον κεντρικό υπολογιστή προορισμού. Η πιο πιθανή αιτία αυτού του σφάλματος είναι ένα πρόβλημα με τις παραμέτρους του τείχους προστασίας. Για να διορθώσετε το πρόβλημα, ελέγξτε αυτές τις ρυθμίσεις:

- Επαληθεύστε τις παραμέτρους του τείχους προστασίας σας με τις πληροφορίες στις [διευθύνσεις URL και τις περιοχές διευθύνσεων IP της Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Εάν το σφάλμα αφορά συγκεκριμένα την Ηλεκτρονική προστασία του Exchange (EOP), θα πρέπει να έχετε ειδοποιηθεί προηγουμένως για αλλαγή στις [διευθύνσεις IP ηλεκτρονικής προστασίας του Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Βεβαιωθείτε ότι η υπηρεσία παροχής Internet (ISP) δεν αποκλείει τη θύρα.

- Επαληθεύστε τις ρυθμίσεις του έξυπνου κεντρικού υπολογιστή και του διακομιστή προορισμού στις συνδέσεις σας.

Σημειώστε ότι το Microsoft 365 δεν αποκλείει *τις εισερχόμενες* συνδέσεις με αυτόν τον τρόπο.
