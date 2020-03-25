---
title: Επιτάχυνση μετεγκατάστασης του SharePoint με 503 σφάλματα
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931658"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="a94a0-102">Επιτάχυνση μετεγκατάστασης του SharePoint με 503 σφάλματα</span><span class="sxs-lookup"><span data-stu-id="a94a0-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="a94a0-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="a94a0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a94a0-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="a94a0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a94a0-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="a94a0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a94a0-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="a94a0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a94a0-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="a94a0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a94a0-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="a94a0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a94a0-109">**Σφάλματα 503 κατά τη μετεγκατάσταση στο SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="a94a0-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="a94a0-110">Φαίνεται ότι κάνετε μετεγκατάσταση στο SharePoint Online και λαμβάνετε 503 σφάλματα.</span><span class="sxs-lookup"><span data-stu-id="a94a0-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="a94a0-111">Ακολουθήστε τα παρακάτω βήματα, ώστε να σας βοηθήσουμε το συντομότερο δυνατό.</span><span class="sxs-lookup"><span data-stu-id="a94a0-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="a94a0-112">Κάντε κλικ στην επιλογή **Επικοινωνία με την υποστήριξη**και, στη **συνέχεια, νέα αίτηση εξυπηρέτησης**.</span><span class="sxs-lookup"><span data-stu-id="a94a0-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="a94a0-113">Για τον τίτλο και την περιγραφή, πληκτρολογήστε **Επιτάχυνση μετεγκατάστασης του SharePoint με 503**.</span><span class="sxs-lookup"><span data-stu-id="a94a0-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="a94a0-114">Μόλις υποβληθεί το εισιτήριο, παρακαλείστε να το ενημερώσετε με τις ακόλουθες πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="a94a0-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="a94a0-115">Πόσο απομένει από τη μετανάστευση (για παράδειγμα, πόσα TBs;).</span><span class="sxs-lookup"><span data-stu-id="a94a0-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="a94a0-116">Ημερομηνία έναρξης και λήξης της μετεγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="a94a0-116">Migration start and end date.</span></span>
    - <span data-ttu-id="a94a0-117">Περιγράψτε από πού μετεγκαθιστάτε το περιεχόμενό σας, όπως sharePoint Server, Box, GDrive, Κοινόχρηστα στοιχεία αρχείων κ.λπ..</span><span class="sxs-lookup"><span data-stu-id="a94a0-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="a94a0-118">Υπολογίστε τον αριθμό των σφαλμάτων επιτάχυνσης (για παράδειγμα, x γκάζι ανά ώρα;) και πότε συνέβη το στραγγαλισμό.</span><span class="sxs-lookup"><span data-stu-id="a94a0-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="a94a0-119">Ποιο εργαλείο μετεγκατάστασης χρησιμοποιείτε (για παράδειγμα, SPMT ή ShareGate).</span><span class="sxs-lookup"><span data-stu-id="a94a0-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


