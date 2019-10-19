---
title: Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551451"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="e39ee-102">Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="e39ee-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="e39ee-103">Στο SharePoint και το OneDrive, περιορίζετε την πρόσβαση σε στοιχεία, όπως αρχεία, φακέλους και λίστες, παραχωρώντας πρόσβαση μόνο σε ομάδες ή άτομα στα οποία θέλετε να έχετε πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="e39ee-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="e39ee-104">Από προεπιλογή, τα δικαιώματα στο SharePoint μεταβιβάζονται από υψηλότερα επάνω στην ιεραρχία.</span><span class="sxs-lookup"><span data-stu-id="e39ee-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="e39ee-105">Έτσι, ένα αρχείο κληρονομεί τα δικαιώματά του από το φάκελο, ο οποίος κληρονομεί τα δικαιώματά του από τη βιβλιοθήκη, το οποίο κληρονομεί τα δικαιώματά του από την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="e39ee-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="e39ee-106">Μπορείτε να κάνετε κοινή χρήση σε υψηλότερο επίπεδο (όπως με την κοινή χρήση μιας ολόκληρης τοποθεσίας) και στη συνέχεια να σπάσετε τη μεταβίβαση, αν δεν θέλετε να κάνετε κοινή χρήση όλων των στοιχείων της τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="e39ee-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="e39ee-107">Ωστόσο, δεν το προτείνουμε αυτό επειδή καθιστά τη διατήρηση των δικαιωμάτων πιο περίπλοκη και σύγχυση στο μέλλον.</span><span class="sxs-lookup"><span data-stu-id="e39ee-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="e39ee-108">Εδώ είναι τι μπορείτε να κάνετε αντ ' αυτού:</span><span class="sxs-lookup"><span data-stu-id="e39ee-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="e39ee-109">Εάν, για παράδειγμα, θέλετε να κάνετε κοινή χρήση όλων των περιεχομένων ενός φακέλου εκτός από ένα αρχείο, μετακινήστε αυτό το αρχείο σε μια νέα θέση που δεν είναι κοινόχρηστη.</span><span class="sxs-lookup"><span data-stu-id="e39ee-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="e39ee-110">Εάν έχετε δύο υποφακέλους σε ένα φάκελο και θέλετε να κάνετε κοινή χρήση ενός υποφακέλου με τις ομάδες A και B και να επιτρέψετε μόνο στην ομάδα A πρόσβαση στον δεύτερο υποφάκελο, μοιραστείτε το γονικό φάκελο με την ομάδα α και προσθέστε την ομάδα β στον πρώτο υποφάκελο.</span><span class="sxs-lookup"><span data-stu-id="e39ee-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="e39ee-111">Διακοπή κοινής χρήσης αρχείου ή φακέλου</span><span class="sxs-lookup"><span data-stu-id="e39ee-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

