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
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="669ee-102">Προστασία από επίθεση Backscatter</span><span class="sxs-lookup"><span data-stu-id="669ee-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="669ee-103">Το backscatter είναι αναφορές μη παράδοσης (γνωστές και ως αναφορές NDR ή μηνύματα αναπήδησης) που λαμβάνετε για μηνύματα που δεν έχετε στείλει.</span><span class="sxs-lookup"><span data-stu-id="669ee-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="669ee-104">Οι αποστολείς ανεπιθύμητης αλληλογραφίας πλαστογραφούν (πλαστογραφούν) τη διεύθυνση **"Από":** των μηνυμάτων τους και συχνά χρησιμοποιούν πραγματικές διευθύνσεις ηλεκτρονικού ταχυδρομείου για να δώσουν αξιοπιστία στα μηνύματά τους.</span><span class="sxs-lookup"><span data-stu-id="669ee-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="669ee-105">Έτσι, όταν οι αποστολείς ανεπιθύμητης αλληλογραφίας στέλνουν αναπόφευκτα μηνύματα σε μη υπάρχων παραλήπτες, ο διακομιστής ηλεκτρονικού ταχυδρομείου προορισμού ουσιαστικά εξαπατάται για να επιστρέψει το μήνυμα που δεν παραδόθηκε σε μια NDR στον πλαστό αποστολέα στη διεύθυνση **Από:**</span><span class="sxs-lookup"><span data-stu-id="669ee-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="669ee-106">Μπορείτε να βρείτε πρόσθετες πληροφορίες [στο Backscatter στο EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="669ee-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="669ee-107">**Ενεργοποίηση της προστασίας backscatter**</span><span class="sxs-lookup"><span data-stu-id="669ee-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="669ee-108">Για να ενεργοποιήσετε την προστασία backscatter, ακολουθήστε την παρακάτω διαδρομή.</span><span class="sxs-lookup"><span data-stu-id="669ee-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="669ee-109">**protection.office.com > Πολιτική διαχείρισης απειλών > > Antispam > Επιλέξτε την πολιτική φίλτρου ανεπιθύμητης αλληλογραφίας και την πολιτική επεξεργασίας > Ιδιότητες ανεπιθύμητης αλληλογραφίας > Σήμανση ως ανεπιθύμητης αλληλογραφίας > Backscatter NDR > Ορίστε την σε "Ενεργοποιήστε"**</span><span class="sxs-lookup"><span data-stu-id="669ee-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="669ee-110">Εάν πιστεύετε ότι ένας λογαριασμός έχει παραβιαστεί, ανατρέξτε στα εξής:</span><span class="sxs-lookup"><span data-stu-id="669ee-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="669ee-111">Απάντηση σε λογαριασμό ηλεκτρονικού ταχυδρομείου που έχει παραβιαστεί</span><span class="sxs-lookup"><span data-stu-id="669ee-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="669ee-112">Κατάργηση αποκλεισμένων χρηστών από την πύλη "Περιορισμένοι χρήστες" στο Office 365</span><span class="sxs-lookup"><span data-stu-id="669ee-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



