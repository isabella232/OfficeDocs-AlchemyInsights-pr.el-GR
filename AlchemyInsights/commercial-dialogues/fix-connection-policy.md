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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746752"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="4d067-102">Επιδιόρθωση πολιτικής σύνδεσης</span><span class="sxs-lookup"><span data-stu-id="4d067-102">Fix connection policy</span></span>

<span data-ttu-id="4d067-103">Το μήνυμα ηλεκτρονικού ταχυδρομείου επισημάνθηκε ως ασφαλές και παραδόθηκε στα εισερχόμενα του χρήστη, επειδή η διεύθυνση IP αποστολής επισημάνθηκε ως ασφαλής στην πολιτική φίλτρου σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="4d067-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="4d067-104">Για να αναθεωρήσετε την πολιτική, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="4d067-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="4d067-105">Μεταβείτε στο [Κέντρο ασφάλειας του Office 365 & και, στη](https://go.microsoft.com/fwlink/p/?linkid=2077143)συνέχεια, μεταβείτε στην πολιτική διαχείρισης **απειλών**  >    >  [κατά της ανεπιθύμητης αλληλογραφίας.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="4d067-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="4d067-106">Στην καρτέλα **"Προσαρμογή",** επιλέξτε την πολιτική **φίλτρου σύνδεσης και, στη** συνέχεια, επιλέξτε **"Επεξεργασία πολιτικής".**</span><span class="sxs-lookup"><span data-stu-id="4d067-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="4d067-107">Εξετάστε τη λίστα **επιτρεπόμενων διευθύνσεων IP.**</span><span class="sxs-lookup"><span data-stu-id="4d067-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="4d067-108">Δείτε εάν **είναι ενεργοποιημένη η ασφαλής** λίστα.</span><span class="sxs-lookup"><span data-stu-id="4d067-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="4d067-109">Η Microsoft εγγράφεται σε πηγές αξιόπιστων αποστολέων τρίτων κατασκευαστών.</span><span class="sxs-lookup"><span data-stu-id="4d067-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="4d067-110">Εάν **είναι ενεργοποιημένη η** ασφαλής λίστα, αυτοί οι αξιόπιστοι αποστολείς δεν επισημαίνονται κατά λάθος ως ανεπιθύμητη αλληλογραφία.</span><span class="sxs-lookup"><span data-stu-id="4d067-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="4d067-111">Σας συνιστούμε να επιλέξετε αυτή την επιλογή, επειδή θα μειωθεί ο αριθμός των ψευδών θετικών μηνυμάτων (καλή αλληλογραφία που έχει ταξινομηθεί ως ανεπιθύμητη αλληλογραφία) που λαμβάνετε.</span><span class="sxs-lookup"><span data-stu-id="4d067-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
