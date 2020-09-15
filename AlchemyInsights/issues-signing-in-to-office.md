---
title: Προβλήματα κατά την είσοδο σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695287"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Κενή οθόνη εισόδου στις εφαρμογές του Microsoft 365

Για να διορθώσετε αυτό το πρόβλημα, δοκιμάστε τα εξής:
- Εγκαταστήστε τις πιο πρόσφατες ενημερώσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και το [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Επαναφορά επιλογών του Internet Explorer: μεταβείτε στις επιλογές **Εργαλεία**  >  **Internet**για  >  **προχωρημένους**  >  **Επαναφορά ρυθμίσεων του Internet Explorer** (Σημειώστε ότι θα χάσετε τις προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, δοκιμάστε να συνδεθείτε στο Office ξανά.
- Απενεργοποιήστε το προστατευτικό εφαρμογής του Windows Defender (WDAG) ή οποιοδήποτε παρόμοιο τείχος προστασίας ή πρόγραμμα εντοπισμού ιών:
    1. Στον πίνακα ελέγχου, μεταβείτε στην επιλογή **προγράμματα**και, στη συνέχεια, επιλέξτε **Ενεργοποίηση ή απενεργοποίηση δυνατοτήτων των Windows**.
    2. Εάν είναι ενεργοποιημένη η προστασία εφαρμογών του Windows Defender, δοκιμάστε να την απενεργοποιήσετε.<br/>
    **Σημείωση:** Ίσως χρειαστεί να επανεκκινήσετε τον υπολογιστή σας.
- Βεβαιωθείτε ότι η προσθήκη του Microsoft. AAD. BrokerPlugin [AAD](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν εμποδίζεται από οποιαδήποτε εφαρμογή ή πρόγραμμα τείχους προστασίας/προστασίας από ιούς.
- [Καταργήστε τα διαπιστευτήρια του Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0. (Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα προβλήματα σύνδεσης στην είσοδο μετά την ενημέρωση στο Office 2016 Δόμηση 16.0.7967 στα Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).