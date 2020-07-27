---
title: Ένας χρήστης λαμβάνει σφάλμα άρνησης πρόσβασης κατά την προσθήκη πρόσθετων στο Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 1f4672e306a282b3e1d20c75f4e361c02cdddaed
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423722"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="b8be8-102">Ένας χρήστης λαμβάνει σφάλμα άρνησης πρόσβασης κατά την προσθήκη πρόσθετων στο Outlook</span><span class="sxs-lookup"><span data-stu-id="b8be8-102">One user gets Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="b8be8-103">Χρήστης PowerShell Για να βρείτε δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="b8be8-103">User PowerShell To find permissions:</span></span>

<span data-ttu-id="b8be8-104">Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Ανάθεση $false | Μορφοποίηση-Πίνακας -Αυτόματος ρόλος,Όνομα ΡόλουAssignee,Τύπος RoleAssignee</span><span class="sxs-lookup"><span data-stu-id="b8be8-104">Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>