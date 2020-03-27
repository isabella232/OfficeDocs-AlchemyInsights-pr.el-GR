---
title: Επιδόσεις μετεγκατάστασης SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932248"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="57f72-102">Επιδόσεις μετεγκατάστασης SharePoint</span><span class="sxs-lookup"><span data-stu-id="57f72-102">SharePoint migration performance</span></span>

<span data-ttu-id="57f72-103">**Σημαντικό**: Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν σημαντικές επιχειρηματικές εφαρμογές με την υπηρεσία να εκτελείται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="57f72-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="57f72-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="57f72-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="57f72-105">Σε αυτούς τους πρωτόγνωρους καιρούς, λαμβάνουμε μέτρα για να εξασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες και αξιόπιστες στον ύψιστο βαθμό για τους χρήστες σας, οι οποίοι εξαρτώνται από την υπηρεσία περισσότερο από ποτέ για απομακρυσμένες εργασίες.</span><span class="sxs-lookup"><span data-stu-id="57f72-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="57f72-106">Για αυτόν τον στόχο, εφαρμόσαμε αυστηρότερα όρια περιορισμού σε εφαρμογές παρασκηνίου (μετεγκατάσταση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τη διάρκεια των πρωινών ωρών των εργάσιμων ημερών.</span><span class="sxs-lookup"><span data-stu-id="57f72-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="57f72-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη απόδοση κατά τη διάρκεια αυτών των ωρών.</span><span class="sxs-lookup"><span data-stu-id="57f72-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="57f72-108">Ωστόσο, κατά τις βραδινές ώρες της περιοχής σας και τα σαββατοκύριακα, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά μεγαλύτερο όγκο αιτήσεων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="57f72-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="57f72-109">**Επιδόσεις μετεγκατάστασης**</span><span class="sxs-lookup"><span data-stu-id="57f72-109">**Migration performance**</span></span>

<span data-ttu-id="57f72-110">Οι επιδόσεις της μετεγκατάστασης μπορούν να επηρεαστούν από την υποδομή του δικτύου, το μέγεθος αρχείου, το χρόνο μετεγκατάστασης και τις επιβραδύνσεις.</span><span class="sxs-lookup"><span data-stu-id="57f72-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="57f72-111">Η κατανόηση αυτής της διαδικασίας θα σας βοηθήσει να σχεδιάσετε και να μεγιστοποιήσετε την απόδοση της μετεγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="57f72-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="57f72-112">Για περισσότερες πληροφορίες, επισκεφθείτε τις συνδέσεις παρακάτω.</span><span class="sxs-lookup"><span data-stu-id="57f72-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="57f72-113">Sharepoint Online και ταχύτητα μετεγκατάστασης ODB</span><span class="sxs-lookup"><span data-stu-id="57f72-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="57f72-114">Αποφυγή επιβράδυνσης ή αποκλεισμού στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="57f72-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="57f72-115">Λήψη και εγκατάσταση του εργαλείου μετεγκατάστασης του SharePoint</span><span class="sxs-lookup"><span data-stu-id="57f72-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
