---
title: Εξερχόμενο μήνυμα ηλεκτρονικού ταχυδρομείου στο φάκελο ανεπιθύμητης αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769183"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="6da40-102">Εξερχόμενο μήνυμα ηλεκτρονικού ταχυδρομείου στο φάκελο ανεπιθύμητης αλληλογραφίας</span><span class="sxs-lookup"><span data-stu-id="6da40-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="6da40-103">Εάν βλέπετε τα μηνύματα εξερχομένων να επισημαίνονται ως ανεπιθύμητη αλληλογραφία, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="6da40-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="6da40-104">Εάν δεν το έχετε κάνει ήδη, εξετάστε το ενδεχόμενο να [ρυθμίσετε τις ειδοποιήσεις πολιτικής εξερχόμενων ανεπιθύμητων μηνυμάτων](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="6da40-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="6da40-105">Χρησιμοποιήστε την [Ανίχνευση μηνύματος](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) για να δείτε εάν το μήνυμα εξερχομένων έχει την τιμή συμβάντος **spam** με τις πρόσθετες λεπτομέρειες: **Χρησιμοποιήστε το χώρο συγκέντρωσης παράδοσης υψηλού κινδύνου**.</span><span class="sxs-lookup"><span data-stu-id="6da40-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="6da40-106">Για αυτά τα μηνύματα, επιλέξτε το περιεχόμενο του μηνύματος για να δείτε τι μπορεί να θεωρηθεί ανεπιθύμητη αλληλογραφία.</span><span class="sxs-lookup"><span data-stu-id="6da40-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="6da40-107">Για παράδειγμα, οι υπογραφές μπορεί μερικές φορές να προκαλέσουν προβλήματα για πολλούς χρήστες.</span><span class="sxs-lookup"><span data-stu-id="6da40-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="6da40-108">Εάν έχετε πολλά παραδείγματα νομίμων εξερχόμενων μηνυμάτων που επισημαίνονται ως ανεπιθύμητη αλληλογραφία, ανοίξτε ένα δελτίο υποστήριξης και ζητήστε από τον αντιπρόσωπο υποστήριξης να υποβάλει τα μηνύματά σας ως ψευδώς θετικά στους αναλυτές ανεπιθύμητης αλληλογραφίας.</span><span class="sxs-lookup"><span data-stu-id="6da40-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="6da40-109">Να είστε προετοιμασμένοι για την παροχή δειγμάτων μηνυμάτων που περιλαμβάνουν όλες τις κεφαλίδες μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="6da40-109">Be prepared to provide sample messages that include all message headers.</span></span>
