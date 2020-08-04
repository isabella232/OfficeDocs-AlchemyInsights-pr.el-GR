---
title: Παύση προγραμματισμένων ενημερώσεων
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555106"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="7570d-102">Παύση προγραμματισμένων ενημερώσεων</span><span class="sxs-lookup"><span data-stu-id="7570d-102">Pausing scheduled updates</span></span>

<span data-ttu-id="7570d-103">Όταν εκδίδεται μια εντολή παύσης, οι συσκευές δεν επεξεργάζονται την εντολή μέχρι την επόμενη φορά που θα κάνουν μεταβίβαση ελέγχου στο Intune.</span><span class="sxs-lookup"><span data-stu-id="7570d-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="7570d-104">Για το λόγο αυτό, οι συσκευές σας ενδέχεται να έχουν:</span><span class="sxs-lookup"><span data-stu-id="7570d-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="7570d-105">Εγκαταστήσατε τις προγραμματισμένες ενημερώσεις πριν από το check-in.</span><span class="sxs-lookup"><span data-stu-id="7570d-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="7570d-106">Έχει απενεργοποιηθεί όταν εκδώσατε την εντολή παύσης.</span><span class="sxs-lookup"><span data-stu-id="7570d-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="7570d-107">Σε αυτήν την περίπτωση, όταν οι συσκευές ήταν ενεργοποιημένες, ενδέχεται να έχουν κάνει λήψη και εγκατάσταση των προγραμματισμένων ενημερώσεων πριν από το check-in.</span><span class="sxs-lookup"><span data-stu-id="7570d-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>