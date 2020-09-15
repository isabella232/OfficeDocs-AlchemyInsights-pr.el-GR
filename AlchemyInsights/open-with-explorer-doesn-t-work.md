---
title: Το άνοιγμα με την εξερεύνηση δεν λειτουργεί
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694456"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="b8484-102">Το άνοιγμα με την εξερεύνηση δεν λειτουργεί</span><span class="sxs-lookup"><span data-stu-id="b8484-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="b8484-103">Εάν το **Άνοιγμα με την Εξερεύνηση** ή την **προβολή στην Εξερεύνηση αρχείων** δεν λειτουργεί, βεβαιωθείτε ότι η υπηρεσία προγράμματος-πελάτη του προγράμματος-πελάτη έχει τεθεί σε **εκτέλεση** ακολουθώντας τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="b8484-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="b8484-104">Για παράδειγμα, μπορεί να χρειαστεί πολύς χρόνος για να ανοίξετε μια βιβλιοθήκη του SharePoint ή του OneDrive, όταν η υπηρεσία δεν εκτελείται.</span><span class="sxs-lookup"><span data-stu-id="b8484-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="b8484-105">Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε Run, επιλέξτε την εφαρμογή υπολογιστή για εκτέλεση, πληκτρολογήστε Services. msc και, στη συνέχεια, επιλέξτε **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="b8484-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="b8484-106">Κάντε κύλιση προς τα κάτω στην υπηρεσία προγράμματος-πελάτη του προγράμματος-πελάτη και επιλέξτε τη στήλη **κατάσταση** .</span><span class="sxs-lookup"><span data-stu-id="b8484-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="b8484-107">Εάν η κατάσταση της υπηρεσίας προγράμματος-πελάτη του προγράμματος-πελάτη δεν **εκτελείται**, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στην επιλογή **Έναρξη**και, στη συνέχεια, κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="b8484-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="b8484-108">Ενεργοποιήστε την υπηρεσία, εάν είναι απαραίτητο, επιλέγοντας είτε **Χειροκίνητη** είτε **Αυτόματη** στο πλαίσιο **Τύπος εκκίνησης** .</span><span class="sxs-lookup"><span data-stu-id="b8484-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b8484-109">Για να αντιμετωπίσετε προβλήματα κατά το άνοιγμα στην Εξερεύνηση αρχείων, ανατρέξτε [στο θέμα Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="b8484-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="b8484-110">Εξερευνήστε το συγχρονισμό ως καλύτερη εναλλακτική λύση: [Συγχρονίστε τα αρχεία του SharePoint με το νέο πρόγραμμα-πελάτη συγχρονισμού του OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="b8484-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

