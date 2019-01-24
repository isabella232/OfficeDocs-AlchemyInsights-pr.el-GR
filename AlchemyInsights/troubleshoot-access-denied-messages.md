---
title: Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470675"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="2fca1-102">Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση</span><span class="sxs-lookup"><span data-stu-id="2fca1-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="2fca1-p101">Εάν κάποιος έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" σε έναν κοινόχρηστο φάκελο, ο διαχειριστής συλλογής τοποθεσιών μπορεί να έχετε ενεργοποιήσει την "περιορισμένης πρόσβασης χρήστη δικαίωμα κλειδώματος λειτουργία". Για να απενεργοποιήστε αυτήν τη ρύθμιση:</span><span class="sxs-lookup"><span data-stu-id="2fca1-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="2fca1-105">Μεταβείτε στην τοποθεσία, κάντε κλικ στο εικονίδιο ρυθμίσεις και, στη συνέχεια, κάντε κλικ στο κουμπί **Ρυθμίσεις τοποθεσίας**.</span><span class="sxs-lookup"><span data-stu-id="2fca1-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="2fca1-106">Στην περιοχή **Διαχείριση συλλογής τοποθεσιών**, κάντε κλικ στο κουμπί " **δυνατότητες συλλογής τοποθεσιών**".</span><span class="sxs-lookup"><span data-stu-id="2fca1-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="2fca1-107">Δίπλα στο στοιχείο **κατάσταση λειτουργίας κλειδώματος δικαιωμάτων περιορισμένης πρόσβασης χρήστη**, κάντε κλικ στο κουμπί **Απενεργοποίηση**.</span><span class="sxs-lookup"><span data-stu-id="2fca1-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="2fca1-p102">Ένα μήνυμα που δεν επιτρέπεται η πρόσβαση μπορεί επίσης να προκύψει για κοινόχρηστους φακέλους, αν η τοποθεσία είναι μια τοποθεσία δημοσίευσης. Για πληροφορίες, ανατρέξτε στο θέμα [Πρόσβαση κατά την πρόσβαση σε έναν κοινόχρηστο φάκελο](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="2fca1-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="2fca1-p103">Εάν ένα κάποιος έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" όταν προσπαθείτε να προβάλετε αιτήσεις πρόσβασης, ο χρήστης πρέπει να προστεθεί ως διαχειριστής συλλογής τοποθεσιών ή μέλος της ομάδας κατόχων για την τοποθεσία. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Πρόσβαση στη λίστα αιτήσεις πρόσβασης](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="2fca1-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="2fca1-112">Εάν ένας χρήστης έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση", αφού ότι αυτά έχουν καταργηθεί από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης και, στη συνέχεια, προστίθεται ξανά, ανατρέξτε στο θέμα [Πρόσβαση όταν ένας λογαριασμός χρήστη είναι συγχρονισμένες με το Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="2fca1-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

