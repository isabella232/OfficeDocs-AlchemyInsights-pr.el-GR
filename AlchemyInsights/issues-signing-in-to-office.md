---
title: Θέματα είσοδο σε εφαρμογές του Office
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938223"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Οθόνη κενή εισόδου σε εφαρμογές του Office

Για να διορθώσετε αυτό το ζήτημα, δοκιμάστε τα εξής:
- Εγκαταστήστε τις τελευταίες ενημερωμένες εκδόσεις για [Windows](https://support.microsoft.com/help/4027667/windows-10-update) και του [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Επαναφέρετε τις επιλογές του Internet Explorer: Μετάβαση σε **Εργαλεία** > **Επιλογές Internet** > **για προχωρημένους** > **Επαναφοράς ρυθμίσεων Internet Explorer** (Σημειώστε ότι θα χάσετε προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, προσπαθήστε να εισέλθετε ξανά στο Office.
- Απενεργοποιήστε το Windows Defender εφαρμογής προστασίας (WDAG) ή οποιοδήποτε παρόμοιο πρόγραμμα προστασίας από ιούς ή τείχους προστασίας:
    1. Στον πίνακα ελέγχου, μεταβείτε σε **προγράμματα**και, στη συνέχεια, επιλέξτε **Ενεργοποίηση δυνατοτήτων των Windows ή να απενεργοποιήσετε**.
    2. Εάν είναι ενεργοποιημένη η προστασία εφαρμογών του Windows Defender, δοκιμάστε να την απενεργοποιήσετε.<br/>
    **Σημείωση:** Ίσως χρειαστεί να κάνετε επανεκκίνηση του υπολογιστή.
- Βεβαιωθείτε ότι το Microsoft.AAD.BrokerPlugin [AAD WAM προσθήκης](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν είναι αποκλεισμένο από οποιαδήποτε εφαρμογή ή ένα πρόγραμμα τείχους προστασίας/κατά-virus.
- [Απαλοιφή Office διαπιστευτήρια](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [ζητήματα σύνδεσης στο είσοδος μετά την ενημερωμένη έκδοση του Office 2016 build 16.0.7967 σε Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).