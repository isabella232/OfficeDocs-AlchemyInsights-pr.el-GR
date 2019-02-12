---
title: Επαναφορά μιας συλλογής τοποθεσιών διαγράφηκε
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 22fb513771abc1a604a347204bac268771cb9e37
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939996"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="86c9f-102">Επαναφορά μιας συλλογής τοποθεσιών διαγράφηκε</span><span class="sxs-lookup"><span data-stu-id="86c9f-102">Restore a deleted site collection</span></span>

<span data-ttu-id="86c9f-p101">Όταν ένας admin μπορεί να διαγράψει μια συλλογή τοποθεσιών classic, τοποθετείται στη συλλογή τοποθεσιών Κάδο Ανακύκλωσης, όπου διατηρείται για 93 ημέρες πριν να διαγραφεί μόνιμα. Για να επαναφέρετε τη συλλογή τοποθεσιών:</span><span class="sxs-lookup"><span data-stu-id="86c9f-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="86c9f-105">Στο κλασικό Κέντρο διαχείρισης του SharePoint, κάντε κλικ στο κουμπί " **Κάδος Ανακύκλωσης** " στην κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="86c9f-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="86c9f-106">Επιλέξτε το πλαίσιο ελέγχου δίπλα από τη συλλογή τοποθεσιών που θέλετε να επαναφέρετε.</span><span class="sxs-lookup"><span data-stu-id="86c9f-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="86c9f-107">Κάντε κλικ στο κουμπί **Επαναφορά διαγραμμένων στοιχείων**.</span><span class="sxs-lookup"><span data-stu-id="86c9f-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="86c9f-p102">Για να επαναφέρετε μια τοποθεσία επικοινωνίας διαγραφεί, μπορείτε να χρησιμοποιήσετε τη νέα προεπισκόπηση Κέντρο διαχείρισης του SharePoint. Διαφορετικά, πρέπει να χρησιμοποιήσετε PowerShell. Για να επαναφέρετε μια τοποθεσία που ανήκει σε μια ομάδα του Office 365, πρέπει να επαναφέρετε την ομάδα στο Κέντρο διαχείρισης Exchange. Ομάδες μπορούν να ανακτηθούν για 30 ημέρες μετά την είναι η διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="86c9f-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

