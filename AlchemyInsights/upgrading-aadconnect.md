---
title: 932 Αναβάθμιση AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766493"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="24cc9-102">Αναβάθμιση σύνδεσης azure ad</span><span class="sxs-lookup"><span data-stu-id="24cc9-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="24cc9-103">Από προεπιλογή, η αυτόματη αναβάθμιση είναι ενεργοποιημένη για το Azure AD Connect, το οποίο σας βοηθά να εξασφαλίσετε ότι εκτελείτε την πιο πρόσφατη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="24cc9-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="24cc9-104">Για να επαληθεύσετε τις ρυθμίσεις αυτόματης αναβάθμισης, χρησιμοποιήστε το cmdlet **Get-ADSyncAutoUpgrade** στο Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="24cc9-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="24cc9-105">Το cmdlet θα επιστρέψει μία από τις ακόλουθες τιμές:</span><span class="sxs-lookup"><span data-stu-id="24cc9-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="24cc9-106">**Ενεργοποιημένο:** Η αυτόματη αναβάθμιση είναι ενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="24cc9-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="24cc9-107">**Απενεργοποιημένο**: Η αυτόματη αναβάθμιση είναι απενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="24cc9-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="24cc9-108">**Αναστολή:** Το σύστημα δεν είναι πλέον κατάλληλο για αυτόματη λήψη αναβαθμίσεων.</span><span class="sxs-lookup"><span data-stu-id="24cc9-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="24cc9-109">Δεν μπορείτε να ρυθμίσετε αυτήν την τιμή. Έχει ρυθμιστεί από το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="24cc9-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="24cc9-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="24cc9-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="24cc9-111">Για να κάνετε λήψη της τελευταίας έκδοσης του Azure AD Connect, μεταβείτε στο [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="24cc9-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
