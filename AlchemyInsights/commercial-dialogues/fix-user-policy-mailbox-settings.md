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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746727"
---
# <a name="fix-user-policymailbox-settings"></a>Επιδιόρθωση ρυθμίσεων πολιτικής χρήστη/γραμματοκιβωτίου

Οι ρυθμίσεις ανεπιθύμητης αλληλογραφίας στο γραμματοκιβώτιο επηρέασαν αυτό το μήνυμα. Για να ελέγξετε τις ρυθμίσεις, κάντε τα εξής:

1. Εκκινεί το κέλυφος διαχείρισης του Exchange. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Άνοιγμα του κελύφους διαχείρισης του Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Εκτελέστε αυτή την εντολή (χρησιμοποιώντας τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Ελέγξτε εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου του αποστολέα αποτελεί μέρος **του TrustedSendersAndDomains** ή **του BlockedSendersAndDomains.** Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου βρίσκεται σε μία από τις λίστες, ίσως χρειαστεί να την καταργήσετε. Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
