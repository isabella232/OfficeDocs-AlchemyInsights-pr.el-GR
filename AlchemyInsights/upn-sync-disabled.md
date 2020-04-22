---
title: Απενεργοποιημένος ο συγχρονισμός UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726104"
---
# <a name="upn-sync-disabled"></a>Απενεργοποιημένος ο συγχρονισμός UPN

Εάν ξεκινήσατε το συγχρονισμό με azure AD πριν από τις 30 Μαρτίου 2016, εκτελέστε το ακόλουθο cmdlet Azure AD PowerShell για να ενεργοποιήσετε τη μαλακή αντιστοίχιση UPN μόνο για τον οργανισμό σας:
  
 **Set-MsolDirSyncFeature -Χαρακτηριστικό EnableSoftMatchOnUpn -Ενεργοποίηση $True**
  
Η μαλακή αντιστοίχιση UPN ενεργοποιείται αυτόματα για οργανισμούς που άρχισαν να συγχρονίζονται με azure AD στις ή μετά τις 30 Μαρτίου 2016.
  
Για να μάθετε περισσότερα σχετικά με την ενεργοποίηση της μαλακής αντιστοίχισης στο UPN και σε άλλες δυνατότητες συγχρονισμού, ανατρέξτε στο θέμα [Δυνατότητες της υπηρεσίας συγχρονισμού Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

