---
title: Καθολικός διαχειριστής και διαχειριστής του SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002962"
- "5674"
ms.openlocfilehash: bc5a0067ce8dd63134f163daa33e7bc662cfdd96
ms.sourcegitcommit: f5a3b2f436b00e18cbf337044ea8818726517651
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/18/2020
ms.locfileid: "44278995"
---
# <a name="global-and-sharepoint-admin"></a><span data-ttu-id="841fe-102">Καθολικός διαχειριστής και διαχειριστής του SharePoint</span><span class="sxs-lookup"><span data-stu-id="841fe-102">Global and SharePoint admin</span></span>

<span data-ttu-id="841fe-103">Στους διαχειριστές καθολικού και SharePoint πρέπει να εκχωρηθεί μια άδεια χρήσης του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="841fe-103">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="841fe-104">Οι λογαριασμοί που μόλις δημιουργήθηκαν μόλις εκχωρούνται με μια άδεια χρήσης του SharePoint ή ρόλο διαχειριστή ενδέχεται να αντιμετωπίσετε ζητήματα πρόσβασης στο SharePoint, όπως "δεν επιτρέπεται η πρόσβαση" ή "ο χρήστης δεν βρέθηκε".</span><span class="sxs-lookup"><span data-stu-id="841fe-104">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="841fe-105">Δώστε τουλάχιστον 24 ώρες για να ολοκληρωθεί ο συγχρονισμός σε όλα τα συστήματά μας.</span><span class="sxs-lookup"><span data-stu-id="841fe-105">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="841fe-106">Καταλαβαίνουμε ότι 24 ώρες μπορεί να φαίνεται σαν ένα μεγάλο χρονικό διάστημα.</span><span class="sxs-lookup"><span data-stu-id="841fe-106">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="841fe-107">Σε πολλές περιπτώσεις, εργαζόμαστε ήδη για μια λύση.</span><span class="sxs-lookup"><span data-stu-id="841fe-107">In many cases, we're already working on a solution.</span></span>

<span data-ttu-id="841fe-108">Οι χρήστες στους οποίοι έχει ανατεθεί ο ρόλος διαχειριστή global ή SharePoint έχουν πρόσβαση στο κέντρο διαχείρισης του SharePoint και μπορούν να δημιουργούν και να διαχειρίζονται τοποθεσίες (που προηγουμένως ονομάζονταν "συλλογές τοποθεσιών"), να υποδεικνύουν διαχειριστές τοποθεσιών, να διαχειρίζονται ρυθμίσεις κοινής χρήσης και πολλά άλλα.</span><span class="sxs-lookup"><span data-stu-id="841fe-108">Users assigned the Global or SharePoint admin role have access to the SharePoint admin center and can create and manage sites (previously called "site collections"), designate site admins, manage sharing settings, and more.</span></span> <span data-ttu-id="841fe-109">Δεν έχουν αυτόματη πρόσβαση σε όλες τις τοποθεσίες και στο OneDrive κάθε χρήστη, αλλά μπορούν να αποκτήσουν πρόσβαση σε οποιαδήποτε τοποθεσία ή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="841fe-109">They don't have automatic access to all sites and each user's OneDrive, but they can give themselves access to any site or OneDrive.</span></span> <span data-ttu-id="841fe-110">Μπορούν επίσης να χρησιμοποιήσουν το Microsoft PowerShell για τη διαχείριση του SharePoint και του OneDrive.</span><span class="sxs-lookup"><span data-stu-id="841fe-110">They can also use Microsoft PowerShell to manage SharePoint and OneDrive.</span></span>

<span data-ttu-id="841fe-111">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Πληροφορίες για το ρόλο διαχειριστή του SharePoint στο Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role).</span><span class="sxs-lookup"><span data-stu-id="841fe-111">To learn more, see [About the SharePoint admin role in Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role).</span></span>
<span data-ttu-id="841fe-112">Υπάρχουν πολλοί λόγοι για τους οποίους το Microsoft SharePoint ή το Microsoft OneDrive ενδέχεται να μην είναι προσβάσιμα.</span><span class="sxs-lookup"><span data-stu-id="841fe-112">There are several reasons why Microsoft SharePoint or Microsoft OneDrive might become inaccessible.</span></span> <span data-ttu-id="841fe-113">Εάν δεν μπορείτε να έχετε πρόσβαση στο SharePoint Online, χρησιμοποιήστε τον παρακάτω οδηγό για να αντιμετωπίσετε αυτό το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="841fe-113">If you can't access SharePoint Online, use the following guide to troubleshoot this issue.</span></span>

- [<span data-ttu-id="841fe-114">Δεν είναι δυνατή η πρόσβαση στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="841fe-114">Unable to access SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

