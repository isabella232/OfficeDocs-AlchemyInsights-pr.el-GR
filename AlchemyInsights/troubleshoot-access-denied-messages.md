---
title: Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500404"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="c98c6-102">Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση</span><span class="sxs-lookup"><span data-stu-id="c98c6-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="c98c6-103">Εάν κάποιος έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" σε έναν κοινόχρηστο φάκελο στο SharePoint, ο διαχειριστής συλλογής τοποθεσιών μπορεί να έχετε ενεργοποιήσει την "περιορισμένης πρόσβασης χρήστη δικαίωμα κλειδώματος λειτουργία".</span><span class="sxs-lookup"><span data-stu-id="c98c6-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="c98c6-104">Για να απενεργοποιήστε αυτήν τη ρύθμιση:</span><span class="sxs-lookup"><span data-stu-id="c98c6-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="c98c6-105">Μεταβείτε στην τοποθεσία, κάντε κλικ στο εικονίδιο ρυθμίσεις και, στη συνέχεια, κάντε κλικ στο κουμπί **Ρυθμίσεις τοποθεσίας**.</span><span class="sxs-lookup"><span data-stu-id="c98c6-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="c98c6-106">Στην περιοχή **Διαχείριση συλλογής τοποθεσιών**, κάντε κλικ στο κουμπί " **δυνατότητες συλλογής τοποθεσιών**".</span><span class="sxs-lookup"><span data-stu-id="c98c6-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="c98c6-107">Δίπλα στο στοιχείο **κατάσταση λειτουργίας κλειδώματος δικαιωμάτων περιορισμένης πρόσβασης χρήστη**, κάντε κλικ στο κουμπί **Απενεργοποίηση**.</span><span class="sxs-lookup"><span data-stu-id="c98c6-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="c98c6-108">Ένα μήνυμα που δεν επιτρέπεται η πρόσβαση μπορεί επίσης να προκύψει για κοινόχρηστους φακέλους, αν η τοποθεσία είναι μια τοποθεσία δημοσίευσης.</span><span class="sxs-lookup"><span data-stu-id="c98c6-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="c98c6-109">Για πληροφορίες, ανατρέξτε στο θέμα [Πρόσβαση κατά την πρόσβαση σε έναν κοινόχρηστο φάκελο](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="c98c6-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="c98c6-110">Εάν ένα κάποιος έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" όταν προσπαθείτε να προβάλετε αιτήσεις πρόσβασης, ο χρήστης πρέπει να προστεθεί ως διαχειριστής συλλογής τοποθεσιών ή μέλος της ομάδας κατόχων για την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="c98c6-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="c98c6-111">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Πρόσβαση στη λίστα αιτήσεις πρόσβασης](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="c98c6-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="c98c6-112">Εάν ένας χρήστης έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση", αφού ότι αυτά έχουν καταργηθεί από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης και, στη συνέχεια, προστίθεται ξανά, ανατρέξτε στο θέμα [Πρόσβαση όταν ένας λογαριασμός χρήστη είναι συγχρονισμένες με το Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="c98c6-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

