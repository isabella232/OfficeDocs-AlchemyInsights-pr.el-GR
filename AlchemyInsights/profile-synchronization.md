---
title: Συγχρονισμός προφίλ
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554333"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="d64d1-102">Πότε οι αλλαγές στο προφίλ μου συγχρονίζονται με την εφαρμογή προφίλ χρήστη του SharePoint;</span><span class="sxs-lookup"><span data-stu-id="d64d1-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="d64d1-103">Ηλεκτρονική SharePoint χρησιμοποιεί την εργασία χρονομέτρησης εισαγωγής Active Directory (εισαγωγή AD) για την εισαγωγή χρηστών και ομάδων στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="d64d1-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="d64d1-104">Η εισαγωγή AD συγχρονίζει τις αλλαγές από το χώρο αποθήκευσης καταλόγου SharePoint Online στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="d64d1-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="d64d1-105">Αυτές οι αλλαγές υποβάλλονται σε επεξεργασία σε δέσμες.</span><span class="sxs-lookup"><span data-stu-id="d64d1-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="d64d1-106">Η εργασία χρονομέτρησης εκτελείται μέχρι να συγχρονιστούν οι αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="d64d1-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="d64d1-107">Ο χρόνος που απαιτείται για την εκτέλεση της εργασίας εξαρτάται από τον αριθμό των αλλαγών που θα επεξεργαστούν.</span><span class="sxs-lookup"><span data-stu-id="d64d1-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="d64d1-108">Ένας μεγάλος αριθμός αλλαγών διαρκεί περισσότερο.</span><span class="sxs-lookup"><span data-stu-id="d64d1-108">A large number of changes takes longer.</span></span> <span data-ttu-id="d64d1-109">Η συμφωνία επιπέδου υπηρεσίας (SLA) αναφέρει ότι μια αλλαγή σε ένα χρήστη στον κατάλογο του SharePoint Online θα αντικατοπτρίζεται στην εφαρμογή προφίλ χρήστη σε 24 ώρες.</span><span class="sxs-lookup"><span data-stu-id="d64d1-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="d64d1-110">Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρήστη στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d64d1-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

