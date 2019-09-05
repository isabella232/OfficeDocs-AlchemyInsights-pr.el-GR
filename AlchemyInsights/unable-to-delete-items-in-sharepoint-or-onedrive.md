---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή στο OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748555"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="88b03-102">Δεν είναι δυνατή η διαγραφή στοιχείων</span><span class="sxs-lookup"><span data-stu-id="88b03-102">Unable to delete items</span></span>

<span data-ttu-id="88b03-103">Αντιμετωπίζετε προβλήματα με τη διαγραφή στοιχείων του SharePoint;</span><span class="sxs-lookup"><span data-stu-id="88b03-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="88b03-104">Να είστε πάντα βέβαιοι ότι έχετε τα [κατάλληλα δικαιώματα](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) για να διαγράψετε το στοιχείο ή ότι ένας [διαχειριστής συλλογής τοποθεσιών](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) επιχειρεί να καταργήσει το στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="88b03-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="88b03-105">Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/office365/securitycompliance/retention-policies) στο στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="88b03-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="88b03-106">Βεβαιωθείτε ότι το στοιχείο δεν έχει γίνει [ανάληψη ελέγχου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="88b03-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="88b03-107">Τέλος, οι διαχειριστές μπορούν να χρησιμοποιούν το [SharePoint μοτίβα και πρακτικές](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) που περιέχει μια βιβλιοθήκη των εντολών PowerShell που σας επιτρέπουν να εκτελέσετε σύνθετες ενέργειες διαχείρισης, όπως η αναγκαστική Διαγραφή πεισματική στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="88b03-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="88b03-108">Κατάργηση αρχείου PNP</span><span class="sxs-lookup"><span data-stu-id="88b03-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="88b03-109">Κατάργηση φακέλου PNP</span><span class="sxs-lookup"><span data-stu-id="88b03-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="88b03-110">Κατάργηση στοιχείου λίστας PNP</span><span class="sxs-lookup"><span data-stu-id="88b03-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="88b03-111">Κατάργηση λίστας PNP</span><span class="sxs-lookup"><span data-stu-id="88b03-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="88b03-112">Κατάργηση πεδίου PNP (στήλη)</span><span class="sxs-lookup"><span data-stu-id="88b03-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)