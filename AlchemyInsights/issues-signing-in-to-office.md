---
title: Προβλήματα κατά την είσοδο σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695287"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="bcb61-102">Κενή οθόνη εισόδου στις εφαρμογές του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bcb61-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="bcb61-103">Για να διορθώσετε αυτό το πρόβλημα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="bcb61-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="bcb61-104">Εγκαταστήστε τις πιο πρόσφατες ενημερώσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και το [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="bcb61-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="bcb61-105">Επαναφορά επιλογών του Internet Explorer: μεταβείτε στις επιλογές **Εργαλεία**  >  **Internet**για  >  **προχωρημένους**  >  **Επαναφορά ρυθμίσεων του Internet Explorer** (Σημειώστε ότι θα χάσετε τις προσαρμοσμένες ρυθμίσεις) και, στη συνέχεια, δοκιμάστε να συνδεθείτε στο Office ξανά.</span><span class="sxs-lookup"><span data-stu-id="bcb61-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="bcb61-106">Απενεργοποιήστε το προστατευτικό εφαρμογής του Windows Defender (WDAG) ή οποιοδήποτε παρόμοιο τείχος προστασίας ή πρόγραμμα εντοπισμού ιών:</span><span class="sxs-lookup"><span data-stu-id="bcb61-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="bcb61-107">Στον πίνακα ελέγχου, μεταβείτε στην επιλογή **προγράμματα**και, στη συνέχεια, επιλέξτε **Ενεργοποίηση ή απενεργοποίηση δυνατοτήτων των Windows**.</span><span class="sxs-lookup"><span data-stu-id="bcb61-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="bcb61-108">Εάν είναι ενεργοποιημένη η προστασία εφαρμογών του Windows Defender, δοκιμάστε να την απενεργοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="bcb61-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="bcb61-109">**Σημείωση:** Ίσως χρειαστεί να επανεκκινήσετε τον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="bcb61-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="bcb61-110">Βεβαιωθείτε ότι η προσθήκη του Microsoft. AAD. BrokerPlugin [AAD](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) δεν εμποδίζεται από οποιαδήποτε εφαρμογή ή πρόγραμμα τείχους προστασίας/προστασίας από ιούς.</span><span class="sxs-lookup"><span data-stu-id="bcb61-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="bcb61-111">[Καταργήστε τα διαπιστευτήρια του Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="bcb61-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="bcb61-112">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0.</span><span class="sxs-lookup"><span data-stu-id="bcb61-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="bcb61-113">(Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="bcb61-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="bcb61-114">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα προβλήματα σύνδεσης στην είσοδο μετά την ενημέρωση στο Office 2016 Δόμηση 16.0.7967 στα Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="bcb61-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>