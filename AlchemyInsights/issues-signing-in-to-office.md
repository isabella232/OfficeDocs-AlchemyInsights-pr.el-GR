---
title: Θέματα είσοδο σε εφαρμογές του Office
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938223"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="f7425-102">Οθόνη κενή εισόδου σε εφαρμογές του Office</span><span class="sxs-lookup"><span data-stu-id="f7425-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="f7425-103">Για να διορθώσετε αυτό το ζήτημα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="f7425-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="f7425-104">Εγκαταστήστε τις τελευταίες ενημερωμένες εκδόσεις για [Windows](https://support.microsoft.com/help/4027667/windows-10-update) και του [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="f7425-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="f7425-105">Επαναφέρετε τις επιλογές του Internet Explorer: Μετάβαση σε **Εργαλεία** > **Επιλογές Internet** > **για προχωρημένους** > **Επαναφοράς ρυθμίσεων Internet Explorer** (Σημειώστε ότι θα χάσετε προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, προσπαθήστε να εισέλθετε ξανά στο Office.</span><span class="sxs-lookup"><span data-stu-id="f7425-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="f7425-106">Απενεργοποιήστε το Windows Defender εφαρμογής προστασίας (WDAG) ή οποιοδήποτε παρόμοιο πρόγραμμα προστασίας από ιούς ή τείχους προστασίας:</span><span class="sxs-lookup"><span data-stu-id="f7425-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="f7425-107">Στον πίνακα ελέγχου, μεταβείτε σε **προγράμματα**και, στη συνέχεια, επιλέξτε **Ενεργοποίηση δυνατοτήτων των Windows ή να απενεργοποιήσετε**.</span><span class="sxs-lookup"><span data-stu-id="f7425-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="f7425-108">Εάν είναι ενεργοποιημένη η προστασία εφαρμογών του Windows Defender, δοκιμάστε να την απενεργοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="f7425-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="f7425-109">**Σημείωση:** Ίσως χρειαστεί να κάνετε επανεκκίνηση του υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="f7425-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="f7425-110">Βεβαιωθείτε ότι το Microsoft.AAD.BrokerPlugin [AAD WAM προσθήκης](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν είναι αποκλεισμένο από οποιαδήποτε εφαρμογή ή ένα πρόγραμμα τείχους προστασίας/κατά-virus.</span><span class="sxs-lookup"><span data-stu-id="f7425-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="f7425-111">[Απαλοιφή Office διαπιστευτήρια](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="f7425-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="f7425-112">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0.</span><span class="sxs-lookup"><span data-stu-id="f7425-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f7425-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="f7425-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="f7425-114">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [ζητήματα σύνδεσης στο είσοδος μετά την ενημερωμένη έκδοση του Office 2016 build 16.0.7967 σε Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="f7425-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>