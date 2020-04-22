---
title: Εξερχόμενο μήνυμα ηλεκτρονικού ταχυδρομείου στο φάκελο ανεπιθύμητης αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761168"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="b689e-102">Εξερχόμενο μήνυμα ηλεκτρονικού ταχυδρομείου στο φάκελο ανεπιθύμητης αλληλογραφίας</span><span class="sxs-lookup"><span data-stu-id="b689e-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="b689e-103">Εάν βλέπετε τα εξερχόμενα μηνύματα να επισημαίνονται ως Ανεπιθύμητα, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="b689e-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="b689e-104">Εάν δεν το έχετε κάνει ήδη, εξετάστε το ενδεχόμενο [να ρυθμίσετε τις παραμέτρους των εξερχόμενων ειδοποιήσεων πολιτικής ανεπιθύμητης αλληλογραφίας](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="b689e-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="b689e-105">Χρησιμοποιήστε [την ανίχνευση μηνυμάτων](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) για να δείτε αν το εξερχόμενο μήνυμα έχει την τιμή συμβάντος **Ανεπιθύμητη αλληλογραφία** με τις πρόσθετες λεπτομέρειες: Χρήση χώρου **συγκέντρωσης παράδοσης υψηλού κινδύνου**.</span><span class="sxs-lookup"><span data-stu-id="b689e-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="b689e-106">Για αυτά τα μηνύματα, ελέγξτε το περιεχόμενο του μηνύματος για να δείτε τι μπορεί να θεωρηθεί ανεπιθύμητο.</span><span class="sxs-lookup"><span data-stu-id="b689e-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="b689e-107">Για παράδειγμα, οι υπογραφές μπορεί μερικές φορές να προκαλέσουν προβλήματα σε πολλούς χρήστες.</span><span class="sxs-lookup"><span data-stu-id="b689e-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="b689e-108">Εάν έχετε πολλά παραδείγματα νόμιμων εξερχόμενων μηνυμάτων που επισημαίνονται ως Ανεπιθύμητα, ανοίξτε ένα δελτίο υποστήριξης και ζητήστε από τον παράγοντα υποστήριξης να υποβάλει τα μηνύματά σας ως ψευδώς θετικά στους αναλυτές ανεπιθύμητων μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="b689e-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="b689e-109">Προετοιμαστείτε να παρέχετε δείγματα μηνυμάτων που περιλαμβάνουν όλες τις κεφαλίδες μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="b689e-109">Be prepared to provide sample messages that include all message headers.</span></span>
