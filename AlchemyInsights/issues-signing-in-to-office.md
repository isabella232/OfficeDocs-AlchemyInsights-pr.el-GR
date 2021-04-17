---
title: Προβλήματα κατά την είσοδο σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833039"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Κενή οθόνη σύνδεσης σε εφαρμογές του Microsoft 365

Για να διορθώσετε αυτό το πρόβλημα, δοκιμάστε τα εξής:
- Εγκαταστήστε τις πιο πρόσφατες ενημερώσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [το Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Επαναφορά επιλογών του Internet Explorer: Μεταβείτε στην επιλογή "Εργαλεία internet  >  **Options**  >  **Advanced** Reset Internet  >  **Explorer Settings"** (σημειώστε ότι θα χάσετε τις προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, δοκιμάστε να εισέλθετε ξανά στο Office.
- Απενεργοποιήστε το Windows Defender Application Guard (WDAG) ή οποιοδήποτε παρόμοιο τείχος προστασίας ή πρόγραμμα προστασίας από ιούς:
    1. Στον Πίνακα Ελέγχου, μεταβείτε στην επιλογή **"Προγράμματα"** και, στη συνέχεια, επιλέξτε "Ενεργοποίηση ή **απενεργοποίηση των δυνατοτήτων των Windows".**
    2. Εάν είναι ενεργοποιημένο το Windows Defender Application Guard, δοκιμάστε να το απενεργοποιήσετε.<br/>
    **Σημείωση:** Ίσως χρειαστεί να επανεκκινήσετε τον υπολογιστή.
- Βεβαιωθείτε ότι η προσθήκη Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν έχει αποκλειστεί από καμία εφαρμογή ή πρόγραμμα τείχους προστασίας/προστασίας από ιούς.
- [Καταργήστε τα διαπιστευτήρια του Office χρησιμοποιώντας](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0. (Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Προβλήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση στη δόμηση [16.0.7967 του Office 2016 στα Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)