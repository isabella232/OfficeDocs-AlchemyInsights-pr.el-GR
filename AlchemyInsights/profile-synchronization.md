---
title: Συγχρονισμός προφίλ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801769"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="2b6a2-102">Πότε αλλάζει το προφίλ μου το συγχρονισμό με την εφαρμογή προφίλ χρήστη του SharePoint;</span><span class="sxs-lookup"><span data-stu-id="2b6a2-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="2b6a2-103">Το SharePoint Online χρησιμοποιεί την εργασία χρονομέτρησης εισαγωγής της υπηρεσίας καταλόγου Active Directory (εισαγωγή AD) για την εισαγωγή χρηστών και ομάδων στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="2b6a2-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="2b6a2-104">Η εισαγωγή διαφημίσεων συγχρονίζει τις αλλαγές από το χώρο αποθήκευσης καταλόγου του SharePoint Online στην εφαρμογή προφίλ χρήστη.</span><span class="sxs-lookup"><span data-stu-id="2b6a2-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="2b6a2-105">Αυτές οι αλλαγές υποβάλλονται σε επεξεργασία σε δέσμες.</span><span class="sxs-lookup"><span data-stu-id="2b6a2-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="2b6a2-106">Η εργασία χρονομέτρησης εκτελείται μέχρι να συγχρονιστούν οι αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="2b6a2-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="2b6a2-107">Ο χρόνος που απαιτείται για την εκτέλεση της εργασίας εξαρτάται από τον αριθμό των αλλαγών που θα διεργαστούν.</span><span class="sxs-lookup"><span data-stu-id="2b6a2-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="2b6a2-108">Ένας μεγάλος αριθμός αλλαγών διαρκεί περισσότερο.</span><span class="sxs-lookup"><span data-stu-id="2b6a2-108">A large number of changes takes longer.</span></span> <span data-ttu-id="2b6a2-109">Η συμφωνία επιπέδου εξυπηρέτησης (SLA) αναφέρει ότι μια αλλαγή σε ένα χρήστη στον κατάλογο του SharePoint Online θα αντικατοπτρίζεται στην εφαρμογή προφίλ χρήστη σε 24 ώρες.</span><span class="sxs-lookup"><span data-stu-id="2b6a2-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="2b6a2-110">Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρήστη στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2b6a2-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

