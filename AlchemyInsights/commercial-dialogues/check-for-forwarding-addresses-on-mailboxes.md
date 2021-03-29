---
title: Έλεγχος για προώθηση διευθύνσεων σε γραμματοκιβώτια
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403311"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="dad75-102">Έλεγχος για προώθηση διευθύνσεων σε γραμματοκιβώτια</span><span class="sxs-lookup"><span data-stu-id="dad75-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="dad75-103">Μερικές φορές οι εισβολείς προβιβάουν τα μηνύματα ηλεκτρονικού ταχυδρομείου των χρηστών στον εαυτό τους, επομένως πρώτα θα ελέγξουμε για προώθηση διευθύνσεων και κανόνων στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="dad75-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="dad75-104">Στη συνέχεια, θα ελέγξουμε τα αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="dad75-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="dad75-105">Δείτε πώς μπορείτε να ελέγξετε για διευθύνσεις προώθησης:</span><span class="sxs-lookup"><span data-stu-id="dad75-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="dad75-106">Επιλέξτε **"Χρήστες**  >  **ενεργοί χρήστες".**</span><span class="sxs-lookup"><span data-stu-id="dad75-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="dad75-107">Επιλέξτε το χρήστη του οποίου ο λογαριασμός έχει παραβιαστεί.</span><span class="sxs-lookup"><span data-stu-id="dad75-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="dad75-108">Στο αναδυόμενο στοιχείο που εμφανίζεται, αναπτύξτε τις Ρυθμίσεις αλληλογραφίας και, **στη** συνέχεια, κάντε κλικ στην επιλογή **"Επεξεργασία** **για προώθηση ηλεκτρονικού ταχυδρομείου".**</span><span class="sxs-lookup"><span data-stu-id="dad75-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="dad75-109">Καταργήστε τυχόν διευθύνσεις προώθησης που δεν αναγνωρίζετε.</span><span class="sxs-lookup"><span data-stu-id="dad75-109">Remove any forwarding addresses you don't recognize.</span></span>