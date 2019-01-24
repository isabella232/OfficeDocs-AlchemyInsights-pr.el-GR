---
title: Άνοιγμα με την Εξερεύνηση δεν λειτουργεί
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470685"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="17f9a-102">Άνοιγμα με την Εξερεύνηση δεν λειτουργεί</span><span class="sxs-lookup"><span data-stu-id="17f9a-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="17f9a-p101">Εάν δεν λειτουργεί η **προβολή στην Εξερεύνηση αρχείου** ή **Άνοιγμα με την Εξερεύνηση** βεβαιωθείτε ότι η υπηρεσία WebClient έχει οριστεί να **εκτελεί** , ακολουθώντας τα παρακάτω βήματα. Για παράδειγμα, ίσως χρειαστούν πολύ χρόνο για να ανοίξετε μια βιβλιοθήκη του SharePoint ή OneDrive, όταν δεν εκτελείται η υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="17f9a-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="17f9a-105">Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε εκτέλεση, επιλέξτε το app επιφάνειας εργασίας εκτέλεση, πληκτρολογήστε services.msc και, στη συνέχεια, επιλέξτε **Enter**.</span><span class="sxs-lookup"><span data-stu-id="17f9a-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="17f9a-p102">Κάντε κύλιση έως την υπηρεσία WebClient και ελέγξτε τη στήλη **κατάστασης** . Εάν η κατάσταση της υπηρεσίας WebClient δεν **εκτελείται**, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στο κουμπί **Έναρξη**και στη συνέχεια κάντε κλικ στο κουμπί **OK**. Ενεργοποίηση της υπηρεσίας, εάν χρειάζεται, με την επιλογή **μη αυτόματη** ή **Αυτόματη** στο πλαίσιο **Τύπος εκκίνησης** .</span><span class="sxs-lookup"><span data-stu-id="17f9a-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="17f9a-p103">Για την αντιμετώπιση ζητημάτων ανοίγοντας στην Εξερεύνηση αρχείων, ανατρέξτε στην ενότητα [Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665). Εξερευνήστε συγχρονισμού ως μια καλύτερη εναλλακτική λύση: [αρχεία συγχρονισμού του SharePoint με το πρόγραμμα-πελάτης συγχρονισμού νέα OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="17f9a-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

