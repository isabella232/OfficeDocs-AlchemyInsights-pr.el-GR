---
title: Πρέπει να επισημάνετε έναν ασφαλή αποστολέα τομέα ή ηλεκτρονικού ταχυδρομείου;
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281148"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="75fc7-102">Πρέπει να επισημάνετε έναν ασφαλή αποστολέα τομέα ή ηλεκτρονικού ταχυδρομείου;</span><span class="sxs-lookup"><span data-stu-id="75fc7-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="75fc7-103">Η χρήση **λιστών ασφαλών αποστολέων δεν συνιστάται,** καθώς ανοίγει τον οργανισμό σας σε επιθέσεις ανεπιθύμητης αλληλογραφίας, phish και πλαστοποιίας.</span><span class="sxs-lookup"><span data-stu-id="75fc7-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="75fc7-104">Ωστόσο, εάν υπάρχει επιχειρηματική απαίτηση, **συνιστούμε να** χρησιμοποιήσετε **[κανόνες ροής αλληλογραφίας](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** για αυτό.</span><span class="sxs-lookup"><span data-stu-id="75fc7-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="75fc7-105">Η καθοδήγησή μας εξασφαλίζει τον έλεγχο ταυτότητας αποστολέα (επαληθεύει την αποστολή του τομέα δεν είναι πλαστογραφημένη).</span><span class="sxs-lookup"><span data-stu-id="75fc7-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="75fc7-106">**Σημείωση**: Δεν συνιστάται η διαχείριση ψευδώς θετικών μέσω της χρήσης ασφαλών λιστών αποστολέων, επειδή οι εξαιρέσεις στο φιλτράρισμα ανεπιθύμητης αλληλογραφίας μπορούν να ανοίξουν τον οργανισμό σας σε επιθέσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="75fc7-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="75fc7-107">Εάν οι χρήστες λαμβάνουν μηνύματα που έχουν επισημανθεί εσφαλμένα ως ανεπιθύμητα μηνύματα ή ανεπιθύμητα μηνύματα ηλεκτρονικού ταχυδρομείου, **[αναφέρετε μηνύματα και αρχεία στη Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="75fc7-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="75fc7-108">Οι ασφαλείς αποστολείς στο Outlook, η λίστα επιτρεπόμενων αποστολέων ή η επιτρεπόμενη λίστα τομέων σε πολιτικές κατά της ανεπιθύμητης αλληλογραφίας **θα πρέπει να αποφεύγονται,** επειδή οι αποστολείς παρακάμπτουν όλα τα ανεπιθύμητα μηνύματα, την κοροϊδία και την προστασία phish και τον έλεγχο ταυτότητας αποστολέα (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="75fc7-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="75fc7-109">Αυτή η μέθοδος χρησιμοποιείται καλύτερα μόνο για προσωρινές δοκιμές.</span><span class="sxs-lookup"><span data-stu-id="75fc7-109">This method is best used for temporary testing only.</span></span>
