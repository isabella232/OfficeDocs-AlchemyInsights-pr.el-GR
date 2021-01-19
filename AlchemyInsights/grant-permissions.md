---
title: Εκχώρηση δικαιωμάτων
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901181"
---
# <a name="grant-permissions"></a><span data-ttu-id="1d47b-102">Εκχώρηση δικαιωμάτων</span><span class="sxs-lookup"><span data-stu-id="1d47b-102">Grant permissions</span></span>

1. <span data-ttu-id="1d47b-103">**Εκχώρηση συγκατάθεσης διαχειριστή σε επίπεδο μισθωτών**: ανατρέξτε στο θέμα [εκχώρηση συναίνεσης διαχειριστή σε επίπεδο μισθωτών σε μια εφαρμογή](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) για οδηγίες βήμα προς βήμα για τη χορήγηση συγκατάθεσης διαχειριστή σε επίπεδο μισθωτών από την πύλη Azure, χρησιμοποιώντας το Azure AD PowerShell ή από την ίδια την προτροπή συναίνεσης.</span><span class="sxs-lookup"><span data-stu-id="1d47b-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="1d47b-104">**Εκχώρηση συναίνεσης εκ μέρους ενός συγκεκριμένου χρήστη**: αντί να παραχωρήσετε συναίνεση για ολόκληρο τον οργανισμό, ένας διαχειριστής μπορεί επίσης να χρησιμοποιήσει το [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) για να εκχωρήσει τη συγκατάθεσή του για την ανάθεση δικαιωμάτων εκ μέρους ενός μεμονωμένου χρήστη.</span><span class="sxs-lookup"><span data-stu-id="1d47b-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="1d47b-105">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Λήψη πρόσβασης εκ μέρους ενός χρήστη](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="1d47b-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>