---
title: Συγχρονισμού προφίλ
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290917"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="957ea-102">Όταν οι αλλαγές στο προφίλ μου συγχρονισμό με την εφαρμογή προφίλ χρήστη του SharePoint;</span><span class="sxs-lookup"><span data-stu-id="957ea-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="957ea-103">Ηλεκτρονική SharePoint χρησιμοποιεί την εργασία χρονομέτρησης εισαγωγή Active Directory (AD εισαγωγή) για να εισαγάγετε τους χρήστες και τις ομάδες στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="957ea-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="957ea-p101">Εισαγωγή AD συγχρονίζει τις αλλαγές από το ηλεκτρονικό κατάστημα καταλόγου του SharePoint για την εφαρμογή προφίλ χρήστη. Αυτές οι αλλαγές υποβάλλονται σε επεξεργασία σε δέσμες.</span><span class="sxs-lookup"><span data-stu-id="957ea-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="957ea-106">Η εργασία χρονομέτρησης εκτελείται έως ότου συγχρονιστούν οι αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="957ea-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="957ea-p102">Ο χρόνος που απαιτείται η εκτέλεση της εργασίας εξαρτάται από τον αριθμό των αλλαγών για την επεξεργασία. Ένα μεγάλο αριθμό αλλαγών διαρκεί περισσότερο. Η συμφωνία επιπέδου υπηρεσίας (SLA) δηλώνει ότι μια αλλαγή σε ένα χρήστη στον κατάλογο του SharePoint Online θα εμφανιστεί στην εφαρμογή προφίλ χρήστη σε 24 ώρες.</span><span class="sxs-lookup"><span data-stu-id="957ea-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="957ea-110">Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρήστη στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="957ea-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

