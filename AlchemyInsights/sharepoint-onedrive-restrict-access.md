---
title: Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053765"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="013d3-102">Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="013d3-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="013d3-103">Υπάρχουν πολλοί τρόποι για να περιορίσετε την πρόσβαση στις υπηρεσίες του SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="013d3-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="013d3-104">Αυτές οι διάφορες μέθοδοι περιορισμού πρόσβασης περιγράφονται παρακάτω.</span><span class="sxs-lookup"><span data-stu-id="013d3-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="013d3-105">**Περιορισμός δικαιωμάτων**</span><span class="sxs-lookup"><span data-stu-id="013d3-105">**Permission Restriction**</span></span>

<span data-ttu-id="013d3-106">Στο SharePoint Online και OneDrive για την επιχείρηση, περιορίζουμε την πρόσβαση σε στοιχεία, όπως τοποθεσίες, αρχεία και φακέλους, παρέχοντας πρόσβαση μόνο σε αυτές τις ομάδες/άτομα που θα πρέπει να έχουν πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="013d3-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="013d3-107">Προσαρμογή δικαιωμάτων για μια λίστα ή βιβλιοθήκη του SharePoint</span><span class="sxs-lookup"><span data-stu-id="013d3-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="013d3-108">Προσαρμογή δικαιωμάτων τοποθεσίας SharePoint</span><span class="sxs-lookup"><span data-stu-id="013d3-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="013d3-109">Αλλαγή των δικαιωμάτων σε έναν υποφάκελο</span><span class="sxs-lookup"><span data-stu-id="013d3-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="013d3-110">Έλεγχος πρόσβασης από μη διαχειριζόμενες συσκευές</span><span class="sxs-lookup"><span data-stu-id="013d3-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="013d3-111">Ως ένα SharePoint ή καθολικό διαχειριστή στο Office 365, μπορείτε να αποκλείσετε ή να περιορίσετε την πρόσβαση σε περιεχόμενο του SharePoint και OneDrive από μη διαχειριζόμενες συσκευές (αυτές δεν είναι υβριδική AD συμμετέχει ή συμμορφώνεται με Intune).</span><span class="sxs-lookup"><span data-stu-id="013d3-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="013d3-112">**Περιορισμός θέσης δικτύου**</span><span class="sxs-lookup"><span data-stu-id="013d3-112">**Network Location Restriction**</span></span>

<span data-ttu-id="013d3-113">Ως διαχειριστής ΠΛΗΡΟΦΟΡΙΚΉς, μπορείτε να ελέγχετε την πρόσβαση σε πόρους του SharePoint και του OneDrive με βάση καθορισμένες θέσεις δικτύου που εμπιστεύεστε.</span><span class="sxs-lookup"><span data-stu-id="013d3-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="013d3-114">Αυτό είναι επίσης γνωστό ως πολιτική βάσει τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="013d3-114">This is also known as location-based policy.</span></span> <span data-ttu-id="013d3-115">Για περισσότερες πληροφορίες, ανατρέξτε στο [στοιχείο Έλεγχος πρόσβασης στα δεδομένα του SharePoint Online και OneDrive με βάση τη θέση δικτύου](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="013d3-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="013d3-116">**Περιορισμός κλειδώματος τοποθεσίας**</span><span class="sxs-lookup"><span data-stu-id="013d3-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="013d3-117">Στο SharePoint Online έχετε τη δυνατότητα να κλειδώσετε μια συλλογή τοποθεσιών, ώστε να μην έχει πρόσβαση κανείς.</span><span class="sxs-lookup"><span data-stu-id="013d3-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="013d3-118">Αυτό ορίζεται μέσω PowerShell και το [κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) χρησιμοποιώντας την ιδιότητα [set-τοποθεσία](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -κλείδωμα κατάστασης.</span><span class="sxs-lookup"><span data-stu-id="013d3-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="013d3-119">**Περιορισμός των χρηστών από τη δημιουργία τοποθεσιών ή δευτερευουσών τοποθεσιών**</span><span class="sxs-lookup"><span data-stu-id="013d3-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="013d3-120">Ως διαχειριστής του SharePoint ή καθολικός διαχειριστής του Office 365, μπορείτε να αφήσετε τους χρήστες να δημιουργήσουν και να διαχειριστούν τις δικές τους τοποθεσίες του SharePoint, να καθορίσουν το είδος των τοποθεσιών που μπορούν να δημιουργήσουν και να καθορίσουν τη θέση των τοποθεσιών.</span><span class="sxs-lookup"><span data-stu-id="013d3-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="013d3-121">Για περισσότερες πληροφορίες, ανατρέξτε [στο στοιχείο Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="013d3-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

