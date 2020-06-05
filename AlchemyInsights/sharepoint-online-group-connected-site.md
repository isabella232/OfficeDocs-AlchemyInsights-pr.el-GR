---
title: Προσθήκη ομάδας σε τοποθεσία του SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582811"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="ad4c1-102">Ζητήματα κατά τη δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας στο SharePoint</span><span class="sxs-lookup"><span data-stu-id="ad4c1-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="ad4c1-103">Ορισμένα συνηθισμένα ζητήματα που παρουσιάστηκαν κατά τη δημιουργία ή την εκ νέου δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας.</span><span class="sxs-lookup"><span data-stu-id="ad4c1-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="ad4c1-104">Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="ad4c1-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="ad4c1-105">Λήψη [κελύφους διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="ad4c1-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="ad4c1-106">Για περισσότερες πληροφορίες σχετικά με τα γρήγορα αποτελέσματα με το Powershell, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="ad4c1-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="ad4c1-107">Καταργήστε την τοποθεσία από τις διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet Powershell [κατάργησης-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="ad4c1-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="ad4c1-108">Το Powershell απαιτείται για τη μόνιμη διαγραφή τοποθεσιών ομάδας.</span><span class="sxs-lookup"><span data-stu-id="ad4c1-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="ad4c1-109">Εάν δημιουργείτε μια συνδεδεμένη ομάδα τοποθεσίακαι λαμβάνετε μια προειδοποίηση: **Υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο**, ελέγξτε τις υπάρχουσες ομάδες από το κέντρο [διαχείρισης του Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="ad4c1-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="ad4c1-110">Για να επιλύσετε το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με διαφορετικό ψευδώνυμο.</span><span class="sxs-lookup"><span data-stu-id="ad4c1-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="ad4c1-111">Υπάρχουν διάφοροι τρόποι δημιουργίας και χρήσης σύγχρονων ομάδων με το SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ad4c1-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="ad4c1-112">Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ad4c1-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="ad4c1-113">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Σύνδεση ομάδας του Microsoft 365 χρησιμοποιώντας το περιβάλλον εργασίας χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="ad4c1-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="ad4c1-114">Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία ομάδας Microsoft 365, θα πρέπει να δημιουργήσετε μια [τοποθεσία ομάδας](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="ad4c1-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
