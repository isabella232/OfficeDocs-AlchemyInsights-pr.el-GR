---
title: Ζητήματα που σχετίζονται με την είσοδο στο Microsoft 365 εφαρμογές
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579901"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="9f14b-102">Κενή οθόνη εισόδου στις εφαρμογές Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9f14b-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="9f14b-103">Για να διορθώσετε αυτό το ζήτημα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="9f14b-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9f14b-104">Εγκαταστήστε τις πιο πρόσφατες ενημερωμένες εκδόσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [το Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9f14b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9f14b-105">Επαναφορά επιλογών του Internet Explorer: Μεταβείτε **στις επιλογές**  >  **Internet**  >  **Για προχωρημένους,** επαναφορά των  >  **ρυθμίσεων του Internet Explorer** (σημειώστε ότι θα χάσετε προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, προσπαθήστε να εισέλθετε ξανά στο Office.</span><span class="sxs-lookup"><span data-stu-id="9f14b-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9f14b-106">Απενεργοποιήστε το Windows Defender Application Guard (WDAG) ή οποιοδήποτε παρόμοιο τείχος προστασίας ή πρόγραμμα προστασίας από ιούς:</span><span class="sxs-lookup"><span data-stu-id="9f14b-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9f14b-107">Στον Πίνακα Ελέγχου, μεταβείτε στην **ενότητα Προγράμματα**και, στη συνέχεια, επιλέξτε **Ενεργοποίηση ή απενεργοποίηση δυνατοτήτων των Windows**.</span><span class="sxs-lookup"><span data-stu-id="9f14b-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9f14b-108">Εάν είναι ενεργοποιημένο το Windows Defender Application Guard, δοκιμάστε να τον απενεργοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="9f14b-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9f14b-109">**Σημείωση:** Ίσως χρειαστεί να επανεκκινήσετε τον υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="9f14b-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9f14b-110">Βεβαιωθείτε ότι η προσθήκη Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν αποκλείεται από οποιαδήποτε εφαρμογή ή πρόγραμμα τείχους προστασίας/προστασίας από ιούς.</span><span class="sxs-lookup"><span data-stu-id="9f14b-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9f14b-111">[Καταργήστε τις πιστοποιήσεις του Office χρησιμοποιώντας](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="9f14b-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9f14b-112">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0.</span><span class="sxs-lookup"><span data-stu-id="9f14b-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9f14b-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9f14b-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9f14b-114">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ζητήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση για τη δημιουργία του Office 2016 16.0.7967 στα Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9f14b-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>