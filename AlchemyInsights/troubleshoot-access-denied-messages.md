---
title: Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται η πρόσβαση
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759800"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="05ab4-102">Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται η πρόσβαση</span><span class="sxs-lookup"><span data-stu-id="05ab4-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="05ab4-103">Εάν κάποιος έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" σε έναν κοινόχρηστο φάκελο στο SharePoint, ο διαχειριστής συλλογής τοποθεσιών μπορεί να έχει ενεργοποιήσει τη "λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης".</span><span class="sxs-lookup"><span data-stu-id="05ab4-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="05ab4-104">Για να απενεργοποιήσετε την αυτήν την ενεργοποίηση:</span><span class="sxs-lookup"><span data-stu-id="05ab4-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="05ab4-105">Μεταβείτε στην τοποθεσία, κάντε κλικ στο εικονίδιο Ρυθμίσεις και, στη συνέχεια, κάντε κλικ στην επιλογή **Ρυθμίσεις τοποθεσίας**.</span><span class="sxs-lookup"><span data-stu-id="05ab4-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="05ab4-106">Στην περιοχή **Διαχείριση συλλογής τοποθεσιών**, κάντε κλικ στην επιλογή **Δυνατότητες συλλογής τοποθεσιών**.</span><span class="sxs-lookup"><span data-stu-id="05ab4-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="05ab4-107">Δίπλα στην **επιλογή Λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης**, κάντε κλικ στην επιλογή **Απενεργοποίηση**.</span><span class="sxs-lookup"><span data-stu-id="05ab4-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="05ab4-108">Ένα μήνυμα δεν επιτρέπεται η Access μπορεί επίσης να προκύψει για κοινόχρηστους φακέλους, εάν η τοποθεσία είναι τοποθεσία δημοσίευσης.</span><span class="sxs-lookup"><span data-stu-id="05ab4-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="05ab4-109">Για πληροφορίες, ανατρέξτε στο θέμα [Δεν επιτρέπεται η πρόσβαση κατά την πρόσβαση σε έναν κοινόχρηστο φάκελο](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="05ab4-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="05ab4-110">Εάν κάποιος έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" κατά την προσπάθεια προβολής αιτήσεων πρόσβασης, ο χρήστης πρέπει να προστεθεί είτε ως διαχειριστής συλλογής τοποθεσιών είτε ως μέλος της ομάδας "Κάτοχοι" για την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="05ab4-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="05ab4-111">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Λίστα Μη επιτράπηκε η πρόσβαση σε αιτήσεις πρόσβασης](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="05ab4-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="05ab4-112">Εάν ένας χρήστης έλαβε ένα μήνυμα "Δεν επιτρέπεται η πρόσβαση" μετά την κατάργηση του από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης και, στη συνέχεια, προστέθηκε ξανά, ανατρέξτε στο θέμα [Δεν επιτρέπεται η πρόσβαση όταν ένας λογαριασμός χρήστη συγχρονίζεται με το Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="05ab4-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

