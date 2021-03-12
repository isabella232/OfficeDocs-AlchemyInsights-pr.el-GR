---
title: Επιδιόρθωση πολιτικής μισθωτή (παράκαμψη ενέργειας)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745884"
---
# <a name="fix-tenant-policy-action-override"></a>Επιδιόρθωση πολιτικής μισθωτή (παράκαμψη ενέργειας)

Μια πολιτική καταπολέμησης της ανεπιθύμητης αλληλογραφίας στο μισθωτή σας επηρέασε αυτό το μήνυμα. Για να αναθεωρήσετε την πολιτική, κάντε τα εξής:

1. Μεταβείτε στο [Κέντρο ασφάλειας του Office 365 & και, στη](https://go.microsoft.com/fwlink/p/?linkid=2077143)συνέχεια, μεταβείτε στην πολιτική διαχείρισης **απειλών**  >    >  [κατά της ανεπιθύμητης αλληλογραφίας.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Ελέγξτε εάν  η προέλευση πολιτικής υποδεικνύει τα εξής: **Add-Xheader/ModifySubject/Redirect/Delete/No action/ Μήνυμα "BCC"**

    Εάν ναι, στην καρτέλα **"Προσαρμογή",** ελέγξτε τις ρυθμίσεις της πολιτικής που επηρέασε το μήνυμα. Είναι πιθανό οι τυπικές ρυθμίσεις που **εφαρμόστηκαν σε** όλους τους πελάτες του Exchange Online Protection να επηρέασαν το μήνυμα.

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση παραμέτρων των πολιτικών φίλτρου ανεπιθύμητης αλληλογραφίας, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων των πολιτικών φίλτρου ανεπιθύμητης αλληλογραφίας.](https://go.microsoft.com/fwlink/?linkid=2101431)
