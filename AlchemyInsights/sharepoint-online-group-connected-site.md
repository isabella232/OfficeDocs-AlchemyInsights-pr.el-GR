---
title: Προσθήκη ομάδας σε τοποθεσία του SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771202"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="c2917-102">Ζητήματα κατά τη δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας στο SharePoint</span><span class="sxs-lookup"><span data-stu-id="c2917-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="c2917-103">Ορισμένα συνηθισμένα προβλήματα που παρουσιάζονται κατά τη δημιουργία ή την εκ νέου δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας.</span><span class="sxs-lookup"><span data-stu-id="c2917-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="c2917-104">Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="c2917-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="c2917-105">Λήψη [κελύφους διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="c2917-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="c2917-106">Για περισσότερες πληροφορίες σχετικά με τα γρήγορα αποτελέσματα με το PowerShell, ανατρέξτε στο θέμα [γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="c2917-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="c2917-107">Καταργήστε την τοποθεσία από διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c2917-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="c2917-108">Το PowerShell απαιτείται για τη μόνιμη διαγραφή τοποθεσιών ομάδας.</span><span class="sxs-lookup"><span data-stu-id="c2917-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="c2917-109">Εάν δημιουργείτε μια ομάδα συνδεδεμένη τοποθεσία και λαμβάνετε μια προειδοποίηση: **υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο**, επιλέξτε τις υπάρχουσες ομάδες από το [Κέντρο διαχείρισης του Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="c2917-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="c2917-110">Για να επιλύσετε το πρόβλημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με ένα διαφορετικό ψευδώνυμο αντιστοιχισμένο.</span><span class="sxs-lookup"><span data-stu-id="c2917-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="c2917-111">Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε σύγχρονες ομάδες με το SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c2917-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="c2917-112">Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c2917-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="c2917-113">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα σύνδεση μιας ομάδας Microsoft 365 με το περιβάλλον εργασίας χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="c2917-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="c2917-114">Για να δημιουργήσετε μια τοποθεσία Microsoft 365 που είναι συνδεδεμένη στην ομάδα, θα πρέπει να δημιουργήσετε μια [τοποθεσία ομάδας](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="c2917-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
