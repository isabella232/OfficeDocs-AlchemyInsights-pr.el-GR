---
title: Θέση δεδομένων
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655282"
---
# <a name="data-location"></a><span data-ttu-id="41912-102">Θέση δεδομένων</span><span class="sxs-lookup"><span data-stu-id="41912-102">Data location</span></span>

<span data-ttu-id="41912-103">Μπορείτε να προβάλετε τη θέση του μισθωτή σας στο κέντρο διαχείρισης ή συνδέοντας στο Exchange Online μέσω του PowerShell.</span><span class="sxs-lookup"><span data-stu-id="41912-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="41912-104">**Κέντρο διαχείρισης:**</span><span class="sxs-lookup"><span data-stu-id="41912-104">**Admin center:**</span></span>
1. <span data-ttu-id="41912-105">Συνδεθείτε στο [κέντρο διαχείρισης](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="41912-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="41912-106">Επιλέξτε**προφίλ οργάνωσης** **ρυθμίσεων** > .</span><span class="sxs-lookup"><span data-stu-id="41912-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="41912-107">Στην περιοχή **Θέση δεδομένων**, επιλέξτε **Προβολή λεπτομερειών**.</span><span class="sxs-lookup"><span data-stu-id="41912-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="41912-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="41912-108">**PowerShell:**</span></span>
1. <span data-ttu-id="41912-109">Συνδεθείτε στο Exchange Online χρησιμοποιώντας το Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="41912-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="41912-110">Εκτελέστε το cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) για να εμφανίσετε μια λίστα με τις ιδιότητες του μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="41912-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="41912-111">Κοιτάξτε την ιδιότητα OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="41912-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="41912-112">Όταν έχετε τη θέση δεδομένων για EXO και SPO, μπορείτε να προσδιορίσετε τη θέση δεδομένων για άλλες υπηρεσίες που μπορείτε να χρησιμοποιήσετε από [το σημείο όπου βρίσκονται τα δεδομένα σας](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="41912-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>