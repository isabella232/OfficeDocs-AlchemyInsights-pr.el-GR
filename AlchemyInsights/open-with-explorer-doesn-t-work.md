---
title: Άνοιγμα με την Εξερεύνηση δεν λειτουργεί
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764908"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="bcb67-102">Άνοιγμα με την Εξερεύνηση δεν λειτουργεί</span><span class="sxs-lookup"><span data-stu-id="bcb67-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="bcb67-103">Εάν δεν λειτουργεί η **προβολή στην Εξερεύνηση αρχείου** ή **Άνοιγμα με την Εξερεύνηση** βεβαιωθείτε ότι η υπηρεσία WebClient έχει οριστεί να **εκτελεί** , ακολουθώντας τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="bcb67-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="bcb67-104">Για παράδειγμα, ίσως χρειαστούν πολύ χρόνο για να ανοίξετε μια βιβλιοθήκη του SharePoint ή OneDrive, όταν δεν εκτελείται η υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="bcb67-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="bcb67-105">Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε εκτέλεση, επιλέξτε το app επιφάνειας εργασίας εκτέλεση, πληκτρολογήστε services.msc και, στη συνέχεια, επιλέξτε **Enter**.</span><span class="sxs-lookup"><span data-stu-id="bcb67-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="bcb67-106">Κάντε κύλιση έως την υπηρεσία WebClient και ελέγξτε τη στήλη **κατάστασης** .</span><span class="sxs-lookup"><span data-stu-id="bcb67-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="bcb67-107">Εάν η κατάσταση της υπηρεσίας WebClient δεν **εκτελείται**, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στο κουμπί **Έναρξη**και στη συνέχεια κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="bcb67-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="bcb67-108">Ενεργοποίηση της υπηρεσίας, εάν χρειάζεται, με την επιλογή **μη αυτόματη** ή **Αυτόματη** στο πλαίσιο **Τύπος εκκίνησης** .</span><span class="sxs-lookup"><span data-stu-id="bcb67-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="bcb67-109">Για την αντιμετώπιση ζητημάτων ανοίγοντας στην Εξερεύνηση αρχείων, ανατρέξτε στην ενότητα [Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="bcb67-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="bcb67-110">Εξερευνήστε συγχρονισμού ως μια καλύτερη εναλλακτική λύση: [αρχεία συγχρονισμού του SharePoint με το πρόγραμμα-πελάτης συγχρονισμού νέα OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="bcb67-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

