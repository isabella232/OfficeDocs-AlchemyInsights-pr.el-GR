---
title: Ο συγχρονισμός UPN απενεργοποιήθηκε
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038112"
---
# <a name="upn-sync-disabled"></a>Ο συγχρονισμός UPN απενεργοποιήθηκε

Εάν ξεκινήσατε να συγχρονίζετε το Azure AD πριν από τις 30 Μαρτίου 2016, εκτελέστε το ακόλουθο cmdlet Azure AD PowerShell για να ενεργοποιήσετε την ομαλή αντιστοίχιση UPN μόνο για τον οργανισμό σας:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Η απαλή αντιστοίχιση UPN ενεργοποιείται αυτόματα για οργανισμούς που ξεκίνησαν να συγχρονίζονται με το Azure AD στις ή μετά τις 30 Μαρτίου 2016.
  
Για να μάθετε περισσότερα σχετικά με την ενεργοποίηση της ομαλής αντιστοίχισης στο UPN και σε άλλες δυνατότητες συγχρονισμού, ανατρέξτε στο [θέμα Δυνατότητες υπηρεσίας συγχρονισμού του Azure AD Σύνδεση υπηρεσίας συγχρονισμού.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

