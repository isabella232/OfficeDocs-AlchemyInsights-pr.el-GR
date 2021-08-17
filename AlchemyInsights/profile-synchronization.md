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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320709"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Πότε συγχρονίζονται οι αλλαγές προφίλ μου με SharePoint εφαρμογή προφίλ χρήστη;

SharePoint Το Online χρησιμοποιεί την εργασία χρονομετρητή εισαγωγής υπηρεσίας καταλόγου Active Directory (AD Import) για την εισαγωγή χρηστών και ομάδων στην εφαρμογή προφίλ χρήστη. 
  
1. Η εισαγωγή AD συγχρονίζει τις αλλαγές από SharePoint Online Directory Store στην εφαρμογή προφίλ χρήστη. Αυτές οι αλλαγές υποβάλλονται σε επεξεργασία σε δέσμες.
    
2. Η εργασία χρονομετρητή εκτελείται μέχρι να συγχρονιστούν οι αλλαγές.
    
**Σημείωση:** Ο χρόνος που απαιτείται για την εκτέλεση της εργασίας εξαρτάται από τον αριθμό των αλλαγών που πρέπει να γίνουν. Ένας μεγάλος αριθμός αλλαγών διαρκεί περισσότερο. Η Σύμβαση επιπέδου υπηρεσίας (SLA) αναφέρει ότι μια αλλαγή σε ένα χρήστη του SharePoint Online Directory θα αντικατοπτρίζεται στην εφαρμογή προφίλ χρήστη σε 24 ώρες. 
  
[Περισσότερες πληροφορίες σχετικά με το συγχρονισμό προφίλ χρηστών στο SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

