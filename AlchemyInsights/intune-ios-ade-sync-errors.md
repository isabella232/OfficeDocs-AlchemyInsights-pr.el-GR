---
title: Σφάλματα συγχρονισμού αυτόματης εγγραφής συσκευών της Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448922"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="f5cde-102">Σφάλματα συγχρονισμού αυτόματης εγγραφής συσκευών της Apple</span><span class="sxs-lookup"><span data-stu-id="f5cde-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="f5cde-103">"Εντοπίσαμε ότι έχετε ένα ή περισσότερα διακριτικά ADE/DEP που βρίσκονται σε κατάσταση σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="f5cde-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="f5cde-104">Μέχρι να επιλυθεί η κατάσταση σφάλματος για κάθε διακριτικό που επηρεάζεται, η λειτουργικότητα ADE δεν θα λειτουργεί όπως αναμένεται.".</span><span class="sxs-lookup"><span data-stu-id="f5cde-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="f5cde-105">Αυτό το σφάλμα ενδέχεται να εμφανιστεί με διάφορους τρόπους, όπως:</span><span class="sxs-lookup"><span data-stu-id="f5cde-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="f5cde-106">Οι συσκευές ενδέχεται να μην συγχρονίζονται από ABM/ASM στο Intune</span><span class="sxs-lookup"><span data-stu-id="f5cde-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="f5cde-107">Οι αναθέσεις προφίλ εγγραφής ενδέχεται να αποτυγχάνουν</span><span class="sxs-lookup"><span data-stu-id="f5cde-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="f5cde-108">Οι συσκευές ενδέχεται να μην ολοκληρώσουν την εγγραφή ADE με επιτυχία</span><span class="sxs-lookup"><span data-stu-id="f5cde-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="f5cde-109">Ελέγξτε για το σφάλμα συγχρονισμού που αναφέρθηκε στην κονσόλα Intune στην περιοχή Συσκευές **> Εγγραφή συσκευών > διακριτικά εγγραφής >** προγράμματος εγγραφής Apple.</span><span class="sxs-lookup"><span data-stu-id="f5cde-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="f5cde-110">Μία από τις πιο συνηθισμένες αιτίες του σφάλματος συγχρονισμού είναι η λήξη του τρέχοντος διακριτικού.</span><span class="sxs-lookup"><span data-stu-id="f5cde-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="f5cde-111">Σε πολλές περιπτώσεις, η ανανέωση του διακριτικού που επηρεάζεται θα επιλύσει το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="f5cde-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="f5cde-112">Εάν ένα ή περισσότερα από τα διακριτικά σας έχουν λήξει, ανατρέξτε στην ακόλουθη τεκμηρίωση που θα σας βοηθήσει να τα ανανεώσετε ανάλογα με την περίπτωση:</span><span class="sxs-lookup"><span data-stu-id="f5cde-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="f5cde-113">Ανανέωση διακριτικού αυτόματης εγγραφής συσκευής</span><span class="sxs-lookup"><span data-stu-id="f5cde-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="f5cde-114">Επιπλέον, μπορείτε να δείτε την ακόλουθη τεκμηρίωση για να δείτε πιθανές αποκατάσταση για άλλα σφάλματα που προκαλούν αποτυχίες συγχρονισμού διακριτικών:</span><span class="sxs-lookup"><span data-stu-id="f5cde-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="f5cde-115">Σφάλματα συγχρονισμού ABM/ASM για διακριτικά εγγραφής αυτοματοποιημένων συσκευών για iOS/iPadOS και macOS</span><span class="sxs-lookup"><span data-stu-id="f5cde-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="f5cde-116">Σφάλματα συγχρονισμού ABM/ASM για διακριτικά εγγραφής αυτοματοποιημένων συσκευών για iOS/iPadOS και macOS</span><span class="sxs-lookup"><span data-stu-id="f5cde-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
