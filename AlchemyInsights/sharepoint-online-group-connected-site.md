---
title: Προσθήκη ομάδας σε μια τοποθεσία του SharePoint
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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051101"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="eebde-102">Ζητήματα κατά τη δημιουργία ή την ομαδοποίηση συνδεδεμένων τοποθεσιών στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="eebde-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="eebde-103">Υπάρχουν μερικά συνηθισμένα ζητήματα που παρουσιάστηκαν κατά τη δημιουργία ή την εκ νέου δημιουργία μιας ομάδας συνδεδεμένων τοποθεσιών.</span><span class="sxs-lookup"><span data-stu-id="eebde-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="eebde-104">Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="eebde-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="eebde-105">Κατεβάστε το [κέλυφος διαχείρισης του Μπίσπο](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="eebde-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="eebde-106">Για περισσότερες πληροφορίες σχετικά με γρήγορα αποτελέσματα με PowerShell, δείτε [γρήγορα αποτελέσματα με το SharePoint Online κέλυφος διαχείρισης](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="eebde-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="eebde-107">Κατάργηση της τοποθεσίας από διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet PowerShell [Διαγραφή τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="eebde-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="eebde-108">Εάν δημιουργείτε μια τοποθεσία συνδεδεμένη σε ομάδα και λαμβάνετε μια προειδοποίηση μια άλλη ομάδα με το ίδιο ψευδώνυμο υπάρχει ήδη, ελέγξτε τις υπάρχουσες ομάδες από το [Office 365 από το κέντρο διαχείρισης](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="eebde-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="eebde-109">Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με διαφορετικό ψευδώνυμο που έχει αντιστοιχιστεί.</span><span class="sxs-lookup"><span data-stu-id="eebde-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="eebde-110">Υπάρχουν διαφορετικοί τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε σύγχρονες ομάδες με το SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eebde-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="eebde-111">Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365.</span><span class="sxs-lookup"><span data-stu-id="eebde-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="eebde-112">Για περισσότερες πληροφορίες, ανατρέξτε [στο αρχείο σύνδεση μιας ομάδας του Office 365 χρησιμοποιώντας το χρήστη του SharePoint το ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="eebde-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="eebde-113">Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία της ομάδας Office 365, θα πρέπει να δημιουργήσετε μια τοποθεσία ομάδας.</span><span class="sxs-lookup"><span data-stu-id="eebde-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="eebde-114">Για περισσότερες πληροφορίες, ανατρέξτε [στο σημείο δημιουργία μιας τοποθεσίας ομάδας στο SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="eebde-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

