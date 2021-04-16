---
title: Θέλετε να επισημάνετε έναν τομέα ή έναν αποστολέα ηλεκτρονικού ταχυδρομείου ως ασφαλή;
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792132"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="9d562-102">Θέλετε να επισημάνετε έναν τομέα ή έναν αποστολέα ηλεκτρονικού ταχυδρομείου ως ασφαλή;</span><span class="sxs-lookup"><span data-stu-id="9d562-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="9d562-103">Η χρήση **ασφαλών λιστών αποστολέων δεν συνιστάται,** καθώς ανοίγει τον οργανισμό σας σε επιθέσεις ανεπιθύμητης αλληλογραφίας, ηλεκτρονικού "ψαρέματος" και πλαστογράφησης.</span><span class="sxs-lookup"><span data-stu-id="9d562-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="9d562-104">Ωστόσο, εάν υπάρχει επιχειρηματική απαίτηση, συνιστάται να χρησιμοποιήσετε **τους** Κανόνες **[ροής αλληλογραφίας για](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** αυτό.</span><span class="sxs-lookup"><span data-stu-id="9d562-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="9d562-105">Οι οδηγίες μας διασφαλίζουν τον έλεγχο ταυτότητας αποστολέα (επαληθεύει ότι ο τομέας αποστολής δεν πλαστογραφήθηκε).</span><span class="sxs-lookup"><span data-stu-id="9d562-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="9d562-106">**Σημείωση:** Δεν συνιστάται η διαχείριση ψευδών θετικών με τη χρήση λιστών ασφαλών αποστολέων, επειδή οι εξαιρέσεις στο φιλτράρισμα ανεπιθύμητης αλληλογραφίας μπορούν να ανοίξουν τον οργανισμό σας σε επιθέσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="9d562-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="9d562-107">Εάν οι χρήστες σας λαμβάνουν μηνύματα που έχουν επισημανθεί εσφαλμένα ως ανεπιθύμητη αλληλογραφία ή ανεπιθύμητη αλληλογραφία, **[αναφέρετε μηνύματα και αρχεία στη Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="9d562-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="9d562-108">Οι ασφαλείς αποστολείς στο Outlook, τη λίστα επιτρεπόμενων  αποστολέων ή τη λίστα επιτρεπόμενων τομέων στις πολιτικές καταπολέμησης της ανεπιθύμητης αλληλογραφίας θα πρέπει να αποφεύγονται, επειδή οι αποστολείς παρακάμπτουν όλη την προστασία ανεπιθύμητης αλληλογραφίας, πλαστογράφησης και ηλεκτρονικού "ψαρέματος" και τον έλεγχο ταυτότητας αποστολέα (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="9d562-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="9d562-109">Αυτή η μέθοδος χρησιμοποιείται καλύτερα μόνο για προσωρινούς ελέγχους.</span><span class="sxs-lookup"><span data-stu-id="9d562-109">This method is best used for temporary testing only.</span></span>
