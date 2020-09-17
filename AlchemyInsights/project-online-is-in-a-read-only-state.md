---
title: Το Project Online βρίσκεται σε κατάσταση μόνο για ανάγνωση
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801652"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="5005c-102">Το Project Online βρίσκεται σε κατάσταση μόνο για ανάγνωση</span><span class="sxs-lookup"><span data-stu-id="5005c-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="5005c-103">Υπάρχουν τρεις κοινοί λόγοι για τους οποίους το Project Online μπορεί να φτάσει σε κατάσταση μόνο για ανάγνωση:</span><span class="sxs-lookup"><span data-stu-id="5005c-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="5005c-104">Οι εταιρείες έχουν μόνο μια άδεια χρήσης του Project Online Essentials.</span><span class="sxs-lookup"><span data-stu-id="5005c-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="5005c-105">Αυτό δεν επαρκεί για να διατηρήσει την τοποθεσία ζωντανή και τελικά θα αποδοθεί από την προμήθεια.</span><span class="sxs-lookup"><span data-stu-id="5005c-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="5005c-106">Τοποθετούμε την τοποθεσία σε κατάσταση μόνο για ανάγνωση, ώστε οι διαχειριστές να γνωρίζουν ότι κάτι δεν πάει καλά και να μπορούν να αποκτήσουν τις σωστές άδειες χρήσης.</span><span class="sxs-lookup"><span data-stu-id="5005c-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="5005c-107">Οι διαχειριστές θα πρέπει να προσθέσουν μια άδεια χρήσης του Project Online Professional ή/και Premium.</span><span class="sxs-lookup"><span data-stu-id="5005c-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="5005c-108">Η τοποθεσία θα εξέλθει από μόνο για ανάγνωση σε αυτό το σημείο.</span><span class="sxs-lookup"><span data-stu-id="5005c-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="5005c-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Σύγκριση λύσεων διαχείρισης έργων](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="5005c-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="5005c-110">Έχει συμπληρωθεί το όριο που έχει εκχωρηθεί.</span><span class="sxs-lookup"><span data-stu-id="5005c-110">Assigned quota has been reached.</span></span> <span data-ttu-id="5005c-111">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα όριο μεγέθους του Project Web App](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="5005c-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="5005c-112">Επιλέξτε [Ρύθμιση παραμέτρων των δεδομένων αναφοράς χρονολογικής φάσης στο Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) για να δείτε τον τρόπο με τον οποίο η λεπτομερής αναφορά μπορεί να επηρεάσει τη χρήση των ορίων.</span><span class="sxs-lookup"><span data-stu-id="5005c-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="5005c-113">Μόνο για ανάγνωση μπορεί να είναι μια πολύ προσωρινή συνθήκη που μπορεί να προκύψει κατά τη συντήρηση.</span><span class="sxs-lookup"><span data-stu-id="5005c-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="5005c-114">Οι περισσότερες συντηρήσεις δεν παρατηρούνται καν από τους πελάτες μας και δεν θα βλέπετε συχνά αυτό το θέμα, αλλά υπάρχουν φορές που οι σύντομες περίοδοι μόνο για ανάγνωση είναι έμπειρες.</span><span class="sxs-lookup"><span data-stu-id="5005c-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
