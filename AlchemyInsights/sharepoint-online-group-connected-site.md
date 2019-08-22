---
title: Προσθήκη μιας ομάδας σε μια τοποθεσία του SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507847"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="0f785-102">Ζητήματα κατά τη δημιουργία ή την ομάδα συνδεδεμένες τοποθεσίες SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0f785-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="0f785-103">Υπάρχουν μερικά κοινά θέματα που προέκυψαν κατά τη δημιουργία ή την εκ νέου δημιουργία ομάδας συνδεδεμένη τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="0f785-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="0f785-104">Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="0f785-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="0f785-105">Λήψη [κέλυφος διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="0f785-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="0f785-106">Για περισσότερες πληροφορίες σχετικά με γρήγορα αποτελέσματα με το powershell, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με το SharePoint Online κέλυφος διαχείρισης](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="0f785-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="0f785-107">Καταργήστε την τοποθεσία από διαγραφή τοποθεσίες χρησιμοποιώντας το cmdlet powershell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="0f785-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="0f785-108">Εάν δημιουργείτε μια συνδεδεμένη τοποθεσία ομάδας και λάβετε μια προειδοποίηση, υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο, ελέγξτε τις υπάρχουσες ομάδες από το [Office 365 από το Κέντρο διαχείρισης](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="0f785-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="0f785-109">Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήσετε την τοποθεσία με διαφορετικό ψευδώνυμο που έχει αντιστοιχιστεί.</span><span class="sxs-lookup"><span data-stu-id="0f785-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="0f785-110">Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε τις σύγχρονες ομάδες με το SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0f785-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="0f785-111">Μπορείτε να συνδέσετε τις υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365.</span><span class="sxs-lookup"><span data-stu-id="0f785-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="0f785-112">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [σύνδεση μια ομάδα Office 365 χρησιμοποιώντας το ineterface χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="0f785-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="0f785-113">Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία ομάδας του Office 365, θα χρειαστεί να δημιουργήσετε μια τοποθεσία ομάδας.</span><span class="sxs-lookup"><span data-stu-id="0f785-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="0f785-114">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Δημιουργία τοποθεσίας ομάδας του SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="0f785-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

