---
title: Ανάπτυξη προσθεμάτων για Εφαρμογές Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233526"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="d1af9-102">Ανάπτυξη προσθεμάτων για Εφαρμογές Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d1af9-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="d1af9-103">Η κεντρική ανάπτυξη είναι ο προτεινόμενος τρόπος για Office πρόσθετα σε χρήστες και ομάδες εντός του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="d1af9-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="d1af9-104">Για να αναπτύξετε πρόσθετα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="d1af9-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="d1af9-105">**Σημείωση:** Για να εγκαταστήσετε πρόσθετα για Office ως μεμονωμένο χρήστη, ανατρέξτε στο θέμα Προβολή, διαχείριση και εγκατάσταση προσθεμάτων [σε Office προγραμμάτων.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="d1af9-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="d1af9-106">Επίσης, βεβαιωθείτε ότι η μεμονωμένη απόκτηση Office του Store είναι ενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="d1af9-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="d1af9-107">Για λεπτομέρειες, ανατρέξτε στο θέμα Αποτροπή λήψεων προσθεμάτων απενεργοποιώντας το Office Store σε όλα τα [προγράμματα-πελάτες (εκτός Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="d1af9-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="d1af9-108">Βεβαιωθείτε ότι το περιβάλλον σας πληροί τις απαιτήσεις για την ανάπτυξη προσθεμάτων χρησιμοποιώντας την Κεντρική ανάπτυξη.</span><span class="sxs-lookup"><span data-stu-id="d1af9-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="d1af9-109">Για λεπτομέρειες, ανατρέξτε στο θέμα ["Απαιτήσεις".](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="d1af9-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="d1af9-110">Μεταβείτε **Ρυθμίσεις**  >  **"Λήψη**  >  **εφαρμογών"** στο Microsoft 365 διαχείρισης για να αναπτύξετε πρόσθετα.</span><span class="sxs-lookup"><span data-stu-id="d1af9-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="d1af9-111">Σημειώσεις:</span><span class="sxs-lookup"><span data-stu-id="d1af9-111">Notes:</span></span> 

- <span data-ttu-id="d1af9-112">Οι ενσωματωμένες εφαρμογές απαιτούν ο διαχειριστής να έχει δικαιώματα καθολικού διαχειριστή Exchange διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="d1af9-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="d1af9-113">Κατά την ανάπτυξη προσθεμάτων σε πολλούς χρήστες, συνιστάται να κάνετε αναθέσεις εργασιών χρησιμοποιώντας ομάδες αντί για μεμονωμένους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="d1af9-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="d1af9-114">Για λεπτομέρειες, [ανατρέξτε στο θέμα "Ζητήματα" κατά την εκχώρηση ενός προσθέτου σε χρήστες και ομάδες.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="d1af9-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="d1af9-115">Η κεντρική ανάπτυξη δεν υποστηρίζει χρήστες σε ένθετες ομάδες ή ομάδες που έχουν γονικές ομάδες.</span><span class="sxs-lookup"><span data-stu-id="d1af9-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="d1af9-116">Για λεπτομέρειες, ανατρέξτε [στο θέμα Αναθέσεις εργασιών χρηστών και ομάδων.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="d1af9-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="d1af9-117">Βεβαιωθείτε ότι η υπηρεσία διαχείρισης εφαρμογών του Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') είναι ενεργοποιημένη για να πραγματοποιήσουν είσοδο οι χρήστες.</span><span class="sxs-lookup"><span data-stu-id="d1af9-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="d1af9-118">Για λεπτομέρειες, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων ιδιοτήτων εφαρμογής.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="d1af9-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="d1af9-119">Εάν αντιμετωπίζετε προβλήματα με την ανάπτυξη προσθεμάτων χρησιμοποιώντας ενσωματωμένες εφαρμογές, δοκιμάστε να αναπτύξετε χρησιμοποιώντας [πρόσθετα.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="d1af9-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="d1af9-120">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="d1af9-120">For more information, see:</span></span>

<span data-ttu-id="d1af9-121">[Ανάπτυξη προσθεμάτων στο κέντρο διαχείρισης](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Διαχείριση προσθεμάτων στο κέντρο διαχείρισης](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Χρήση των cmdlet Του PowerShell κεντρικής ανάπτυξης για τη διαχείριση προσθεμάτων](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Δημοσίευση Office με χρήση της Κεντρικής ανάπτυξης μέσω του Microsoft 365 διαχείρισης](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Αντιμετώπιση προβλημάτων: Ο χρήστης δεν βλέπει πρόσθετα](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Αντιμετώπιση σφαλμάτων χρήστη με Office πρόσθετα](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="d1af9-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>