---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή το OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511976"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="4f103-102">Δεν είναι δυνατή η διαγραφή στοιχείων</span><span class="sxs-lookup"><span data-stu-id="4f103-102">Unable to delete items</span></span>

<span data-ttu-id="4f103-103">Οι πολιτικές διατήρησης μπορεί να προκαλέσουν αυτό, πρέπει είτε να απενεργοποιήσετε είτε να εξαιρέσετε την αντίστοιχη διατήρηση που προκαλεί αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="4f103-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="4f103-104">Μετά την κατάργηση μιας πολιτικής διατήρησης ή διατήρησης, ενδέχεται να χρειαστούν έως και 24 ώρες για να εφαρμοστεί η αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="4f103-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="4f103-105">Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) στο στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="4f103-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="4f103-106">Η τοποθεσία ενδέχεται να έχει υπερβεί το όριο αποθήκευσης, να αυξήσει το [όριο τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) και να διαγράψει το στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="4f103-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="4f103-107">Βεβαιωθείτε ότι δεν έχει γίνει ανάληψη ελέγχου του [στοιχείου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="4f103-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="4f103-108">Τέλος, οι διαχειριστές μπορούν να [χρησιμοποιήσουν μοτίβα και πρακτικές του SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), η οποία περιέχει μια βιβλιοθήκη εντολών PowerShell που σας επιτρέπουν να εκτελείτε σύνθετες ενέργειες διαχείρισης, όπως η σταδιακή διαγραφή επίμονων στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="4f103-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="4f103-109">Κατάργηση αρχείου PNP</span><span class="sxs-lookup"><span data-stu-id="4f103-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="4f103-110">Κατάργηση φακέλου PNP</span><span class="sxs-lookup"><span data-stu-id="4f103-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="4f103-111">Κατάργηση στοιχείου λίστας PNP</span><span class="sxs-lookup"><span data-stu-id="4f103-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="4f103-112">Κατάργηση λίστας PNP</span><span class="sxs-lookup"><span data-stu-id="4f103-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="4f103-113">Κατάργηση πεδίου PNP (Στήλη)</span><span class="sxs-lookup"><span data-stu-id="4f103-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)