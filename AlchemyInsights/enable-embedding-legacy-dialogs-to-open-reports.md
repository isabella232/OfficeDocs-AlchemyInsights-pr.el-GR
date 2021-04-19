---
title: Ενεργοποίηση των παραθύρων διαλόγου ενσωμάτωσης παλαιού τύπου για το άνοιγμα αναφορών
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814264"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="90d97-102">Ενεργοποίηση των παραθύρων διαλόγου ενσωμάτωσης παλαιού τύπου για το άνοιγμα αναφορών</span><span class="sxs-lookup"><span data-stu-id="90d97-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="90d97-103">**Σύμπτωμα**</span><span class="sxs-lookup"><span data-stu-id="90d97-103">**Symptom**</span></span>

<span data-ttu-id="90d97-104">Οι χρήστες δεν μπορούν να ανοίξουν αναφορές.</span><span class="sxs-lookup"><span data-stu-id="90d97-104">Users are unable to open reports.</span></span> <span data-ttu-id="90d97-105">"Κάτι δεν πήγε καλά.</span><span class="sxs-lookup"><span data-stu-id="90d97-105">"Something has gone wrong.</span></span> <span data-ttu-id="90d97-106">Ελέγξτε τις τεχνικές λεπτομέρειες για περισσότερες λεπτομέρειες".</span><span class="sxs-lookup"><span data-stu-id="90d97-106">Check technical details for more details."</span></span>

<span data-ttu-id="90d97-107">**Αιτία**</span><span class="sxs-lookup"><span data-stu-id="90d97-107">**Cause**</span></span>

<span data-ttu-id="90d97-108">Οι αναφορές δεν φορτώνονται στο UCI με το σφάλμα "Η περιγραφή φόρμας είναι null ή δεν έχει οριστεί".</span><span class="sxs-lookup"><span data-stu-id="90d97-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="90d97-109">Οι αναφορές στο UCI εξακολουθούν να απαιτούν παράθυρα διαλόγου παλαιού τύπου, επομένως το σύστημα του πελάτη πρέπει να έχει ενεργοποιημένη τη *δυνατότητα allowlegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="90d97-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="90d97-110">**Λύση**</span><span class="sxs-lookup"><span data-stu-id="90d97-110">**Solution**</span></span>

1. <span data-ttu-id="90d97-111">Μεταβείτε **στην καρτέλα ">", > "Ρυθμίσεις συστήματος" > καρτέλα "Γενικά".**</span><span class="sxs-lookup"><span data-stu-id="90d97-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="90d97-112">Ορίστε την επιλογή "Ενεργοποίηση ενσωμάτωσης ορισμένων παραθύρων διαλόγου παλαιού τύπου στο πρόγραμμα-πελάτη προγράμματος-πελάτη ενοποιημένου περιβάλλοντος εργασίας" **σε "Ναι".**</span><span class="sxs-lookup"><span data-stu-id="90d97-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
