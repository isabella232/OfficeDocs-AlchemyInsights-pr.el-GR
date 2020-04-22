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
# <a name="upn-sync-disabled"></a><span data-ttu-id="8b8b3-102">Απενεργοποιημένος ο συγχρονισμός UPN</span><span class="sxs-lookup"><span data-stu-id="8b8b3-102">UPN sync disabled</span></span>

<span data-ttu-id="8b8b3-103">Εάν ξεκινήσατε το συγχρονισμό με azure AD πριν από τις 30 Μαρτίου 2016, εκτελέστε το ακόλουθο cmdlet Azure AD PowerShell για να ενεργοποιήσετε τη μαλακή αντιστοίχιση UPN μόνο για τον οργανισμό σας:</span><span class="sxs-lookup"><span data-stu-id="8b8b3-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="8b8b3-104">**Set-MsolDirSyncFeature -Χαρακτηριστικό EnableSoftMatchOnUpn -Ενεργοποίηση $True**</span><span class="sxs-lookup"><span data-stu-id="8b8b3-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="8b8b3-105">Η μαλακή αντιστοίχιση UPN ενεργοποιείται αυτόματα για οργανισμούς που άρχισαν να συγχρονίζονται με azure AD στις ή μετά τις 30 Μαρτίου 2016.</span><span class="sxs-lookup"><span data-stu-id="8b8b3-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="8b8b3-106">Για να μάθετε περισσότερα σχετικά με την ενεργοποίηση της μαλακής αντιστοίχισης στο UPN και σε άλλες δυνατότητες συγχρονισμού, ανατρέξτε στο θέμα [Δυνατότητες της υπηρεσίας συγχρονισμού Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="8b8b3-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

