---
title: Αντιμετώπιση προβλημάτων για μηνύματα που δεν επιτρέπεται να έχουν πρόσβαση
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704894"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="b32eb-102">Αντιμετώπιση προβλημάτων για μηνύματα που δεν επιτρέπεται να έχουν πρόσβαση</span><span class="sxs-lookup"><span data-stu-id="b32eb-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="b32eb-103">Εάν κάποιος εμφανιστεί το μήνυμα "Δεν επιτρέπεται η πρόσβαση" σε έναν κοινόχρηστο φάκελο στο SharePoint, ο διαχειριστής της συλλογής τοποθεσιών ενδέχεται να έχει ενεργοποιήσει τη "Λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης".</span><span class="sxs-lookup"><span data-stu-id="b32eb-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="b32eb-104">Για να το απενεργοποιήσετε:</span><span class="sxs-lookup"><span data-stu-id="b32eb-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="b32eb-105">Μεταβείτε στην τοποθεσία, κάντε κλικ στο εικονίδιο "Ρυθμίσεις" και, στη συνέχεια, κάντε κλικ στην **επιλογή "Ρυθμίσεις τοποθεσίας".**</span><span class="sxs-lookup"><span data-stu-id="b32eb-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="b32eb-106">Στην περιοχή **"Διαχείριση συλλογής τοποθεσιών",** κάντε κλικ **στην επιλογή "Δυνατότητες συλλογής τοποθεσιών".**</span><span class="sxs-lookup"><span data-stu-id="b32eb-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="b32eb-107">Δίπλα στη λειτουργία **κλειδώματος δικαιωμάτων χρηστών με περιορισμένη πρόσβαση, κάντε** κλικ στην **επιλογή "Απενεργοποίηση".**</span><span class="sxs-lookup"><span data-stu-id="b32eb-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="b32eb-108">Ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" μπορεί επίσης να προκύψει για κοινόχρηστους φακέλους, εάν η τοποθεσία είναι μια τοποθεσία δημοσίευσης.</span><span class="sxs-lookup"><span data-stu-id="b32eb-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="b32eb-109">Για πληροφορίες, ανατρέξτε [στο θέμα "Δεν επιτρέπεται η πρόσβαση" κατά την πρόσβαση σε έναν κοινόχρηστο φάκελο.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="b32eb-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="b32eb-110">Εάν κάποιος εμφανίζεται το μήνυμα "Δεν επιτρέπεται η πρόσβαση" όταν προσπαθεί να δει αιτήσεις πρόσβασης, ο χρήστης πρέπει να προστεθεί είτε ως διαχειριστής συλλογής τοποθεσιών είτε ως μέλος της ομάδας "Κάτοχοι" για την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="b32eb-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="b32eb-111">Για περισσότερες πληροφορίες, ανατρέξτε στη [λίστα "Δεν επιτρέπεται η πρόσβαση σε αιτήσεις πρόσβασης".](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="b32eb-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="b32eb-112">Εάν ένας χρήστης λαμβάνει το μήνυμα "Δεν επιτρέπεται η πρόσβαση" αφού καταργήθηκε από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης και, στη συνέχεια, προστεθεί ξανά, ανατρέξτε στο θέμα "Δεν επιτρέπεται η πρόσβαση" όταν ένας λογαριασμός χρήστη συγχρονίζεται με το [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="b32eb-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

