---
title: Περιορισμός της πρόσβασης στο SharePoint ή OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471083"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8f76d-102">Περιορισμός της πρόσβασης στο SharePoint ή OneDrive</span><span class="sxs-lookup"><span data-stu-id="8f76d-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8f76d-p101">Στο SharePoint και OneDrive, περιορίσετε την πρόσβαση σε στοιχεία, όπως αρχεία, φακέλους και λίστες εκχωρώντας πρόσβαση μόνο σε ομάδες ή μεμονωμένους χρήστες που θέλετε να έχετε πρόσβαση. Από προεπιλογή, τα δικαιώματα στο SharePoint έχουν μεταβιβαστεί από επάνω υψηλότερα στην ιεραρχία. Έτσι ένα αρχείο μεταβιβάζονται τα δικαιώματα από το φάκελο, το οποίο μεταβιβάζονται τα δικαιώματα από τη βιβλιοθήκη, το οποίο μεταβιβάζονται τα δικαιώματα από την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="8f76d-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="8f76d-p102">Μπορείτε να κάνετε κοινή χρήση σε υψηλότερο επίπεδο (όπως με την κοινή χρήση ολόκληρης της τοποθεσίας) και στη συνέχεια να διακόψετε τη μεταβίβαση, εάν δεν θέλετε να κάνετε κοινή χρήση όλων των στοιχείων στην τοποθεσία. Ωστόσο, δεν συνιστάται επειδή καθιστά τη διατήρηση των δικαιωμάτων πιο σύνθετη και σύγχυση στο μέλλον. Εδώ είναι τι θα κάνατε στη θέση:</span><span class="sxs-lookup"><span data-stu-id="8f76d-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="8f76d-109">Εάν, για παράδειγμα, θέλετε να μοιραστείτε όλα τα περιεχόμενα ενός φακέλου, εκτός από ένα αρχείο σε αυτό, θα πρέπει να μετακινήσετε αυτό το αρχείο σε μια νέα θέση που δεν είναι κοινόχρηστο.</span><span class="sxs-lookup"><span data-stu-id="8f76d-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="8f76d-110">Εάν έχετε δύο υποφακέλους σε ένα φάκελο και θέλετε να χρησιμοποιείτε από κοινού έναν υποφάκελο με ομάδες Α και Β και επιτρέπεται μόνο η ομάδα Α πρόσβαση στον δεύτερο υποφάκελο, κοινή χρήση στον γονικό φάκελο με ομάδα Α και Προσθήκη ομάδας Β στον πρώτο υποφάκελο.</span><span class="sxs-lookup"><span data-stu-id="8f76d-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="8f76d-111">Διακόψετε την κοινή χρήση ενός αρχείου ή φακέλου</span><span class="sxs-lookup"><span data-stu-id="8f76d-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

