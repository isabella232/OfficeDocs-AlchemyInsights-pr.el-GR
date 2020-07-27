---
title: Πολλοί χρήστες λαμβάνουν σφάλμα άρνησης πρόσβασης κατά την προσθήκη πρόσθετων στο Outlook
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
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423713"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="99ce2-102">Πολλοί χρήστες λαμβάνουν σφάλμα άρνησης πρόσβασης κατά την προσθήκη πρόσθετων στο Outlook</span><span class="sxs-lookup"><span data-stu-id="99ce2-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="99ce2-103">Μπορείτε να καθορίσετε ποιοι διαχειριστές στην εταιρεία σας έχουν δικαιώματα εγκατάστασης και διαχείρισης πρόσθετων για το Outlook.</span><span class="sxs-lookup"><span data-stu-id="99ce2-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="99ce2-104">Μπορείτε επίσης να καθορίσετε ποιοι χρήστες στην εταιρεία σας έχουν δικαίωμα εγκατάστασης και διαχείρισης πρόσθετων για δική τους χρήση.</span><span class="sxs-lookup"><span data-stu-id="99ce2-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="99ce2-105">Για λεπτομέρειες, ανατρέξτε στο θέμα [Καθορισμός των διαχειριστών και των χρηστών που μπορούν να εγκαταστήσουν και να διαχειριστούν πρόσθετα για το Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="99ce2-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="99ce2-106">Για να επαληθεύσετε ότι έχετε εκχωρήσει με επιτυχία δικαιώματα για ένα χρήστη, αντικαταστήστε <Role Name> με το όνομα του ρόλου που θέλετε να επαληθεύσετε και εκτελέστε την ακόλουθη εντολή στο Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="99ce2-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="99ce2-107">Get-ManagementRoleAssignment -Ρόλος " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="99ce2-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="99ce2-108">Αυτό το παράδειγμα σάς δείχνει πώς μπορείτε να επαληθεύσετε σε ποιον έχετε εκχωρήσει δικαιώματα για την εγκατάσταση πρόσθετων από το Office Store για τον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="99ce2-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="99ce2-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="99ce2-109">PowerShell</span></span>

<span data-ttu-id="99ce2-110">-Ρόλος "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="99ce2-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="99ce2-111">Στα αποτελέσματα, Get-ManagementRoleAssignment, εξετάστε τις καταχωρήσεις στη στήλη Αποτελεσματικοί χρήστες.</span><span class="sxs-lookup"><span data-stu-id="99ce2-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="99ce2-112">Για λεπτομερείς πληροφορίες σύνταξης και παραμέτρων, ανατρέξτε στο θέμα [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="99ce2-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 