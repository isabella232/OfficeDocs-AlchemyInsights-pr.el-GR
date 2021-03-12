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
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="d1306-102">Επιδιόρθωση ρυθμίσεων πολιτικής χρήστη/γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="d1306-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="d1306-103">Οι ρυθμίσεις ανεπιθύμητης αλληλογραφίας στο γραμματοκιβώτιο επηρέασαν αυτό το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="d1306-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="d1306-104">Για να ελέγξετε τις ρυθμίσεις, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="d1306-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="d1306-105">Εκκινεί το κέλυφος διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1306-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="d1306-106">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Άνοιγμα του κελύφους διαχείρισης του Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="d1306-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="d1306-107">Εκτελέστε αυτή την εντολή (χρησιμοποιώντας τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="d1306-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="d1306-108">Ελέγξτε εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου του αποστολέα αποτελεί μέρος **του TrustedSendersAndDomains** ή **του BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="d1306-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="d1306-109">Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου βρίσκεται σε μία από τις λίστες, ίσως χρειαστεί να την καταργήσετε.</span><span class="sxs-lookup"><span data-stu-id="d1306-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="d1306-110">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="d1306-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
