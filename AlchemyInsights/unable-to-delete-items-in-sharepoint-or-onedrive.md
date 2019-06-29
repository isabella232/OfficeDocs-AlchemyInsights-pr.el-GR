---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή OneDrive
ms.author: kirks
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
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366533"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="241bf-102">Δεν είναι δυνατή η διαγραφή στοιχείων</span><span class="sxs-lookup"><span data-stu-id="241bf-102">Unable to delete items</span></span>

<span data-ttu-id="241bf-103">Αντιμετωπίζετε ζητήματα με τη διαγραφή στοιχείων;</span><span class="sxs-lookup"><span data-stu-id="241bf-103">Having issues deleting items?</span></span>

- <span data-ttu-id="241bf-104">Πάντα βεβαιωθείτε ότι έχετε τα [κατάλληλα δικαιώματα](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) για να διαγράψετε το στοιχείο ή να έχετε μια προσπάθεια [διαχειριστής συλλογής τοποθεσιών](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) , κατάργηση του στοιχείου.</span><span class="sxs-lookup"><span data-stu-id="241bf-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="241bf-105">Βεβαιωθείτε ότι δεν υπάρχει μια ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/office365/securitycompliance/retention-policies) στο στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="241bf-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="241bf-106">Βεβαιωθείτε ότι το στοιχείο δεν είναι [ανάληψη ελέγχου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="241bf-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="241bf-107">Τέλος, οι διαχειριστές μπορούν να χρησιμοποιούν [SharePoint μοτίβα και πρακτικές](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) που περιέχει μια βιβλιοθήκη του PowerShell εντολές που σας επιτρέπουν να εκτελέσετε ενέργειες διαχείρισης πολύπλοκων όπως επιβάλλει τη διαγραφή stubborn στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="241bf-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="241bf-108">Κατάργηση αρχείου Τοποθέτησης και Άμεσης Λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="241bf-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="241bf-109">Κατάργηση του φακέλου Τοποθέτησης και Άμεσης Λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="241bf-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="241bf-110">Κατάργηση στοιχείου λίστας Τοποθέτησης και Άμεσης Λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="241bf-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="241bf-111">Κατάργηση της λίστας Τοποθέτησης και Άμεσης Λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="241bf-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="241bf-112">Κατάργηση Τοποθέτησης και Άμεσης Λειτουργίας πεδίο (στήλη)</span><span class="sxs-lookup"><span data-stu-id="241bf-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)