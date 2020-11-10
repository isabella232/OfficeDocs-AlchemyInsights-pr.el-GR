---
title: Σχόλια σε στοιχεία λίστας
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982493"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="96c47-102">Σχόλια σε στοιχεία λίστας</span><span class="sxs-lookup"><span data-stu-id="96c47-102">Comments on List items</span></span>

<span data-ttu-id="96c47-103">Οι χρήστες θα μπορούν σύντομα να προσθέσουν και να διαγράψουν σχόλια σε στοιχεία λίστας.</span><span class="sxs-lookup"><span data-stu-id="96c47-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="96c47-104">Οι χρήστες μπορούν να προβάλουν όλα τα σχόλια σε ένα στοιχείο λίστας και να φιλτράρουν μεταξύ προβολών που εμφανίζουν σχόλια ή δραστηριότητες που σχετίζονται με ένα στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="96c47-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="96c47-105">**Χρονισμός** :</span><span class="sxs-lookup"><span data-stu-id="96c47-105">**Timing** :</span></span>

<span data-ttu-id="96c47-106">**Στοχευμένη κυκλοφορία** : σταδιακή ανάπτυξη στα μέσα Οκτωβρίου και αναμένεται να ολοκληρωθεί μέχρι τα μέσα Νοεμβρίου</span><span class="sxs-lookup"><span data-stu-id="96c47-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="96c47-107">**Τυπική κυκλοφορία** : σταδιακή ανάπτυξη στα μέσα Νοεμβρίου και αναμένεται να ολοκληρωθεί στις αρχές Δεκεμβρίου</span><span class="sxs-lookup"><span data-stu-id="96c47-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="96c47-108">**Εγκατάσταση** : στοχευμένη κυκλοφορία για ολόκληρο τον οργανισμό</span><span class="sxs-lookup"><span data-stu-id="96c47-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="96c47-109">Οι χρήστες πρέπει να σημειώσουν τα παρακάτω για να προσθέσουν και να διαγράψουν σχόλια:</span><span class="sxs-lookup"><span data-stu-id="96c47-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="96c47-110">Τα σχόλια ακολουθούν τις εγγενείς ρυθμίσεις δικαιωμάτων στο SharePoint.</span><span class="sxs-lookup"><span data-stu-id="96c47-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="96c47-111">Οι κλασικές λίστες που δεν έχουν κατασκευαστεί ακόμα για να εμφανίζονται σε σύγχρονα περιβάλλοντα εργασίας χρήστη, όπως οι λίστες εργασιών, δεν θα έχουν αυτήν τη δυνατότητα σχολιασμού.</span><span class="sxs-lookup"><span data-stu-id="96c47-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="96c47-112">Η προσθήκη σχολίου σε λίστες στο teams δεν είναι διαθέσιμη με αυτή την έκδοση.</span><span class="sxs-lookup"><span data-stu-id="96c47-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="96c47-113">Τα σχόλια δεν καταχωρούνται με ευρετήριο από την αναζήτηση.</span><span class="sxs-lookup"><span data-stu-id="96c47-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="96c47-114">Οι διαχειριστές μπορούν να απενεργοποιήσουν αυτήν τη δυνατότητα σε επίπεδο οργανισμού, αλλάζοντας την παράμετρο **CommentsOnListItemsDisabled** στο cmdlet SPOTenant PowerShell του **συνόλου** .</span><span class="sxs-lookup"><span data-stu-id="96c47-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="96c47-115">Προς το παρόν, δεν είναι δυνατή η απενεργοποίηση του σχολιασμού σε επίπεδο τοποθεσίας ή λίστας.</span><span class="sxs-lookup"><span data-stu-id="96c47-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="96c47-116">Ελπίζουμε να έχουμε αυτά τα στοιχεία ελέγχου σε μια νεότερη ενημέρωση, πιθανόν κατά το πρώτο τρίμηνο του 2021.</span><span class="sxs-lookup"><span data-stu-id="96c47-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
