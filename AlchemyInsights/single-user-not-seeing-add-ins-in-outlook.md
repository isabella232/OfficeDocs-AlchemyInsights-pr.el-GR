---
title: Ο μεμονωμένος χρήστης δεν βλέπει πρόσθετα στο Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197959"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="aa277-102">Ο μεμονωμένος χρήστης δεν βλέπει πρόσθετα στο Outlook</span><span class="sxs-lookup"><span data-stu-id="aa277-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="aa277-103">Ο χρήστης μπορεί να είναι μέρος ενός ρόλου που δεν έχει τη σωστή παράμετρο AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="aa277-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="aa277-104">Εκτελέστε αυτό το cmdlet για να μάθετε αν ο σωστός ρόλος σχετίζεται με το χρήστη:</span><span class="sxs-lookup"><span data-stu-id="aa277-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="aa277-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Ανάθεση $false | Μορφοποίηση-Πίνακας -Αυτόματος ρόλος,Όνομα ΡόλουAssignee,Τύπος RoleAssignee</span><span class="sxs-lookup"><span data-stu-id="aa277-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="aa277-106">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Καθορισμός των διαχειριστών και των χρηστών που μπορούν να εγκαταστήσουν και να διαχειριστούν πρόσθετα για το Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="aa277-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
