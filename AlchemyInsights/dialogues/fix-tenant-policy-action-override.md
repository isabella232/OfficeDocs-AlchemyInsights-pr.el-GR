---
title: Επιδιόρθωση πολιτικής μισθωτή (παράκαμψη ενέργειας)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694064"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="42641-102">Επιδιόρθωση πολιτικής μισθωτή (παράκαμψη ενέργειας)</span><span class="sxs-lookup"><span data-stu-id="42641-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="42641-103">Μια πολιτική καταπολέμησης της ανεπιθύμητης αλληλογραφίας στο μισθωτή σας επηρέασα αυτό το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="42641-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="42641-104">Για να εξετάσετε την πολιτική, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="42641-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="42641-105">Μεταβείτε στο Κέντρο [συμμόρφωσης ασφαλείας του Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143)και, στη συνέχεια, μεταβείτε στην **Πολιτική** διαχείρισης  >  **απειλών κατά** της  >  [ανεπιθύμητης αλληλογραφίας.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="42641-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="42641-106">Ελέγξτε εάν  η προέλευση πολιτικής υποδεικνύει τα εξής: **Add-Xheader/ModifySubject/Redirect/Delete/No action/ Μήνυμα "BCC"**</span><span class="sxs-lookup"><span data-stu-id="42641-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="42641-107">Εάν ναι, στην καρτέλα **"Προσαρμογή",** ελέγξτε τις ρυθμίσεις της πολιτικής που επηρέασαν το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="42641-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="42641-108">Είναι πιθανό οι Τυπικές ρυθμίσεις που **εφαρμόζονται σε** όλους τους πελάτες του Exchange Online Protection να επηρέασαν το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="42641-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="42641-109">Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση παραμέτρων των πολιτικών φίλτρου ανεπιθύμητης αλληλογραφίας, ανατρέξτε στο θέμα ["Ρύθμιση παραμέτρων των πολιτικών φίλτρου ανεπιθύμητης αλληλογραφίας".](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="42641-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
