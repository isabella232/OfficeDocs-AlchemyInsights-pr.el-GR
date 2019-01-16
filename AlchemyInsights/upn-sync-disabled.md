---
title: Συγχρονισμός UPN απενεργοποιημένη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291514"
---
# <a name="upn-sync-disabled"></a>Συγχρονισμός UPN απενεργοποιημένη

Εάν ξεκινήσει συγχρονισμό Azure AD πριν από τις 30 Μαρτίου 2016, εκτελέστε τα παρακάτω cmdlet Azure AD PowerShell ενεργοποίησης UPN μαλακό αντιστοιχία για τον οργανισμό σας μόνο:
  
 **Σύνολο MsolDirSyncFeature-δυνατότητα EnableSoftMatchOnUpn-Ενεργοποίηση $True**
  
Ταίριασμα μαλακό UPN ενεργοποιείται αυτόματα για τους οργανισμούς που ξεκίνησε το συγχρονισμό Azure AD στις ή μετά τις 30 Μαρτίου 2016.
  
Για να μάθετε περισσότερα σχετικά με την ενεργοποίηση του λογισμικού που ταιριάζουν σε UPN και άλλες δυνατότητες συγχρονισμού, δείτε: [σύνδεση AD Azure δυνατότητες υπηρεσίας συγχρονισμού](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

