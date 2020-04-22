---
title: Άνοιγμα με την Εξερεύνηση δεν λειτουργεί
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713034"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="aa8c6-102">Άνοιγμα με την Εξερεύνηση δεν λειτουργεί</span><span class="sxs-lookup"><span data-stu-id="aa8c6-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="aa8c6-103">Εάν **το άνοιγμα με την Εξερεύνηση** ή την Προβολή στην Εξερεύνηση **αρχείων** δεν λειτουργεί, βεβαιωθείτε ότι η υπηρεσία WebClient έχει οριστεί σε **Εκτέλεση** ακολουθώντας τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="aa8c6-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="aa8c6-104">Για παράδειγμα, μπορεί να χρειαστεί πολύς χρόνος για να ανοίξετε μια βιβλιοθήκη του SharePoint ή του OneDrive όταν η υπηρεσία δεν εκτελείται.</span><span class="sxs-lookup"><span data-stu-id="aa8c6-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="aa8c6-105">Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε εκτέλεση, επιλέξτε την εφαρμογή Εκτέλεση επιφάνειας εργασίας, πληκτρολογήστε services.msc και, στη συνέχεια, επιλέξτε **Enter**.</span><span class="sxs-lookup"><span data-stu-id="aa8c6-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="aa8c6-106">Κάντε κύλιση προς τα κάτω στην υπηρεσία WebClient και ελέγξτε τη στήλη **Κατάσταση.**</span><span class="sxs-lookup"><span data-stu-id="aa8c6-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="aa8c6-107">Εάν η κατάσταση της υπηρεσίας WebClient δεν **εκτελείται**, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στην επιλογή **Έναρξη**και, στη συνέχεια, κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa8c6-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="aa8c6-108">Ενεργοποιήστε την υπηρεσία, εάν χρειάζεται, επιλέγοντας **"Μη αυτόματη"** ή **"Αυτόματη"** στο πλαίσιο **Τύπος εκκίνησης.**</span><span class="sxs-lookup"><span data-stu-id="aa8c6-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="aa8c6-109">Για να αντιμετωπίσετε ζητήματα που ανοίγονται στην Εξερεύνηση αρχείων, ανατρέξτε στο θέμα [Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="aa8c6-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="aa8c6-110">Εξερεύνηση συγχρονισμού ως καλύτερης εναλλακτικής λύσης: [Συγχρονισμός αρχείων του SharePoint με το νέο πρόγραμμα-πελάτη συγχρονισμού του OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="aa8c6-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

