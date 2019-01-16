---
title: Επαναφορά μιας συλλογής τοποθεσιών διαγράφηκε
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290880"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="d1ea1-102">Επαναφορά μιας συλλογής τοποθεσιών διαγράφηκε</span><span class="sxs-lookup"><span data-stu-id="d1ea1-102">Restore a deleted site collection</span></span>

<span data-ttu-id="d1ea1-p101">Όταν ένας admin μπορεί να διαγράψει μια συλλογή τοποθεσιών classic, τοποθετείται στη συλλογή τοποθεσιών Κάδο Ανακύκλωσης, όπου διατηρείται για 93 ημέρες πριν να διαγραφεί μόνιμα. Για να επαναφέρετε τη συλλογή τοποθεσιών:</span><span class="sxs-lookup"><span data-stu-id="d1ea1-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="d1ea1-105">Στο κλασικό Κέντρο διαχείρισης του SharePoint, κάντε κλικ στο κουμπί " **Κάδος Ανακύκλωσης** " στην κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="d1ea1-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d1ea1-106">Επιλέξτε το πλαίσιο ελέγχου δίπλα από τη συλλογή τοποθεσιών που θέλετε να επαναφέρετε.</span><span class="sxs-lookup"><span data-stu-id="d1ea1-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d1ea1-107">Κάντε κλικ στο κουμπί **Επαναφορά διαγραμμένων στοιχείων**.</span><span class="sxs-lookup"><span data-stu-id="d1ea1-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d1ea1-p102">Για να επαναφέρετε μια τοποθεσία επικοινωνίας διαγραφεί, μπορείτε να χρησιμοποιήσετε τη νέα προεπισκόπηση Κέντρο διαχείρισης του SharePoint. Διαφορετικά, πρέπει να χρησιμοποιήσετε PowerShell. Για να επαναφέρετε μια τοποθεσία που ανήκει σε μια ομάδα του Office 365, πρέπει να επαναφέρετε την ομάδα στο Κέντρο διαχείρισης Exchange. Ομάδες μπορούν να ανακτηθούν για 30 ημέρες μετά την είναι η διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="d1ea1-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

