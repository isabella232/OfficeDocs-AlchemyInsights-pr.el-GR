---
title: Επιτάχυνση του SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931442"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5a151-102">Επιτάχυνση του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5a151-102">SharePoint Online throttling</span></span>

<span data-ttu-id="5a151-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="5a151-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5a151-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="5a151-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5a151-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="5a151-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5a151-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="5a151-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5a151-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="5a151-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5a151-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="5a151-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5a151-109">**Επιτάχυνση του SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="5a151-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="5a151-110">Το SharePoint Online χρησιμοποιεί επιτάχυνση για να διατηρήσει τη βέλτιστη απόδοση και αξιοπιστία της υπηρεσίας SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="5a151-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5a151-111">Ο περιορισμός περιορίζει τον αριθμό των ενεργειών χρήστη ή των ταυτόχρονων κλήσεων (ανά δέσμη ενεργειών ή κώδικα) για να αποτραπεί η υπερβολική χρήση πόρων.</span><span class="sxs-lookup"><span data-stu-id="5a151-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5a151-112">Για περισσότερες πληροφορίες, παρακαλούμε επισκεφθείτε τους παρακάτω συνδέσμους.</span><span class="sxs-lookup"><span data-stu-id="5a151-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="5a151-113">Αποφύγετε την επιτάχυνση ή τον αποκλεισμό στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5a151-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="5a151-114">Μετεγκατάσταση δεδομένων και επιτάχυνση SPO</span><span class="sxs-lookup"><span data-stu-id="5a151-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="5a151-115">Ταχύτητα μετεγκατάστασης του SharePoint Online και του OneDrive</span><span class="sxs-lookup"><span data-stu-id="5a151-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="5a151-116">Χειρισμός του sharepoint online στραγγαλισμού χρησιμοποιώντας εκθετική απενεργοποίηση</span><span class="sxs-lookup"><span data-stu-id="5a151-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="5a151-117">Σχεδιασμός δυναμικότητας και δοκιμή φόρτωσης του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5a151-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

