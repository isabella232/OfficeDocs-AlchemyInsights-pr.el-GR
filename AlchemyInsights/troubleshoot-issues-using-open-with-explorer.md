---
title: Αντιμετώπιση προβλημάτων με τη χρήση του ανοίγματος με την Εξερεύνηση
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742733"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="ea0b0-102">Επιδιόρθωση προβλημάτων με το άνοιγμα με την Εξερεύνηση</span><span class="sxs-lookup"><span data-stu-id="ea0b0-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="ea0b0-103">Διορθώστε συνηθισμένα προβλήματα με το άνοιγμα μιας βιβλιοθήκης εγγράφων στο SharePoint ή στο OneDrive χρησιμοποιώντας την εντολή " **Άνοιγμα με την Εξερεύνηση** ":</span><span class="sxs-lookup"><span data-stu-id="ea0b0-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="ea0b0-104">Χρησιμοποιήστε τον Internet Explorer 10 ή 11 του Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="ea0b0-105">**Άνοιγμα με Explorer** δεν είναι συμβατό με το Microsoft Edge, το Google Chrome, το Firefox και άλλα.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="ea0b0-106">Το **Άνοιγμα με την Εξερεύνηση** είναι απενεργοποιημένο σε όλα τα προγράμματα περιήγησης εκτός από τον Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="ea0b0-107">**Άνοιγμα με την Εξερεύνηση** δεν είναι διαθέσιμη στη σύγχρονη εμπειρία για βιβλιοθήκες του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="ea0b0-108">Εναλλακτικά, χρησιμοποιήστε **την προβολή στην Εξερεύνηση αρχείων** .</span><span class="sxs-lookup"><span data-stu-id="ea0b0-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="ea0b0-109">Επιλέξτε Προβολή **επιλογών** \> προβολής **στην Εξερεύνηση αρχείων**.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="ea0b0-110">Η προβολή στην Εξερεύνηση αρχείων δεν είναι συμβατή με το Microsoft Edge, το Google Chrome, το Firefox και άλλα.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="ea0b0-111">**Προβολή στην Εξερεύνηση αρχείων** στο διαθέσιμο μόνο στον Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="ea0b0-112">Βεβαιωθείτε ότι η υπηρεσία WebClient εκτελείται.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="ea0b0-113">Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε Run, επιλέξτε το Εκτέλεση εφαρμογής επιφάνειας εργασίας, πληκτρολογήστε Services. msc και, στη συνέχεια, πιέστε το πλήκτρο ENTER.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="ea0b0-114">Μετακινηθείτε προς τα κάτω στην υπηρεσία WebClient και βεβαιωθείτε ότι η στήλη κατάστασης εμφανίζει την **ένδειξη** "εκτέλεση".</span><span class="sxs-lookup"><span data-stu-id="ea0b0-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="ea0b0-115">Εάν δεν το κάνει, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στο κουμπί **Έναρξη**και, στη συνέχεια, κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="ea0b0-116">(Ίσως χρειαστεί να ενεργοποιήσετε πρώτα την υπηρεσία, επιλέγοντας είτε **Χειροκίνητη** είτε **Αυτόματη** στο πλαίσιο **Τύπος εκκίνησης** .)</span><span class="sxs-lookup"><span data-stu-id="ea0b0-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="ea0b0-117">Το άνοιγμα μιας βιβλιοθήκης στην Εξερεύνηση αρχείων είναι βολικό αν χρειάζεται να αντιγράψετε ή να μετακινήσετε πολλά αρχεία και φακέλους μία φορά, αλλά αν θέλετε να εργάζεστε τακτικά στη βιβλιοθήκη, συνιστούμε να το συγχρονίσετε.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="ea0b0-118">Για να αντιμετωπίσετε ζητήματα που ανοίγουν στην Εξερεύνηση αρχείων, ανατρέξτε [στο θέμα Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="ea0b0-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="ea0b0-119">Για πληροφορίες σχετικά με τη ρύθμιση του συγχρονισμού, ανατρέξτε [στο θέμα Συγχρονισμός αρχείων του SharePoint με το νέο πρόγραμμα-πελάτη συγχρονισμού OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="ea0b0-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="ea0b0-120">Ανατρέξτε στο άρθρο [Πώς να χρησιμοποιήσετε την εντολή "Άνοιγμα με την Εξερεύνηση" για να αντιμετωπίσετε ζητήματα στο SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="ea0b0-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

