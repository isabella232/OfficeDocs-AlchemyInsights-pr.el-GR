---
title: Αποκλεισμός ή κατάργηση αποκλεισμού της εξωτερικής αυτόματης προώθησης μηνυμάτων ηλεκτρονικού ταχυδρομείου
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897468"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Αποκλεισμός ή κατάργηση αποκλεισμού της αιωνίου αυτόματης προώθησης μηνυμάτων ηλεκτρονικού ταχυδρομείου

Για να ενεργοποιήσετε ή να απενεργοποιήσετε την προώθηση ηλεκτρονικού ταχυδρομείου για ένα συγκεκριμένο γραμματοκιβώτιο, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων προώθησης ηλεκτρονικού ταχυδρομείου.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Οι διαχειριστές μπορούν να ελέγχουν την εξωτερική προώθηση για τον οργανισμό χρησιμοποιώντας πολιτικές [εξερχόμενης ανεπιθύμητης αλληλογραφίας.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Μπορείτε να διαχειριστείτε τις πολιτικές εξερχόμενης ανεπιθύμητης αλληλογραφίας στην πύλη Microsoft 365 Defender ή χρησιμοποιώντας το <https://security.microsoft.com/antispam> [cmdlet Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) στο Exchange Online PowerShell.

Εάν εμφανιστεί το ακόλουθο σφάλμα: "Δεν επιτρέπεται η πρόσβαση **550 5.7.520,** ο οργανισμός σας δεν επιτρέπει την εξωτερική προώθηση", βεβαιωθείτε ότι η πολιτική έχει ρυθμιστεί ώστε να ενεργοποιεί εξωτερικά μηνύματα αυτόματης προώθησης.

**Σημείωση:** Συνιστάται η προεπιλεγμένη τιμή **"Αυτόματη" -** Το σύστημα ελέγχεται για τη ρύθμιση κανόνων αυτόματης προώθησης στην προεπιλεγμένη πολιτική φίλτρου ανεπιθύμητης αλληλογραφίας εξερχομένων (η αυτόματη εξωτερική προώθηση έχει αποκλειστεί, ενώ η εσωτερική αυτόματη προώθηση εξακολουθεί να λειτουργεί).  Θα πρέπει να δημιουργήσετε προσαρμοσμένες πολιτικές φίλτρου εξερχόμενης ανεπιθύμητης αλληλογραφίας και να χρησιμοποιήσετε την τιμή **"Ενεργό" -** Η προώθηση είναι ενεργοποιημένη μόνο για τους χρήστες που χρειάζονται εξωτερική αυτόματη προώθηση μηνυμάτων ηλεκτρονικού ταχυδρομείου. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Ρύθμιση παραμέτρων εξωτερικής προώθησης ηλεκτρονικού ταχυδρομείου Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
