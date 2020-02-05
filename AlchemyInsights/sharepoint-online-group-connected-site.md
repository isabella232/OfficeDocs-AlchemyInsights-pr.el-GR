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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770351"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="78e4c-102">Ζητήματα κατά τη δημιουργία μιας ομάδας συνδεδεμένη τοποθεσία στο SharePoint</span><span class="sxs-lookup"><span data-stu-id="78e4c-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="78e4c-103">Ορισμένα συνηθισμένα ζητήματα που παρουσιάζονται κατά τη δημιουργία ή την εκ νέου δημιουργία μιας ομάδας συνδεδεμένης τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="78e4c-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="78e4c-104">Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε μόνιμα την προηγούμενη τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="78e4c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="78e4c-105">Κατεβάστε το [κέλυφος διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="78e4c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="78e4c-106">Για περισσότερες πληροφορίες σχετικά με τα γρήγορα αποτελέσματα με το PowerShell, δείτε [γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="78e4c-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="78e4c-107">Καταργήστε την τοποθεσία από διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet [Κατάργηση-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="78e4c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="78e4c-108">Απαιτείται PowerShell για τη μόνιμη διαγραφή τοποθεσιών ομάδας.</span><span class="sxs-lookup"><span data-stu-id="78e4c-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="78e4c-109">Εάν δημιουργείτε μια ομάδα συνδεδεμένη τοποθεσία και λαμβάνετε μια προειδοποίηση: **υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο**, ελέγξτε τις υπάρχουσες ομάδες από το [Office 365 από το κέντρο διαχείρισης](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="78e4c-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="78e4c-110">Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με ένα διαφορετικό ψευδώνυμο αντιστοιχισμένο.</span><span class="sxs-lookup"><span data-stu-id="78e4c-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="78e4c-111">Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε σύγχρονες ομάδες με το SharePoint.</span><span class="sxs-lookup"><span data-stu-id="78e4c-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="78e4c-112">Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365.</span><span class="sxs-lookup"><span data-stu-id="78e4c-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="78e4c-113">Για περισσότερες πληροφορίες, ανατρέξτε [στο σημείο σύνδεση μιας ομάδας του Office 365 χρησιμοποιώντας το περιβάλλον εργασίας χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="78e4c-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="78e4c-114">Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία του Office 365 Group, θα πρέπει να δημιουργήσετε μια [τοποθεσία ομάδας](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="78e4c-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
