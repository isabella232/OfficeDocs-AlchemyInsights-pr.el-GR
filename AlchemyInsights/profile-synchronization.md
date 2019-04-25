---
title: Συγχρονισμού προφίλ
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371984"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="9fc35-102">Όταν οι αλλαγές στο προφίλ μου συγχρονισμό με την εφαρμογή προφίλ χρήστη του SharePoint;</span><span class="sxs-lookup"><span data-stu-id="9fc35-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="9fc35-103">Ηλεκτρονική SharePoint χρησιμοποιεί την εργασία χρονομέτρησης εισαγωγή Active Directory (AD εισαγωγή) για να εισαγάγετε τους χρήστες και τις ομάδες στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="9fc35-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="9fc35-104">Εισαγωγή AD συγχρονίζει τις αλλαγές από το ηλεκτρονικό κατάστημα καταλόγου του SharePoint για την εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="9fc35-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="9fc35-105">Αυτές οι αλλαγές υποβάλλονται σε επεξεργασία σε δέσμες.</span><span class="sxs-lookup"><span data-stu-id="9fc35-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="9fc35-106">Η εργασία χρονομέτρησης εκτελείται έως ότου συγχρονιστούν οι αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="9fc35-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="9fc35-107">Ο χρόνος που απαιτείται η εκτέλεση της εργασίας εξαρτάται από τον αριθμό των αλλαγών για την επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="9fc35-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="9fc35-108">Ένα μεγάλο αριθμό αλλαγών διαρκεί περισσότερο.</span><span class="sxs-lookup"><span data-stu-id="9fc35-108">A large number of changes takes longer.</span></span> <span data-ttu-id="9fc35-109">Η συμφωνία επιπέδου υπηρεσίας (SLA) δηλώνει ότι μια αλλαγή σε ένα χρήστη στον κατάλογο του SharePoint Online θα εμφανιστεί στην εφαρμογή προφίλ χρήστη σε 24 ώρες.</span><span class="sxs-lookup"><span data-stu-id="9fc35-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="9fc35-110">Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρήστη στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9fc35-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

