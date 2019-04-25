---
title: 932 AADConnect αναβάθμιση
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389684"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="0f4b9-102">Αναβάθμιση Azure AD σύνδεση</span><span class="sxs-lookup"><span data-stu-id="0f4b9-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="0f4b9-103">Από προεπιλογή, ενεργοποιείται η Αυτόματη αναβάθμιση για σύνδεση AD Azure, που συμβάλλει ώστε να χρησιμοποιείτε την πιο πρόσφατη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="0f4b9-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="0f4b9-104">Για να επαληθεύσετε τις ρυθμίσεις αυτόματης αναβάθμισης, χρησιμοποιήστε το cmdlet **Get-ADSyncAutoUpgrade** σε Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0f4b9-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="0f4b9-105">Το cmdlet θα επιστρέψει μία από τις ακόλουθες τιμές:</span><span class="sxs-lookup"><span data-stu-id="0f4b9-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="0f4b9-106">**Ενεργοποίηση**: Αυτόματη αναβάθμιση είναι ενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="0f4b9-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="0f4b9-107">**Απενεργοποιημένο**: Αυτόματη αναβάθμιση είναι απενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="0f4b9-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="0f4b9-108">**Αναστολής**: το σύστημα δεν είναι πλέον επιλέξιμες να λαμβάνετε αυτόματες αναβαθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="0f4b9-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="0f4b9-109">Δεν μπορείτε να ρυθμίσετε αυτήν την τιμή; ορίζεται από το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="0f4b9-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="0f4b9-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="0f4b9-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="0f4b9-111">Για να κάνετε λήψη της τελευταίας έκδοσης του σύνδεση AD Azure, μεταβείτε στο [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="0f4b9-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
