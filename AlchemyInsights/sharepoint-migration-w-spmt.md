---
title: Μετεγκατάσταση του SharePoint με SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931550"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="2277b-102">Μετεγκατάσταση του SharePoint με SPMT</span><span class="sxs-lookup"><span data-stu-id="2277b-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="2277b-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="2277b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2277b-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="2277b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2277b-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="2277b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2277b-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="2277b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2277b-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="2277b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2277b-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="2277b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2277b-109">**Εργαλείο μετεγκατάστασης του SharePoint**</span><span class="sxs-lookup"><span data-stu-id="2277b-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="2277b-110">Σχεδιασμένο για χρήση για μετεγκαταστάσεις που κυμαίνονται από το μικρότερο σύνολο αρχείων έως μια μεγάλης κλίμακας εταιρική μετεγκατάσταση, το Εργαλείο μετεγκατάστασης του SharePoint θα σας επιτρέψει να μεταφέρετε τις πληροφορίες σας στο cloud και να επωφεληθείτε από την πιο πρόσφατη συνεργασία, ευφυΐα και λύσεις ασφαλείας με το Office 365.</span><span class="sxs-lookup"><span data-stu-id="2277b-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="2277b-111">Λήψη και εγκατάσταση του εργαλείου μετεγκατάστασης του SharePoint</span><span class="sxs-lookup"><span data-stu-id="2277b-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="2277b-112">Αντιμετώπιση συνηθισμένων προβλημάτων και σφαλμάτων SPMT</span><span class="sxs-lookup"><span data-stu-id="2277b-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="2277b-113">Αντιμετώπιση προβλημάτων εγκατάστασης SPMT</span><span class="sxs-lookup"><span data-stu-id="2277b-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
