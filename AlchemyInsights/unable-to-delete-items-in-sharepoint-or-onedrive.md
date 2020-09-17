---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή στο OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806111"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="a4c76-102">Δεν είναι δυνατή η διαγραφή στοιχείων</span><span class="sxs-lookup"><span data-stu-id="a4c76-102">Unable to delete items</span></span>

<span data-ttu-id="a4c76-103">Οι πολιτικές διατήρησης μπορεί να προκαλέσουν αυτό το πρόβλημα, πρέπει είτε να απενεργοποιήσετε είτε να εξαιρέσετε τη σχετική αναμονή που προκαλεί αυτό το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="a4c76-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="a4c76-104">Μετά την κατάργηση μιας πολιτικής διατήρησης ή μιας διατήρησης, μπορεί να χρειαστούν έως και 24 ώρες για να ισχύσει η αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="a4c76-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="a4c76-105">Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) στο στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="a4c76-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="a4c76-106">Η τοποθεσία μπορεί να έχει υπερβεί το όριο χώρου αποθήκευσης, να αυξήσει το όριο της [τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) και να διαγράψει το στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="a4c76-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="a4c76-107">Βεβαιωθείτε ότι δεν έχει γίνει [ανάληψη ελέγχου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) του στοιχείου σε άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="a4c76-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="a4c76-108">Τέλος, οι διαχειριστές μπορούν να χρησιμοποιούν [μοτίβα και πρακτικές του SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), τα οποία περιέχουν εντολές του PowerShell, οι οποίες σας επιτρέπουν να εκτελείτε σύνθετες ενέργειες διαχείρισης, όπως η υποχρεωτική Διαγραφή επίμονων στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="a4c76-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="a4c76-109">Κατάργηση αρχείου PNP</span><span class="sxs-lookup"><span data-stu-id="a4c76-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="a4c76-110">Κατάργηση φακέλου τοποθέτησης και άμεσης λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="a4c76-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="a4c76-111">Κατάργηση στοιχείου λίστας τοποθέτησης και άμεσης λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="a4c76-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="a4c76-112">Κατάργηση λίστας τοποθέτησης και άμεσης λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="a4c76-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="a4c76-113">Κατάργηση πεδίου τοποθέτησης και άμεσης λειτουργίας (στήλη)</span><span class="sxs-lookup"><span data-stu-id="a4c76-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)