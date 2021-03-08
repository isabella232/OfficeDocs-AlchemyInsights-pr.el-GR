---
title: Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524282"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="1d41d-102">Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας</span><span class="sxs-lookup"><span data-stu-id="1d41d-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="1d41d-103">Ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="1d41d-103">Follow these steps:</span></span>

1. <span data-ttu-id="1d41d-104">Εάν δεν είστε καθολικός διαχειριστής, για να αναζητήσετε μηνύματα, ο λογαριασμός σας πρέπει να προστεθεί στην ομάδα ρόλων **"Διαχείριση eDiscovery"** ή στο ρόλο διαχείρισης αναζήτησης **συμμόρφωσης.**</span><span class="sxs-lookup"><span data-stu-id="1d41d-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="1d41d-105">Για να διαγράψετε μηνύματα, θα πρέπει να συμμετάσχετε στην ομάδα ρόλων **"Διαχείριση οργανισμού"** ή στο ρόλο **διαχείρισης "Αναζήτηση και εκκαθάριση".**</span><span class="sxs-lookup"><span data-stu-id="1d41d-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="1d41d-106">Τα δικαιώματα σε αυτούς τους ρόλους εκχωρούνται στο [Κέντρο συμμόρφωσης & ασφαλείας.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="1d41d-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="1d41d-107">[Δημιουργήστε μια αναζήτηση περιεχομένου για](https://docs.microsoft.com/office365/securitycompliance/content-search) να βρείτε το μήνυμα προς διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="1d41d-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="1d41d-108">[Συνδεθείτε με το Κέντρο & Συμμόρφωσης PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="1d41d-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="1d41d-109">Εάν χρησιμοποιείτε MFA, ανατρέξτε σε αυτές τις οδηγίες: Σύνδεση στο PowerShell του Κέντρου συμμόρφωσης & ασφάλειας με χρήση [ελέγχου ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="1d41d-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="1d41d-110">Διαγράψτε το μήνυμα: εκτελέστε `New-ComplianceSearchAction` το cmdlet για να διαγράψετε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="1d41d-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="1d41d-111">Τα διαγραμμένα μηνύματα μετακινούνται στο φάκελο "Ανακτήσιμα" ενός χρήστη.</span><span class="sxs-lookup"><span data-stu-id="1d41d-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="1d41d-112">Για ένα παράδειγμα εντολής, ανατρέξτε [στο βήμα 3: Διαγραφή του μηνύματος.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="1d41d-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
