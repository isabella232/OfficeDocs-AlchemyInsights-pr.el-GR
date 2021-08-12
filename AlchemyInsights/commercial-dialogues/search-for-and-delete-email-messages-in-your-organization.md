---
title: Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948883"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας

Ακολουθήστε τα εξής βήματα:

1. Εάν δεν είστε καθολικός διαχειριστής, για να αναζητήσετε μηνύματα, ο λογαριασμός σας πρέπει να προστεθεί στην ομάδα ρόλων **της Διαχείρισης eDiscovery** ή στο ρόλο **διαχείρισης αναζήτησης συμμόρφωσης.** Για να διαγράψετε μηνύματα, θα πρέπει να συμμετάσχετε στην ομάδα ρόλων διαχείρισης **οργανισμού** ή στο ρόλο διαχείρισης αναζήτησης **και εκκαθάρισης.** Τα δικαιώματα σε αυτούς τους ρόλους εκχωρούνται στο [κέντρο & ασφάλειας.](https://protection.office.com)
2. [Δημιουργήστε μια αναζήτηση περιεχομένου για](https://docs.microsoft.com/office365/securitycompliance/content-search) να βρείτε το μήνυμα που θα διαγράψετε.
3. [Σύνδεση στο PowerShell & ασφάλειας και συμμόρφωσης.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Εάν χρησιμοποιείτε MFA, ανατρέξτε στις παρακάτω οδηγίες: Σύνδεση στην ασφάλεια [& PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων
4. Διαγράψτε το μήνυμα: εκτελέστε `New-ComplianceSearchAction` το cmdlet για να διαγράψετε το μήνυμα. Τα διαγραμμένα μηνύματα μετακινούνται στο φάκελο "Ανακτήσιμα" ενός χρήστη. Για ένα παράδειγμα εντολής, [ανατρέξτε στο βήμα 3: Διαγραφή του μηνύματος.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
