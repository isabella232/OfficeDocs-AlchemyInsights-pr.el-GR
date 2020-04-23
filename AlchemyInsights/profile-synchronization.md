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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Πότε οι αλλαγές στο προφίλ μου συγχρονίζονται με την εφαρμογή προφίλ χρήστη του SharePoint;

Το SharePoint Online χρησιμοποιεί την εργασία χρονομήυπο (Εισαγωγή AD) της υπηρεσίας καταλόγου Active Directory για την εισαγωγή χρηστών και ομάδων στην εφαρμογή προφίλ χρήστη. 
  
1. Η εισαγωγή AD συγχρονίζει τις αλλαγές από το χώρο αποθήκευσης καταλόγου του SharePoint Online στην εφαρμογή προφίλ χρήστη. Οι αλλαγές αυτές υποβάλλονται σε επεξεργασία σε δέσμες.
    
2. Η εργασία χρονοδιακανών εκτελείται μέχρι να συγχρονιστούν οι αλλαγές.
    
> [!NOTE]
> Ο χρόνος που χρειάζεται η εργασία για την εκτέλεση εξαρτάται από τον αριθμό των αλλαγών στην επεξεργασία. Ένας μεγάλος αριθμός αλλαγών διαρκεί περισσότερο. Η σύμβαση επιπέδου υπηρεσίας (SLA) αναφέρει ότι μια αλλαγή σε ένα χρήστη στον κατάλογο του SharePoint Online θα αντικατοπτρίζεται στην εφαρμογή προφίλ χρήστη σε 24 ώρες. 
  
[Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρήστη στο SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

