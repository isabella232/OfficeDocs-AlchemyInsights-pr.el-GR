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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694064"
---
# <a name="fix-tenant-policy-action-override"></a>Επιδιόρθωση πολιτικής μισθωτή (παράκαμψη ενέργειας)

Μια πολιτική καταπολέμησης της ανεπιθύμητης αλληλογραφίας στο μισθωτή σας επηρέασα αυτό το μήνυμα. Για να εξετάσετε την πολιτική, κάντε τα εξής:

1. Μεταβείτε στο Κέντρο [συμμόρφωσης ασφαλείας του Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143)και, στη συνέχεια, μεταβείτε στην **Πολιτική** διαχείρισης  >  **απειλών κατά** της  >  [ανεπιθύμητης αλληλογραφίας.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Ελέγξτε εάν  η προέλευση πολιτικής υποδεικνύει τα εξής: **Add-Xheader/ModifySubject/Redirect/Delete/No action/ Μήνυμα "BCC"**

    Εάν ναι, στην καρτέλα **"Προσαρμογή",** ελέγξτε τις ρυθμίσεις της πολιτικής που επηρέασαν το μήνυμα. Είναι πιθανό οι Τυπικές ρυθμίσεις που **εφαρμόζονται σε** όλους τους πελάτες του Exchange Online Protection να επηρέασαν το μήνυμα.

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση παραμέτρων των πολιτικών φίλτρου ανεπιθύμητης αλληλογραφίας, ανατρέξτε στο θέμα ["Ρύθμιση παραμέτρων των πολιτικών φίλτρου ανεπιθύμητης αλληλογραφίας".](https://go.microsoft.com/fwlink/?linkid=2101431)
