---
title: 1332 OWA - κανόνες εισερχομένων δεν εκτελούνται για ένα γραμματοκιβώτιο
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204060"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Έναν κανόνα εισερχομένων δεν λειτουργεί όπως αναμένεται

Επαληθεύστε τις παρακάτω ρυθμίσεις:

- Ένα μήνυμα μπορεί να ανακατευθυνθεί, προωθούνται ή αποστέλλεται απάντηση σε αυτόματα, με βάση κανόνες εισερχομένων μόνο μία φορά. Ανακατεύθυνση κανόνα (έναν κανόνα εισερχομένων ή κανόνα ροής αλληλογραφίας, γνωστή και ως έναν κανόνα μεταφοράς) να προσθέσετε έως και δέκα προώθησης παραλήπτες σε ένα μήνυμα. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Εισερχόμενα εγγραφών, μεταφορά, και τα όρια του κανόνα](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Κανόνες εισερχομένων δεν λειτουργούν στο γραμματοκιβώτιο εναλλακτική καταγραφή στο χρονικό. Για περισσότερες πληροφορίες σχετικά με το γραμματοκιβώτιο του εναλλακτικού καταγραφή στο χρονικό, δείτε [εναλλακτικό καταγραφή στο χρονικό γραμματοκιβώτιο](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Για να διορθώσετε αυτά τα ζητήματα, ανατρέξτε στην ενότητα [KB 2829319](https://support.microsoft.com/kb/2829319).

Εάν δεν εφαρμόσετε τα προηγούμενα θέματα, εκτέλεση της διαγνωστικής έκθεσης κανόνα εισερχομένων πριν προωθήσετε το ζήτημα στην υποστήριξη της Microsoft:

1. Ανοίξτε το γραμματοκιβώτιο στο Outlook στο web και κάντε κλικ στο κουμπί <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Ρυθμίσεις** > **προβάλετε όλες τις ρυθμίσεις Outlook** > **Mail** > **κανόνες**.

2. Στο κάτω μέρος της σελίδας, κάντε κλικ στο κουμπί **Εάν τους κανόνες σας δεν λειτουργούν κάντε κλικ εδώ για να δημιουργήσετε μια διαγνωστική έκθεση**.
