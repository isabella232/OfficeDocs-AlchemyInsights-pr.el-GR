---
title: Αντιμετώπιση προβλημάτων και σφαλμάτων του εργαλείου μετεγκατάστασης του SharePoint
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931118"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="b31f1-102">Αντιμετώπιση προβλημάτων και σφαλμάτων του εργαλείου μετεγκατάστασης του SharePoint</span><span class="sxs-lookup"><span data-stu-id="b31f1-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="b31f1-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="b31f1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b31f1-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="b31f1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b31f1-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="b31f1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b31f1-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="b31f1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b31f1-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="b31f1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b31f1-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="b31f1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b31f1-109">**Συνήθη ζητήματα και σφάλματα**</span><span class="sxs-lookup"><span data-stu-id="b31f1-109">**Common issues and errors**</span></span>

<span data-ttu-id="b31f1-110">Ενδέχεται να αντιμετωπίσετε ορισμένα συνηθισμένα ζητήματα και σφάλματα κατά τη χρήση του Εργαλείου μετεγκατάστασης του SharePoint (SPMT).</span><span class="sxs-lookup"><span data-stu-id="b31f1-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="b31f1-111">Ανατρέξτε στους παρακάτω συνδέσμους για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="b31f1-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="b31f1-112">Αντιμετώπιση συνηθισμένων προβλημάτων και σφαλμάτων SPMT</span><span class="sxs-lookup"><span data-stu-id="b31f1-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="b31f1-113">Αντιμετώπιση προβλημάτων εγκατάστασης SPMT</span><span class="sxs-lookup"><span data-stu-id="b31f1-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)