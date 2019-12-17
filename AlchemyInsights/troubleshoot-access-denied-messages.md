---
title: Αντιμετώπιση προβλημάτων μηνυμάτων άρνησης πρόσβασης
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050705"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="ccc32-102">Αντιμετώπιση προβλημάτων μηνυμάτων άρνησης πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="ccc32-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="ccc32-103">Εάν κάποιος πήρε ένα μήνυμα "δεν επιτρέπεται η πρόσβαση" σε έναν κοινόχρηστο φάκελο στο SharePoint, ο διαχειριστής της συλλογής τοποθεσιών μπορεί να έχει ενεργοποιήσει τη "λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης".</span><span class="sxs-lookup"><span data-stu-id="ccc32-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="ccc32-104">Για να το απενεργοποιήσετε:</span><span class="sxs-lookup"><span data-stu-id="ccc32-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="ccc32-105">Αναζητήστε την τοποθεσία, κάντε κλικ στο εικονίδιο Ρυθμίσεις και, στη συνέχεια, κάντε κλικ στην επιλογή **Ρυθμίσεις τοποθεσίας**.</span><span class="sxs-lookup"><span data-stu-id="ccc32-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="ccc32-106">Στην περιοχή **Διαχείριση συλλογής τοποθεσιών**, κάντε κλικ στις **δυνατότητες συλλογής τοποθεσιών**.</span><span class="sxs-lookup"><span data-stu-id="ccc32-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="ccc32-107">Δίπλα στη **λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης**, κάντε κλικ στην επιλογή **Απενεργοποίηση**.</span><span class="sxs-lookup"><span data-stu-id="ccc32-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="ccc32-108">Ένα μήνυμα άρνησης πρόσβασης μπορεί επίσης να προκύψει για κοινόχρηστους φακέλους, εάν η τοποθεσία είναι μια τοποθεσία δημοσίευσης.</span><span class="sxs-lookup"><span data-stu-id="ccc32-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="ccc32-109">Για πληροφορίες, ανατρέξτε [στην ενότητα δεν επιτρέπεται η πρόσβαση κατά την πρόσβαση σε κοινόχρηστο φάκελο](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="ccc32-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="ccc32-110">Εάν κάποιος πήρε ένα μήνυμα "δεν επιτρέπεται η πρόσβαση" κατά την προσπάθεια προβολής αιτήσεων πρόσβασης, ο χρήστης πρέπει να προστεθεί είτε ως διαχειριστής συλλογής τοποθεσιών είτε ως μέλος της ομάδας κατόχων για την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="ccc32-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="ccc32-111">Για περισσότερες πληροφορίες, ανατρέξτε [στο αρχείο δεν επιτρέπεται η πρόσβαση στη λίστα αιτημάτων πρόσβασης](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="ccc32-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="ccc32-112">Εάν ένας χρήστης πήρε ένα μήνυμα "δεν επιτρέπεται η πρόσβαση" μετά την κατάργησή τους από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης και, στη συνέχεια, προστέθηκε πίσω, δείτε την [πρόσβαση δεν επιτρέπεται όταν ένας λογαριασμός χρήστη είναι συγχρονισμένες με το Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="ccc32-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

