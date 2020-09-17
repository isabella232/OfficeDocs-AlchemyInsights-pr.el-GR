---
title: 932 αναβάθμιση AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806039"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="a3576-102">Αναβάθμιση σύνδεσης Azure AD</span><span class="sxs-lookup"><span data-stu-id="a3576-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="a3576-103">Από προεπιλογή, η αυτόματη αναβάθμιση είναι ενεργοποιημένη για το Azure AD Connect, γεγονός που σας βοηθά να διασφαλίσετε ότι χρησιμοποιείτε την πιο πρόσφατη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="a3576-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="a3576-104">Για να επαληθεύσετε τις ρυθμίσεις αυτόματης αναβάθμισης, χρησιμοποιήστε το cmdlet **Get-ADSyncAutoUpgrade** στο Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a3576-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="a3576-105">Το cmdlet θα επιστρέψει μία από τις ακόλουθες τιμές:</span><span class="sxs-lookup"><span data-stu-id="a3576-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="a3576-106">**Ενεργοποιημένο**: η αυτόματη αναβάθμιση είναι ενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="a3576-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="a3576-107">**Απενεργοποιημένη**: η αυτόματη αναβάθμιση είναι απενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="a3576-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="a3576-108">**Αναστέλλεται**: το σύστημα δεν είναι πλέον επιλέξιμο για τη λήψη αυτόματων ενημερώσεων.</span><span class="sxs-lookup"><span data-stu-id="a3576-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="a3576-109">Δεν μπορείτε να ρυθμίσετε τις παραμέτρους αυτής της τιμής. έχει καθοριστεί από το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="a3576-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="a3576-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="a3576-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="a3576-111">Για να κάνετε λήψη της πιο πρόσφατης έκδοσης του Azure AD Connect, μεταβείτε στο [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="a3576-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
