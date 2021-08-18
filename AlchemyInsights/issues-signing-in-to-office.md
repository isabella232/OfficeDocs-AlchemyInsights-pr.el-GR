---
title: Προβλήματα κατά την είσοδο σε Microsoft 365 εφαρμογών
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088036"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Κενή οθόνη σύνδεσης σε Microsoft 365 εφαρμογές

Για να διορθώσετε αυτό το πρόβλημα, δοκιμάστε τα εξής:
- Εγκαταστήστε τις πιο πρόσφατες ενημερώσεις [για Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Επαναφορά επιλογών του Internet Explorer: Μεταβείτε στην επιλογή "Εργαλεία internet  >  **Options**  >  **Advanced** Reset Internet  >  **Explorer Ρυθμίσεις"** (σημειώστε ότι θα χάσετε τις προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, δοκιμάστε να εισέλθετε στο Office ξανά.
- Απενεργοποιήστε το Windows Defender Application Guard (WDAG) ή οποιοδήποτε παρόμοιο τείχος προστασίας ή πρόγραμμα προστασίας από ιούς:
    1. Στον Πίνακα Ελέγχου, μεταβείτε στην επιλογή **"Προγράμματα"** και, στη συνέχεια, **Windows ενεργοποίηση ή απενεργοποίηση των δυνατοτήτων.**
    2. Εάν Windows Defender Application Guard είναι ενεργοποιημένη, δοκιμάστε να την απενεργοποιήσετε.<br/>
    **Σημείωση:** Ίσως χρειαστεί να επανεκκινήσετε τον υπολογιστή.
- Βεβαιωθείτε ότι η προσθήκη Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν έχει αποκλειστεί από καμία εφαρμογή ή πρόγραμμα τείχους προστασίας/προστασίας από ιούς.
- [Καταργήστε Office διαπιστευτηρίων χρησιμοποιώντας](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Διαχείριση διαπιστευτηρίων.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για Office 2016 έχουν αλλάξει σε 16.0. (Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Προβλήματα σύνδεσης κατά την είσοδο μετά την [ενημέρωση στη Office 2016, έκδοση 16.0.7967 στο Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)