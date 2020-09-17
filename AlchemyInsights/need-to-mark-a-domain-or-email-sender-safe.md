---
title: Πρέπει να επισημάνετε έναν τομέα ή έναν αποστολέα ηλεκτρονικού ταχυδρομείου ασφαλή;
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803245"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="2a221-102">Πρέπει να επισημάνετε έναν τομέα ή έναν αποστολέα ηλεκτρονικού ταχυδρομείου ασφαλή;</span><span class="sxs-lookup"><span data-stu-id="2a221-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="2a221-103">**Δεν συνιστάται η χρήση ασφαλών λιστών αποστολέα** , καθώς ανοίγει τον οργανισμό σας σε επιθέσεις ανεπιθύμητης αλληλογραφίας, Phish και πλαστογράφησης.</span><span class="sxs-lookup"><span data-stu-id="2a221-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="2a221-104">Ωστόσο, εάν υπάρχει επιχειρηματική απαίτηση, **συνιστούμε** να χρησιμοποιήσετε **[κανόνες ροής αλληλογραφίας](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** για αυτό.</span><span class="sxs-lookup"><span data-stu-id="2a221-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="2a221-105">Η καθοδήγησή μας διασφαλίζει τον έλεγχο ταυτότητας του αποστολέα (επαληθεύει ότι η αποστολή τομέα δεν είναι πλαστογραφημένη).</span><span class="sxs-lookup"><span data-stu-id="2a221-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="2a221-106">**Σημείωση**: δεν συνιστούμε τη διαχείριση ψευδών θετικών με τη χρήση ασφαλών λιστών αποστολέα, επειδή οι εξαιρέσεις από το φιλτράρισμα ανεπιθύμητης αλληλογραφίας μπορούν να ανοίξουν τον οργανισμό σας σε επιθέσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="2a221-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="2a221-107">Εάν οι χρήστες σας λαμβάνουν μηνύματα που έχουν εσφαλμένη σήμανση ως ανεπιθύμητη αλληλογραφία ή ανεπιθύμητη ηλεκτρονική αλληλογραφία, **[αναφέρετε τα μηνύματα και τα αρχεία σας στη Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="2a221-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="2a221-108">Οι ασφαλείς αποστολείς στο Outlook, η επιτρεπόμενη λίστα αποστολέα ή η επιτρεπόμενη λίστα τομέων στις πολιτικές anti-spam **θα πρέπει να αποφεύγονται** , επειδή οι αποστολείς παρακάμπτουν όλα τα ανεπιθύμητα μηνύματα, την πλαστογράφηση και την προστασία από Phish και τον έλεγχο ταυτότητας του ΑΠΟΣΤΟΛΈΑ (SPF, DKIM, DMARC)</span><span class="sxs-lookup"><span data-stu-id="2a221-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="2a221-109">Αυτή η μέθοδος χρησιμοποιείται καλύτερα μόνο για προσωρινούς ελέγχους.</span><span class="sxs-lookup"><span data-stu-id="2a221-109">This method is best used for temporary testing only.</span></span>
