---
title: 726 Αποκλεισμός προώθησης ηλεκτρονικού ταχυδρομείου
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059632"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Αποκλεισμός ή κατάργηση αποκλεισμού προώθησης ηλεκτρονικού ταχυδρομείου

Για να ενεργοποιήσετε ή να απενεργοποιήσετε την προώθηση ηλεκτρονικού ταχυδρομείου για ένα συγκεκριμένο γραμματοκιβώτιο, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων προώθησης ηλεκτρονικού ταχυδρομείου.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Σε επίπεδο μισθωτή, ο έλεγχος της εξωτερικής προώθησης γίνεται με χρήση της πολιτικής εξερχόμενης ανεπιθύμητης αλληλογραφίας. Μπορείτε να ελέγξετε την πολιτική φίλτρου [](https://protection.office.com/antispam) εξερχόμενης ανεπιθύμητης αλληλογραφίας από το Κέντρο ασφάλειας και συμμόρφωσης εδώ ή χρησιμοποιώντας την εντολή [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Εάν εμφανίζεται το ακόλουθο σφάλμα: "Δεν επιτρέπεται η πρόσβαση **550 5.7.520,** η εταιρεία σας δεν επιτρέπει την εξωτερική προώθηση", βεβαιωθείτε ότι η πολιτική έχει ρυθμιστεί ώστε να ενεργοποιεί την Εξωτερική Αυτόματη προώθηση.

**Σημείωση:** Συνιστάται να διατηρήσετε απενεργοποιημένη την εξωτερική αυτόματη προστασία στην προεπιλεγμένη πολιτική φίλτρου εξερχόμενης ανεπιθύμητης αλληλογραφίας και να την ενεργοποιήσετε μόνο για τους χρήστες που χρειάζονται εξωτερική προώθηση, δημιουργώντας μια προσαρμοσμένη πολιτική για αυτούς τους χρήστες. Μπορείτε να διαβάσετε περισσότερα στην επιλογή ["Ρύθμιση παραμέτρων εξωτερικής προώθησης ηλεκτρονικού ταχυδρομείου" Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)