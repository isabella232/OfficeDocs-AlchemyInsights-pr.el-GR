---
title: Διαγραφή ή επαναφορά εφαρμογών
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014800"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="c3e41-102">Διαγραφή ή επαναφορά εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="c3e41-102">Delete or restore applications</span></span>

<span data-ttu-id="c3e41-103">**Για να διαγράψετε μια εφαρμογή από τον μισθωτή σας Azure AD**:</span><span class="sxs-lookup"><span data-stu-id="c3e41-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="c3e41-104">Στην **πύλη Azure AD**, επιλέξτε **εταιρικές εφαρμογές**.</span><span class="sxs-lookup"><span data-stu-id="c3e41-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="c3e41-105">Στη συνέχεια, εντοπίστε και επιλέξτε την εφαρμογή που θέλετε να διαγράψετε.</span><span class="sxs-lookup"><span data-stu-id="c3e41-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="c3e41-106">Στην ενότητα **Manage** στο αριστερό τμήμα του παραθύρου, επιλέξτε **Ιδιότητες**.</span><span class="sxs-lookup"><span data-stu-id="c3e41-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="c3e41-107">Επιλέξτε **Διαγραφή** και, στη συνέχεια, επιλέξτε **Ναι** για να επιβεβαιώσετε ότι θέλετε να διαγράψετε την εφαρμογή από τον μισθωτή σας Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c3e41-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="c3e41-108">Για περισσότερες πληροφορίες σχετικά με τον τρόπο διαγραφής μιας εφαρμογής, ανατρέξτε στο θέμα [Γρήγορη εκκίνηση: Διαγραφή μιας εφαρμογής από τον μισθωτή του Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="c3e41-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="c3e41-109">Στο PowerShell, το cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) καταργεί τις ρυθμίσεις παραμέτρων του διακομιστή μεσολάβησης εφαρμογής από μια συγκεκριμένη εφαρμογή στο Azure Active Directory και μπορεί να διαγράψει πλήρως την εφαρμογή εάν έχει καθοριστεί.</span><span class="sxs-lookup"><span data-stu-id="c3e41-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="c3e41-110">Μπορείτε να **επαναφέρετε μια διαγραμμένη εφαρμογή χρησιμοποιώντας το** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c3e41-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="c3e41-111">Αφού εντοπιστεί η εφαρμογή που θέλετε να επαναφέρετε, μπορείτε να την επαναφέρετε χρησιμοποιώντας την [Επαναφορά-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="c3e41-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
