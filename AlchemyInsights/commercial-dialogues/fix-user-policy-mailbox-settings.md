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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034718"
---
# <a name="fix-user-policymailbox-settings"></a>Επιδιόρθωση ρυθμίσεων πολιτικής χρήστη/γραμματοκιβωτίου

Οι ρυθμίσεις ανεπιθύμητης αλληλογραφίας στο γραμματοκιβώτιο επηρέασαν αυτό το μήνυμα. Για να ελέγξετε τις ρυθμίσεις, κάντε τα εξής:

1. Εκκίνηση Exchange κελύφους διαχείρισης. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Άνοιγμα Exchange κελύφους διαχείρισης".](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Εκτελέστε αυτή την εντολή (χρησιμοποιώντας τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Ελέγξτε εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου του αποστολέα αποτελεί μέρος **του TrustedSendersAndDomains** ή **του BlockedSendersAndDomains.** Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου βρίσκεται σε μία από τις λίστες, ίσως χρειαστεί να την καταργήσετε. Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
