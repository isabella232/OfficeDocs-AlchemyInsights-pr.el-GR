---
title: Προστασία από επίθεση Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036071"
---
# <a name="protection-from-backscatter-attack"></a>Προστασία από επίθεση Backscatter

Το backscatter είναι αναφορές μη παράδοσης (γνωστές και ως αναφορές NDR ή μηνύματα αναπήδησης) που λαμβάνετε για μηνύματα που δεν έχετε στείλει. Οι αποστολείς ανεπιθύμητης αλληλογραφίας πλαστογραφούν (πλαστογραφούν) τη διεύθυνση **"Από":** των μηνυμάτων τους και συχνά χρησιμοποιούν πραγματικές διευθύνσεις ηλεκτρονικού ταχυδρομείου για να δώσουν αξιοπιστία στα μηνύματά τους. Έτσι, όταν οι αποστολείς ανεπιθύμητης αλληλογραφίας στέλνουν αναπόφευκτα μηνύματα σε μη υπάρχων παραλήπτες, ο διακομιστής ηλεκτρονικού ταχυδρομείου προορισμού ουσιαστικά εξαπατάται για να επιστρέψει το μήνυμα που δεν παραδόθηκε σε μια NDR στον πλαστό αποστολέα στη διεύθυνση **Από:**

Μπορείτε να βρείτε πρόσθετες πληροφορίες [στο Backscatter στο EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**Ενεργοποίηση της προστασίας backscatter**

Για να ενεργοποιήσετε την προστασία backscatter, ακολουθήστε την παρακάτω διαδρομή.

**protection.office.com > Πολιτική διαχείρισης απειλών > > Antispam > Επιλέξτε την πολιτική φίλτρου ανεπιθύμητης αλληλογραφίας και την πολιτική επεξεργασίας > Ιδιότητες ανεπιθύμητης αλληλογραφίας > Σήμανση ως ανεπιθύμητης αλληλογραφίας > Backscatter NDR > Ορίστε την σε "Ενεργοποιήστε"**

Εάν πιστεύετε ότι ένας λογαριασμός έχει παραβιαστεί, ανατρέξτε στα εξής:

- [Απάντηση σε λογαριασμό ηλεκτρονικού ταχυδρομείου που έχει παραβιαστεί](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Κατάργηση αποκλεισμένων χρηστών από την πύλη "Περιορισμένοι χρήστες" στο Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



