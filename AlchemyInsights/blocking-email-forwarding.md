---
title: 726 αποκλεισμός προώθησης ηλεκτρονικού ταχυδρομείου
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478344"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Αποκλεισμός ή κατάργηση αποκλεισμού προώθησης ηλεκτρονικού ταχυδρομείου

Για να ενεργοποιήσετε ή να απενεργοποιήσετε την προώθηση μηνυμάτων ηλεκτρονικού ταχυδρομείου για ένα συγκεκριμένο γραμματοκιβώτιο, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων προώθησης ηλεκτρονικού ταχυδρομείου](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Στο επίπεδο μισθωτών, ο έλεγχος της εξωτερικής προώθησης γίνεται με χρήση της πολιτικής ανεπιθύμητης αλληλογραφίας εξερχομένων. Μπορείτε να επιλέξετε την πολιτική φιλτραρίσματος ανεπιθύμητης αλληλογραφίας από το κέντρο ασφάλειας και συμμόρφωσης [εδώ](https://protection.office.com/antispam) ή χρησιμοποιώντας την [εντολή Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Εάν λαμβάνετε το ακόλουθο μήνυμα σφάλματος: **"δεν επιτρέπεται η πρόσβαση του 550 5.7.520, η εταιρεία σας δεν επιτρέπει την εξωτερική προώθηση"**, βεβαιωθείτε ότι η πολιτική έχει ρυθμιστεί ώστε να ενεργοποιεί την εξωτερική αυτόματη προώθηση.

**Σημείωση:** Συνιστάται να διατηρήσετε την εξωτερική προώθηση απενεργοποιημένη στην προεπιλεγμένη πολιτική φίλτρου ανεπιθύμητης αλληλογραφίας και να την ενεργοποιήσετε μόνο για τους χρήστες που χρειάζονται εξωτερική προώθηση με τη δημιουργία μιας προσαρμοσμένης πολιτικής για αυτούς τους χρήστες. Μπορείτε να διαβάσετε περισσότερα στη [Ρύθμιση παραμέτρων εξωτερικής προώθησης ηλεκτρονικού ταχυδρομείου στο Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).