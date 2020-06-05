---
title: Ζητήματα που σχετίζονται με την είσοδο στο Microsoft 365 εφαρμογές
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579901"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Κενή οθόνη εισόδου στις εφαρμογές Microsoft 365

Για να διορθώσετε αυτό το ζήτημα, δοκιμάστε τα εξής:
- Εγκαταστήστε τις πιο πρόσφατες ενημερωμένες εκδόσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [το Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Επαναφορά επιλογών του Internet Explorer: Μεταβείτε **στις επιλογές**  >  **Internet**  >  **Για προχωρημένους,** επαναφορά των  >  **ρυθμίσεων του Internet Explorer** (σημειώστε ότι θα χάσετε προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, προσπαθήστε να εισέλθετε ξανά στο Office.
- Απενεργοποιήστε το Windows Defender Application Guard (WDAG) ή οποιοδήποτε παρόμοιο τείχος προστασίας ή πρόγραμμα προστασίας από ιούς:
    1. Στον Πίνακα Ελέγχου, μεταβείτε στην **ενότητα Προγράμματα**και, στη συνέχεια, επιλέξτε **Ενεργοποίηση ή απενεργοποίηση δυνατοτήτων των Windows**.
    2. Εάν είναι ενεργοποιημένο το Windows Defender Application Guard, δοκιμάστε να τον απενεργοποιήσετε.<br/>
    **Σημείωση:** Ίσως χρειαστεί να επανεκκινήσετε τον υπολογιστή.
- Βεβαιωθείτε ότι η προσθήκη Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν αποκλείεται από οποιαδήποτε εφαρμογή ή πρόγραμμα τείχους προστασίας/προστασίας από ιούς.
- [Καταργήστε τις πιστοποιήσεις του Office χρησιμοποιώντας](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ζητήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση για τη δημιουργία του Office 2016 16.0.7967 στα Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).