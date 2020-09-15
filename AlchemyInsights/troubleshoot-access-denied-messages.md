---
title: Αντιμετώπιση προβλημάτων σε μηνύματα που δεν επιτρέπονται
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690783"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="889a2-102">Αντιμετώπιση προβλημάτων σε μηνύματα που δεν επιτρέπονται</span><span class="sxs-lookup"><span data-stu-id="889a2-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="889a2-103">Εάν κάποιος έλαβε ένα μήνυμα "δεν επιτρέπεται η πρόσβαση" σε έναν κοινόχρηστο φάκελο στο SharePoint, ο διαχειριστής της συλλογής τοποθεσιών μπορεί να έχει ενεργοποιήσει τη λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="889a2-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="889a2-104">Για να την απενεργοποιήσετε:</span><span class="sxs-lookup"><span data-stu-id="889a2-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="889a2-105">Μεταβείτε στην τοποθεσία, κάντε κλικ στο εικονίδιο Ρυθμίσεις και, στη συνέχεια, κάντε κλικ στην επιλογή **Ρυθμίσεις τοποθεσίας**.</span><span class="sxs-lookup"><span data-stu-id="889a2-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="889a2-106">Στην περιοχή **Διαχείριση συλλογής τοποθεσιών**, κάντε κλικ στην επιλογή **δυνατότητες συλλογής τοποθεσιών**.</span><span class="sxs-lookup"><span data-stu-id="889a2-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="889a2-107">Δίπλα στη **λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης**, κάντε κλικ στην επιλογή **Απενεργοποίηση**.</span><span class="sxs-lookup"><span data-stu-id="889a2-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="889a2-108">Ένα μήνυμα που δεν επιτρέπεται η πρόσβαση μπορεί επίσης να προκύψει για κοινόχρηστους φακέλους, εάν η τοποθεσία είναι μια τοποθεσία δημοσίευσης.</span><span class="sxs-lookup"><span data-stu-id="889a2-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="889a2-109">Για πληροφορίες, ανατρέξτε [στο θέμα δεν επιτρέπεται η πρόσβαση κατά την πρόσβαση σε έναν κοινόχρηστο φάκελο](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="889a2-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="889a2-110">Εάν κάποιος έλαβε ένα μήνυμα "δεν επιτρέπεται η πρόσβαση" όταν προσπαθεί να προβάλει αιτήσεις πρόσβασης, ο χρήστης πρέπει να προστεθεί ως διαχειριστής συλλογής τοποθεσιών ή ως μέλος της ομάδας κατόχων για την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="889a2-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="889a2-111">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα δεν επιτρέπεται η πρόσβαση στη λίστα αιτήσεις πρόσβασης](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="889a2-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="889a2-112">Εάν ένας χρήστης έλαβε ένα μήνυμα "δεν επιτρέπεται η πρόσβαση" μετά την κατάργησή του από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης και, στη συνέχεια, πρόσθεσε ξανά, ανατρέξτε στο θέμα [δεν επιτρέπεται η πρόσβαση όταν ένας λογαριασμός χρήστη είναι συγχρονισμένος με το Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="889a2-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

