---
title: Αντιμετώπιση προβλημάτων με χρήση του "Άνοιγμα με την Εξερεύνηση"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759692"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="a77d9-102">Επιδιόρθωση προβλημάτων με το Άνοιγμα με την Εξερεύνηση</span><span class="sxs-lookup"><span data-stu-id="a77d9-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="a77d9-103">Επιδιόρθωση συνηθισμένων προβλημάτων με το άνοιγμα μιας βιβλιοθήκης εγγράφων στο SharePoint ή το OneDrive χρησιμοποιώντας την εντολή **"Άνοιγμα με εξερεύνηση":**</span><span class="sxs-lookup"><span data-stu-id="a77d9-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="a77d9-104">Χρησιμοποιήστε τον Internet Explorer 10 ή τον Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="a77d9-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="a77d9-105">**Το άνοιγμα με την Εξερεύνηση** δεν είναι συμβατό με το Microsoft Edge, το Google Chrome, το Firefox και άλλα.</span><span class="sxs-lookup"><span data-stu-id="a77d9-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a77d9-106">**Το άνοιγμα με την Εξερεύνηση** είναι απενεργοποιημένο σε όλα τα προγράμματα περιήγησης εκτός από τον Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a77d9-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="a77d9-107">**Το άνοιγμα με την Εξερεύνηση** δεν είναι διαθέσιμο στη σύγχρονη εμπειρία για βιβλιοθήκες του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a77d9-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="a77d9-108">Χρησιμοποιήστε **την Προβολή στην Εξερεύνηση αρχείων.**</span><span class="sxs-lookup"><span data-stu-id="a77d9-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="a77d9-109">Επιλογή **επιλογών προβολής** \> **Προβολή στην Εξερεύνηση αρχείων**.</span><span class="sxs-lookup"><span data-stu-id="a77d9-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="a77d9-110">Η προβολή στην Εξερεύνηση αρχείων δεν είναι συμβατή με το Microsoft Edge, το Google Chrome, τον Firefox και άλλους.</span><span class="sxs-lookup"><span data-stu-id="a77d9-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a77d9-111">**Προβολή στην Εξερεύνηση αρχείων** που είναι διαθέσιμη μόνο στον Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a77d9-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="a77d9-112">Βεβαιωθείτε ότι εκτελείται η υπηρεσία WebClient.</span><span class="sxs-lookup"><span data-stu-id="a77d9-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="a77d9-113">Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε εκτέλεση, επιλέξτε την εφαρμογή Εκτέλεση επιφάνειας εργασίας, πληκτρολογήστε services.msc και, στη συνέχεια, πατήστε το πλήκτρο Enter.</span><span class="sxs-lookup"><span data-stu-id="a77d9-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="a77d9-114">Κάντε κύλιση προς τα κάτω στην υπηρεσία WebClient και βεβαιωθείτε ότι η στήλη **Κατάσταση** εμφανίζει την ένδειξη "Εκτέλεση".</span><span class="sxs-lookup"><span data-stu-id="a77d9-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="a77d9-115">Εάν δεν το κάνει, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στο κουμπί **Έναρξη**και, στη συνέχεια, κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="a77d9-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="a77d9-116">(Ίσως χρειαστεί να ενεργοποιήσετε πρώτα την υπηρεσία επιλέγοντας **Μη αυτόματη** ή **Αυτόματη** στο πλαίσιο **Τύπος** εκκίνησης.)</span><span class="sxs-lookup"><span data-stu-id="a77d9-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a77d9-117">Το άνοιγμα μιας βιβλιοθήκης στην Εξερεύνηση αρχείων είναι βολικό εάν πρέπει να αντιγράψετε ή να μετακινήσετε πολλά αρχεία και φακέλους μία φορά, αλλά εάν θέλετε να εργάζεστε τακτικά στη βιβλιοθήκη, συνιστούμε να τη συγχρονίσετε.</span><span class="sxs-lookup"><span data-stu-id="a77d9-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="a77d9-118">Για να αντιμετωπίσετε ζητήματα που ανοίγονται στην Εξερεύνηση αρχείων, ανατρέξτε στο θέμα [Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="a77d9-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="a77d9-119">Για πληροφορίες σχετικά με τη ρύθμιση συγχρονισμού, ανατρέξτε στο θέμα [Συγχρονισμός αρχείων του SharePoint με το νέο πρόγραμμα-πελάτη συγχρονισμού του OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a77d9-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="a77d9-120">Ανατρέξτε στο άρθρο [Τρόπος χρήσης της εντολής "Άνοιγμα με την Εξερεύνηση" για την αντιμετώπιση προβλημάτων στο SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="a77d9-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

