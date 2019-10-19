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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Πότε οι αλλαγές στο προφίλ μου συγχρονίζονται με την εφαρμογή προφίλ χρήστη του SharePoint;

Ηλεκτρονική SharePoint χρησιμοποιεί την εργασία χρονομέτρησης εισαγωγής Active Directory (εισαγωγή AD) για την εισαγωγή χρηστών και ομάδων στην εφαρμογή προφίλ χρήστη. 
  
1. Η εισαγωγή AD συγχρονίζει τις αλλαγές από το χώρο αποθήκευσης καταλόγου SharePoint Online στην εφαρμογή προφίλ χρήστη. Αυτές οι αλλαγές υποβάλλονται σε επεξεργασία σε δέσμες.
    
2. Η εργασία χρονομέτρησης εκτελείται μέχρι να συγχρονιστούν οι αλλαγές.
    
> [!NOTE]
> Ο χρόνος που απαιτείται για την εκτέλεση της εργασίας εξαρτάται από τον αριθμό των αλλαγών που θα επεξεργαστούν. Ένας μεγάλος αριθμός αλλαγών διαρκεί περισσότερο. Η συμφωνία επιπέδου υπηρεσίας (SLA) αναφέρει ότι μια αλλαγή σε ένα χρήστη στον κατάλογο του SharePoint Online θα αντικατοπτρίζεται στην εφαρμογή προφίλ χρήστη σε 24 ώρες. 
  
[Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρήστη στο SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

