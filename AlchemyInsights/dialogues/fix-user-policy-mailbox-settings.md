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
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="8443a-102">Επιδιόρθωση ρυθμίσεων πολιτικής χρήστη/γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="8443a-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="8443a-103">Οι ρυθμίσεις ανεπιθύμητης αλληλογραφίας στο γραμματοκιβώτιο επηρέασαν αυτό το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="8443a-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="8443a-104">Για να δείτε τις ρυθμίσεις, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="8443a-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="8443a-105">Εκκινούν το Κέλυφος διαχείρισης Exchange.</span><span class="sxs-lookup"><span data-stu-id="8443a-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="8443a-106">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Άνοιγμα κελύφους διαχείρισης Exchange".](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="8443a-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="8443a-107">Εκτελέστε αυτή την εντολή (χρησιμοποιώντας τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="8443a-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="8443a-108">Ελέγξτε εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου του αποστολέα είναι μέρος των αξιόπιστων **διευθύνσεων TrustedSendersAndDomains** ή **BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="8443a-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="8443a-109">Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σε μία από τις λίστες, ίσως χρειαστεί να την καταργήσετε.</span><span class="sxs-lookup"><span data-stu-id="8443a-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="8443a-110">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="8443a-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
