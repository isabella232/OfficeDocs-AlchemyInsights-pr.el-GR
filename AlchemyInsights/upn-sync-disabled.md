---
title: Συγχρονισμός UPN απενεργοποιημένη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532331"
---
# <a name="upn-sync-disabled"></a>Συγχρονισμός UPN απενεργοποιημένη

Εάν ξεκινήσει συγχρονισμό Azure AD πριν από τις 30 Μαρτίου 2016, εκτελέστε τα παρακάτω cmdlet Azure AD PowerShell ενεργοποίησης UPN μαλακό αντιστοιχία για τον οργανισμό σας μόνο:
  
 **Σύνολο MsolDirSyncFeature-δυνατότητα EnableSoftMatchOnUpn-Ενεργοποίηση $True**
  
Ταίριασμα μαλακό UPN ενεργοποιείται αυτόματα για τους οργανισμούς που ξεκίνησε το συγχρονισμό Azure AD στις ή μετά τις 30 Μαρτίου 2016.
  
Για να μάθετε περισσότερα σχετικά με την ενεργοποίηση του λογισμικού που ταιριάζουν σε UPN και άλλες δυνατότητες συγχρονισμού, δείτε: [σύνδεση AD Azure δυνατότητες υπηρεσίας συγχρονισμού](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

