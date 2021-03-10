---
title: Επιδιόρθωση ρυθμίσεων πολιτικής χρήστη/γραμματοκιβωτίου
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694176"
---
# <a name="fix-user-policymailbox-settings"></a>Επιδιόρθωση ρυθμίσεων πολιτικής χρήστη/γραμματοκιβωτίου

Οι ρυθμίσεις ανεπιθύμητης αλληλογραφίας στο γραμματοκιβώτιο επηρέασαν αυτό το μήνυμα. Για να δείτε τις ρυθμίσεις, κάντε τα εξής:

1. Εκκινούν το Κέλυφος διαχείρισης Exchange. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Άνοιγμα κελύφους διαχείρισης Exchange".](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Εκτελέστε αυτή την εντολή (χρησιμοποιώντας τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Ελέγξτε εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου του αποστολέα είναι μέρος των αξιόπιστων **διευθύνσεων TrustedSendersAndDomains** ή **BlockedSendersAndDomains.** Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σε μία από τις λίστες, ίσως χρειαστεί να την καταργήσετε. Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
