---
title: Επιδιόρθωση πολιτικής σύνδεσης
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694165"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="db3db-102">Επιδιόρθωση πολιτικής σύνδεσης</span><span class="sxs-lookup"><span data-stu-id="db3db-102">Fix connection policy</span></span>

<span data-ttu-id="db3db-103">Το μήνυμα ηλεκτρονικού ταχυδρομείου επισημάνθηκε ως ασφαλές και παραδόθηκε στα εισερχόμενα του χρήστη, επειδή η διεύθυνση IP αποστολής είχε επισημανθεί ως ασφαλής στην πολιτική φίλτρου σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="db3db-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="db3db-104">Για να εξετάσετε την πολιτική, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="db3db-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="db3db-105">Μεταβείτε στο Κέντρο [συμμόρφωσης ασφαλείας του Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143)και, στη συνέχεια, μεταβείτε στην **Πολιτική** διαχείρισης  >  **απειλών κατά** της  >  [ανεπιθύμητης αλληλογραφίας.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="db3db-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="db3db-106">Στην καρτέλα **"Προσαρμογή",** επιλέξτε την πολιτική **φίλτρου σύνδεσης και,** στη συνέχεια, επιλέξτε **"Επεξεργασία πολιτικής".**</span><span class="sxs-lookup"><span data-stu-id="db3db-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="db3db-107">Ελέγξτε τη λίστα **επιτρεπόμενων διευθύνσεων IP.**</span><span class="sxs-lookup"><span data-stu-id="db3db-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="db3db-108">Δείτε εάν **είναι ενεργοποιημένη η** λίστα ασφαλών μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="db3db-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="db3db-109">Η Microsoft εγγράφεται σε προελεύσεις αξιόπιστων αποστολέων τρίτων κατασκευαστών.</span><span class="sxs-lookup"><span data-stu-id="db3db-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="db3db-110">Εάν **η λίστα ασφαλών** αποστολέων είναι ενεργοποιημένη, αυτοί οι αξιόπιστοι αποστολείς δεν επισημαίνονται κατά λάθος ως ανεπιθύμητη αλληλογραφία.</span><span class="sxs-lookup"><span data-stu-id="db3db-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="db3db-111">Συνιστάται να κάνετε αυτή την επιλογή, επειδή θα μειωθεί ο αριθμός των ψευδών θετικών (καλού ταχυδρομείου που χαρακτηρίζονται ως ανεπιθύμητη αλληλογραφία) που λαμβάνετε.</span><span class="sxs-lookup"><span data-stu-id="db3db-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
