---
title: Το απόθεμα λογισμικού λείπει ή δεν είναι ακριβές
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676265"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="680db-102">Το απόθεμα λογισμικού λείπει ή δεν είναι ακριβές</span><span class="sxs-lookup"><span data-stu-id="680db-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="680db-103">Το απόθεμα λογισμικού στο Διαχείριση απειλών και ευπαθειών (TVM) είναι μια λίστα γνωστού λογισμικού στον οργανισμό σας με επίσημες κοινές απαριθμήσεις πλατφόρμας (CPE).</span><span class="sxs-lookup"><span data-stu-id="680db-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="680db-104">Τα προϊόντα λογισμικού χωρίς επίσημο CPE δεν έχουν δημοσιευμένα θέματα ευπάθειας.</span><span class="sxs-lookup"><span data-stu-id="680db-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="680db-105">Το απόθεμα περιλαμβάνει επίσης λεπτομέρειες όπως το όνομα του προμηθευτή, τον αριθμό των αδυναμιών, τις απειλές και τον αριθμό των συσκευών που εκτίθενται.</span><span class="sxs-lookup"><span data-stu-id="680db-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="680db-106">Οι αλλαγές λογισμικού σε συσκευές αντικατοπτρίζονται συνήθως στις πύλες ασφαλείας εντός δύο ωρών.</span><span class="sxs-lookup"><span data-stu-id="680db-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="680db-107">Ωστόσο, μερικές φορές μπορεί να διαρκέσει περισσότερο.</span><span class="sxs-lookup"><span data-stu-id="680db-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="680db-108">Προς το παρόν, δεν υπάρχει τρόπος επιβολής συγχρονισμού. αυτή είναι μια συνεχής αξιολόγηση.</span><span class="sxs-lookup"><span data-stu-id="680db-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="680db-109">Εάν κάνατε μια αλλαγή λογισμικού και η αλλαγή δεν αντικατοπτρίζεται με ακρίβεια στο TVM μετά από 5 ώρες, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="680db-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="680db-110">Ελέγξτε την ενότητα αποδεικτικών στοιχείων λογισμικού για να κατανοήσετε τον τρόπο με τον οποίο εντοπίστηκε το λογισμικό.</span><span class="sxs-lookup"><span data-stu-id="680db-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="680db-111">Βεβαιωθείτε ότι το λογισμικό υποστηρίζεται.</span><span class="sxs-lookup"><span data-stu-id="680db-111">Make sure that the software is supported.</span></span> <span data-ttu-id="680db-112">Το λογισμικό μπορεί να είναι ορατό μόνο σε επίπεδο συσκευής, ακόμα και αν προς το παρόν δεν υποστηρίζεται από Διαχείριση απειλών και ευπαθειών.</span><span class="sxs-lookup"><span data-stu-id="680db-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="680db-113">Ωστόσο, μόνο περιορισμένα δεδομένα είναι διαθέσιμα.</span><span class="sxs-lookup"><span data-stu-id="680db-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="680db-114">Για τα βήματα για την αναφορά της ανακρίβειας από την πύλη, ανατρέξτε στο [θέμα Αναφορά ανακρίβειας.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="680db-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="680db-115">**Σημείωση:** Η αναφορά ανακρίβειας από την πύλη MDE είναι ένα κανάλι μίας διαδρομής προς τη μηχανική.</span><span class="sxs-lookup"><span data-stu-id="680db-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="680db-116">Εάν το πρόβλημα είναι επείγον, ανοίξτε ένα δελτίο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="680db-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="680db-117">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Απόθεμα λογισμικού - Διαχείριση απειλών και ευπαθειών.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="680db-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>