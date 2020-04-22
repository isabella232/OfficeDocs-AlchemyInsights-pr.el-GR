---
title: Το Project Online βρίσκεται σε κατάσταση μόνο για ανάγνωση
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: dea4e24b0ceb0054f04e6737df0feb761d1143f3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768005"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="1c3d8-102">Το Project Online βρίσκεται σε κατάσταση μόνο για ανάγνωση</span><span class="sxs-lookup"><span data-stu-id="1c3d8-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="1c3d8-103">Υπάρχουν τρεις συνήθεις λόγοι για τους οποίους το Project Online μπορεί να φτάσει σε κατάσταση μόνο για ανάγνωση:</span><span class="sxs-lookup"><span data-stu-id="1c3d8-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="1c3d8-104">Οι οργανισμοί έχουν μια άδεια χρήσης για ηλεκτρονικά είδη πρώτης ανάγκης έργου μόνο.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="1c3d8-105">Αυτό δεν είναι αρκετό για να κρατήσει το site ζωντανό και τελικά θα πάρει de-provisioned.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="1c3d8-106">Τοποθετούμε την τοποθεσία σε κατάσταση μόνο για ανάγνωση, ώστε οι διαχειριστές να γνωρίζουν ότι κάτι δεν πάει καλά και να μπορούν να αποκτήσουν τις σωστές άδειες χρήσης.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="1c3d8-107">Οι διαχειριστές θα πρέπει να προσθέσουν μια άδεια χρήσης του Project Online Professional ή/και premium.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="1c3d8-108">Η ιστοσελίδα θα βγει από μόνο για ανάγνωση σε εκείνο το σημείο.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="1c3d8-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Σύγκριση λύσεων διαχείρισης έργων](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="1c3d8-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="1c3d8-110">Έχει επιτευχθεί εκχωρημένο όριο.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-110">Assigned quota has been reached.</span></span> <span data-ttu-id="1c3d8-111">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Όριο εφαρμογής του Project Web App](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="1c3d8-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="1c3d8-112">Επιλέξτε [Ρύθμιση παραμέτρων συνάθροισης δεδομένων αναφοράς χρονολογικής φάσης στο Project Online,](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) για να δείτε πώς η υποδιαίρεση αναφορών μπορεί να επηρεάσει τη χρήση ορίου δίσκου.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="1c3d8-113">Μόνο για ανάγνωση μπορεί να είναι μια πολύ προσωρινή κατάσταση που μπορεί να προκύψει κατά τη διάρκεια της συντήρησης.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="1c3d8-114">Οι περισσότεροι συντήρηση δεν είναι καν παρατηρήσει από τους πελάτες μας και δεν θα δείτε συχνά αυτό, αλλά υπάρχουν φορές που οι σύντομες περιόδους μόνο για ανάγνωση είναι έμπειροι.</span><span class="sxs-lookup"><span data-stu-id="1c3d8-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
