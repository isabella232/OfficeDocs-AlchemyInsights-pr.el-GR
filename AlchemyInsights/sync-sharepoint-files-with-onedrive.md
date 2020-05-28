---
title: Αντιμετώπιση ζητημάτων "Άνοιγμα με την Εξερεύνηση" στο SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: be1136f7fd4575d482d38ee70163e5252d4ffbca
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343194"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="7cbbb-102">Αντιμετώπιση ζητημάτων "Άνοιγμα με την Εξερεύνηση" στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7cbbb-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="7cbbb-103">Συνιστάται [να συγχρονίζετε τα αρχεία του SharePoint με το νέο πρόγραμμα-πελάτη συγχρονισμού OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), το οποίο παρέχει [αρχεία κατ ' απαίτηση](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), επειδή παρέχει τοπική πρόσβαση στα αρχεία σας και προσφέρει βέλτιστη απόδοση.</span><span class="sxs-lookup"><span data-stu-id="7cbbb-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="7cbbb-104">Για την αντιμετώπιση προβλημάτων με το "Άνοιγμα με την Εξερεύνηση", ακολουθήστε τα βήματα και τις βέλτιστες πρακτικές που περιγράφονται στα ακόλουθα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="7cbbb-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="7cbbb-105">Πώς μπορείτε να χρησιμοποιήσετε την εντολή "Άνοιγμα με την Εξερεύνηση" για την αντιμετώπιση προβλημάτων στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7cbbb-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="7cbbb-106">Αντιγραφή ή μετακίνηση αρχείων βιβλιοθήκης με χρήση της εντολής "Άνοιγμα με την Εξερεύνηση"</span><span class="sxs-lookup"><span data-stu-id="7cbbb-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="7cbbb-107">**Σημείωση:**</span><span class="sxs-lookup"><span data-stu-id="7cbbb-107">**Note:**</span></span>
>- <span data-ttu-id="7cbbb-108">Το "Άνοιγμα με την Εξερεύνηση" υποστηρίζεται μόνο στον Internet Explorer 10 ή 11.</span><span class="sxs-lookup"><span data-stu-id="7cbbb-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="7cbbb-109">Το "Άνοιγμα με την Εξερεύνηση" δεν λειτουργεί στα Windows με Microsoft Edge, Google Chrome, Mozilla Firefox ή στην πλατφόρμα Mac.</span><span class="sxs-lookup"><span data-stu-id="7cbbb-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="7cbbb-110">Για τον λόγο αυτό, η επιλογή "Προβολή Εξερεύνησης των Windows" μπορεί να είναι απενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="7cbbb-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="7cbbb-111">Το κουμπί "Άνοιγμα με την Εξερεύνηση" δεν εμφανίζεται στην εμπειρία νέας βιβλιοθήκης.</span><span class="sxs-lookup"><span data-stu-id="7cbbb-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="7cbbb-112">Κάντε κλικ στο αναπτυσσόμενο μενού **"Προβολή"** στην επάνω δεξιά γωνία (η ονομασία του αναπτυσσόμενου μενού αλλάζει ανάλογα με την τρέχουσα προβολή) και, στη συνέχεια, κάντε κλικ στην επιλογή **"Προβολή στην Εξερεύνηση αρχείων"**.</span><span class="sxs-lookup"><span data-stu-id="7cbbb-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
