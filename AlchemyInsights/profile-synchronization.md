---
title: Συγχρονισμός προφίλ
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768113"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="7cbab-102">Πότε οι αλλαγές στο προφίλ μου συγχρονίζονται με την εφαρμογή προφίλ χρήστη του SharePoint;</span><span class="sxs-lookup"><span data-stu-id="7cbab-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="7cbab-103">Το SharePoint Online χρησιμοποιεί την εργασία χρονομήυπο (Εισαγωγή AD) της υπηρεσίας καταλόγου Active Directory για την εισαγωγή χρηστών και ομάδων στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="7cbab-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="7cbab-104">Η εισαγωγή AD συγχρονίζει τις αλλαγές από το χώρο αποθήκευσης καταλόγου του SharePoint Online στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="7cbab-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="7cbab-105">Οι αλλαγές αυτές υποβάλλονται σε επεξεργασία σε δέσμες.</span><span class="sxs-lookup"><span data-stu-id="7cbab-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="7cbab-106">Η εργασία χρονοδιακανών εκτελείται μέχρι να συγχρονιστούν οι αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="7cbab-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7cbab-107">Ο χρόνος που χρειάζεται η εργασία για την εκτέλεση εξαρτάται από τον αριθμό των αλλαγών στην επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="7cbab-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="7cbab-108">Ένας μεγάλος αριθμός αλλαγών διαρκεί περισσότερο.</span><span class="sxs-lookup"><span data-stu-id="7cbab-108">A large number of changes takes longer.</span></span> <span data-ttu-id="7cbab-109">Η σύμβαση επιπέδου υπηρεσίας (SLA) αναφέρει ότι μια αλλαγή σε ένα χρήστη στον κατάλογο του SharePoint Online θα αντικατοπτρίζεται στην εφαρμογή προφίλ χρήστη σε 24 ώρες.</span><span class="sxs-lookup"><span data-stu-id="7cbab-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="7cbab-110">Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρήστη στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7cbab-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

