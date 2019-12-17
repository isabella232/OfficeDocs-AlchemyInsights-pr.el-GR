---
title: Αντιμετώπιση ζητημάτων "Άνοιγμα με την Εξερεύνηση" στο SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 21a0c193b752342d47189dda73d171249153f7fc
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050813"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="5a81b-102">Αντιμετώπιση ζητημάτων "Άνοιγμα με την Εξερεύνηση" στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5a81b-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="5a81b-103">Η εντολή "Άνοιγμα με την Εξερεύνηση" ανοίγει μια τοπική περίοδο λειτουργίας της Εξερεύνησης των Windows η οποία εμφανίζει τη δομή φακέλων στον διακομιστή που φιλοξενεί την τοποθεσία SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5a81b-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="5a81b-104">Ως εκ τούτου, συνιστάται [να συγχρονίζετε τα αρχεία του SharePoint με το νέο πρόγραμμα-πελάτη συγχρονισμού OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), </a>το οποίο παρέχει [αρχεία κατ ' απαίτηση,](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) επειδή παρέχει τοπική πρόσβαση στα αρχεία σας και προσφέρει βέλτιστη απόδοση.</span><span class="sxs-lookup"><span data-stu-id="5a81b-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="5a81b-105">Εάν επιλέξατε να χρησιμοποιήσετε την προβολή Εξερεύνησης των Windows αντί να χρησιμοποιήσετε το νέο πρόγραμμα-πελάτη συγχρονισμού OneDrive, βεβαιωθείτε ότι ακολουθείτε τα βήματα και τις βέλτιστες πρακτικές που περιγράφονται στα παρακάτω άρθρα:</span><span class="sxs-lookup"><span data-stu-id="5a81b-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="5a81b-106">Πώς μπορείτε να χρησιμοποιήσετε την εντολή "Άνοιγμα με την Εξερεύνηση" για την αντιμετώπιση προβλημάτων στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5a81b-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="5a81b-107">Αντιγραφή ή μετακίνηση αρχείων βιβλιοθήκης με χρήση της εντολής "Άνοιγμα με την Εξερεύνηση"</span><span class="sxs-lookup"><span data-stu-id="5a81b-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="5a81b-108">Το κουμπί **"Άνοιγμα με την Εξερεύνηση"** δεν εμφανίζεται στην εμπειρία νέας βιβλιοθήκης.</span><span class="sxs-lookup"><span data-stu-id="5a81b-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="5a81b-109">Κάντε κλικ στο αναπτυσσόμενο μενού **"Προβολή"** στην επάνω δεξιά γωνία (η ονομασία του αναπτυσσόμενου μενού αλλάζει ανάλογα με την τρέχουσα προβολή) και, στη συνέχεια, κάντε κλικ στην επιλογή **"Προβολή στην Εξερεύνηση αρχείων"**.</span><span class="sxs-lookup"><span data-stu-id="5a81b-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="5a81b-110">Η εντολή "Άνοιγμα με την Εξερεύνηση" του SharePoint χρησιμοποιεί στοιχεία ελέγχου ActiveX, επομένως υποστηρίζεται μόνο από τον Internet Explorer 10 ή 11.</span><span class="sxs-lookup"><span data-stu-id="5a81b-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="5a81b-111">Το "Άνοιγμα με την Εξερεύνηση" δεν λειτουργεί στα Windows με Microsoft Edge, Google Chrome, Mozilla Firefox ή στην πλατφόρμα Mac.</span><span class="sxs-lookup"><span data-stu-id="5a81b-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="5a81b-112">Για τον λόγο αυτό, η επιλογή "Προβολή Εξερεύνησης των Windows" μπορεί να είναι απενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="5a81b-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="5a81b-113">[Γιατί τα κουμπιά της κορδέλας του SharePoint είναι μη διαθέσιμα ή απενεργοποιημένα](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="5a81b-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

