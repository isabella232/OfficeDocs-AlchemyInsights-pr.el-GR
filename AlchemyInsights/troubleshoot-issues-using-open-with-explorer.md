---
title: Αντιμετώπιση προβλημάτων με το άνοιγμα με την Εξερεύνηση
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 5be8a8f9f67939c7e2671855da259818269d9299
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291183"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="6e88c-102">Επιδιόρθωση προβλημάτων με το άνοιγμα με την Εξερεύνηση</span><span class="sxs-lookup"><span data-stu-id="6e88c-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="6e88c-103">Διορθώστε συνήθη προβλήματα με το άνοιγμα μιας βιβλιοθήκης εγγράφων του SharePoint ή OneDrive, χρησιμοποιώντας την εντολή **Άνοιγμα με την Εξερεύνηση** :</span><span class="sxs-lookup"><span data-stu-id="6e88c-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="6e88c-p101">Χρησιμοποιείτε Internet Explorer 10 ή 11 του Internet Explorer. **Άνοιγμα με την Εξερεύνηση** δεν είναι συμβατό με το Microsoft άκρη, Google Chrome, Firefox και άλλα. **Άνοιγμα με την Εξερεύνηση** είναι απενεργοποιημένη σε όλα τα προγράμματα περιήγησης εκτός από τον Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6e88c-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="6e88c-p102">**Άνοιγμα με την Εξερεύνηση** δεν είναι διαθέσιμη σε μια σύγχρονη εμπειρία για βιβλιοθήκες του SharePoint. Χρησιμοποιήστε την **προβολή στην Εξερεύνηση** . Επιλέξτε **Επιλογές προβολής** \> **προβολή στην Εξερεύνηση**. Προβολή στην Εξερεύνηση του αρχείου δεν είναι συμβατό με το Microsoft άκρη, Google Chrome, Firefox και άλλα. **Προβολή στην Εξερεύνηση αρχείου** στη διαθέσιμη μόνο στον Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6e88c-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="6e88c-p103">Βεβαιωθείτε ότι εκτελείται η υπηρεσία WebClient. Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε εκτέλεση, επιλέξτε το app επιφάνειας εργασίας εκτέλεση, πληκτρολογήστε services.msc και, στη συνέχεια, πιέστε το πλήκτρο Enter. Κάντε κύλιση έως την υπηρεσία WebClient και βεβαιωθείτε ότι η στήλη **κατάστασης** εμφανίζει "Εκτέλεση". Εάν όχι, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στο κουμπί **Έναρξη**και στη συνέχεια κάντε κλικ στο κουμπί **OK**. (Ίσως χρειαστεί να ενεργοποιήσετε πρώτα την υπηρεσία επιλέγοντας **Χειροκίνητη** ή **Αυτόματη** στο πλαίσιο **Τύπος εκκίνησης** ).</span><span class="sxs-lookup"><span data-stu-id="6e88c-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="6e88c-p104">Ανοίγοντας μια βιβλιοθήκη στην Εξερεύνηση αρχείου είναι χρήσιμο εάν θέλετε να αντιγράψετε ή να μετακινήσετε πολλά αρχεία και φακέλους από τη στιγμή, αλλά αν θέλετε να έχετε συνηθίσει να εργάζεστε στη βιβλιοθήκη, συνιστάται να συγχρονίσετε. Για την αντιμετώπιση ζητημάτων ανοίγοντας στην Εξερεύνηση αρχείων, ανατρέξτε στην ενότητα [Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665). Για πληροφορίες σχετικά με τη ρύθμιση του συγχρονισμού, δείτε [αρχεία συγχρονισμού του SharePoint με το πρόγραμμα-πελάτης συγχρονισμού νέα OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="6e88c-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="6e88c-120">Ανατρέξτε στο άρθρο [Τρόπος χρήσης της εντολής "Άνοιγμα με Εξερεύνησης" για την αντιμετώπιση προβλημάτων με την ηλεκτρονική του SharePoint](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="6e88c-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

