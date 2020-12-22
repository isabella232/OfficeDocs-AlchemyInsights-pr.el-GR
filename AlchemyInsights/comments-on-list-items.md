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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724154"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="db349-102">Σχόλια σε στοιχεία λίστας</span><span class="sxs-lookup"><span data-stu-id="db349-102">Comments on List items</span></span>

<span data-ttu-id="db349-103">Οι χρήστες μπορούν να προβάλουν όλα τα σχόλια σε ένα στοιχείο λίστας και να φιλτράρουν μεταξύ προβολών που εμφανίζουν σχόλια ή δραστηριότητες που σχετίζονται με ένα στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="db349-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="db349-104">Οι χρήστες πρέπει να σημειώσουν τα παρακάτω για να προσθέσουν και να διαγράψουν σχόλια:</span><span class="sxs-lookup"><span data-stu-id="db349-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="db349-105">Τα σχόλια ακολουθούν τις εγγενείς ρυθμίσεις δικαιωμάτων στο SharePoint.</span><span class="sxs-lookup"><span data-stu-id="db349-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="db349-106">Οι κλασικές λίστες που δεν έχουν κατασκευαστεί ακόμα για να εμφανίζονται σε σύγχρονα περιβάλλοντα εργασίας χρήστη, όπως οι λίστες εργασιών, δεν θα έχουν αυτήν τη δυνατότητα σχολιασμού.</span><span class="sxs-lookup"><span data-stu-id="db349-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="db349-107">Η προσθήκη σχολίου σε λίστες στο teams δεν είναι διαθέσιμη με αυτή την έκδοση.</span><span class="sxs-lookup"><span data-stu-id="db349-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="db349-108">Τα σχόλια δεν καταχωρούνται με ευρετήριο από την αναζήτηση.</span><span class="sxs-lookup"><span data-stu-id="db349-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="db349-109">Οι διαχειριστές μπορούν να απενεργοποιήσουν αυτήν τη δυνατότητα σε επίπεδο οργανισμού, αλλάζοντας την παράμετρο **CommentsOnListItemsDisabled** στο cmdlet SPOTenant PowerShell του **συνόλου** .</span><span class="sxs-lookup"><span data-stu-id="db349-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="db349-110">Προς το παρόν, δεν είναι δυνατή η απενεργοποίηση του σχολιασμού σε επίπεδο τοποθεσίας ή λίστας.</span><span class="sxs-lookup"><span data-stu-id="db349-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="db349-111">Ελπίζουμε να έχουμε αυτά τα στοιχεία ελέγχου σε μια νεότερη ενημέρωση, πιθανόν κατά το πρώτο τρίμηνο του 2021.</span><span class="sxs-lookup"><span data-stu-id="db349-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
