---
title: Απελευθερώστε χώρο στη μονάδα δίσκου στα Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505356"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="28fff-102">Απελευθερώστε χώρο στη μονάδα δίσκου στα Windows 10</span><span class="sxs-lookup"><span data-stu-id="28fff-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="28fff-103">Ακολουθούν δύο επιλογές για να απελευθερώσετε χώρο στη μονάδα δίσκου στα Windows:</span><span class="sxs-lookup"><span data-stu-id="28fff-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="28fff-104">Απελευθερώστε χώρο στη μονάδα δίσκου στα Windows 10.</span><span class="sxs-lookup"><span data-stu-id="28fff-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="28fff-105">Απελευθερώστε χώρο για ενημερώσεις των Windows 10 με μια εξωτερική συσκευή αποθήκευσης.</span><span class="sxs-lookup"><span data-stu-id="28fff-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="28fff-106">Εάν εξακολουθεί να υπάρχει χαμηλή χωρητικότητα στον δίσκο μετά τη χρήση της Εκκαθάρισης Δίσκου, είναι πιθανό ο φάκελος "Προσωρινά αρχεία" να γεμίζει γρήγορα με αρχεία εφαρμογών (.appx) που χρησιμοποιούνται από το Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="28fff-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="28fff-107">Για να επιδιορθώσετε αυτό το πρόβλημα, πραγματοποιήστε επαναφορά στο Store, εκκαθαρίσετε τη μνήμη cache του Store και, στη συνέχεια, εκτελέστε την Αντιμετώπιση προβλημάτων του Windows Update.</span><span class="sxs-lookup"><span data-stu-id="28fff-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="28fff-108">Βεβαιωθείτε ότι το Microsoft Store είναι κλειστό, προτού συνεχίσετε με αυτά τα βήματα.</span><span class="sxs-lookup"><span data-stu-id="28fff-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="28fff-109">**Βήμα 1: Επαναφορά του Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="28fff-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="28fff-110">**Σημείωση** Με αυτόν τον τρόπο διαγράφονται οριστικά τα δεδομένα της εφαρμογής στη συσκευή, συμπεριλαμβανομένων των προτιμήσεών σας και των λεπτομερειών σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="28fff-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="28fff-111">Επιλέξτε **Έναρξη** > **Ρυθμίσεις** > **Εφαρμογές** > **Εφαρμογές και δυνατότητες**.</span><span class="sxs-lookup"><span data-stu-id="28fff-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="28fff-112">Στη λίστα των εφαρμογών, εντοπίστε και επιλέξτε το Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="28fff-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="28fff-113">Επιλέξτε **Επιλογές για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="28fff-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="28fff-114">Κάντε κύλιση προς τα κάτω, επιλέξτε **Επαναφορά**, και, στη συνέχεια, **Επιβεβαίωση επαναφοράς**.</span><span class="sxs-lookup"><span data-stu-id="28fff-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="28fff-115">**Βήμα 2: Πραγματοποιήστε εκκαθάριση της μνήμης cache του Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="28fff-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="28fff-116">Πατήστε το πλήκτρο με το λογότυπο των Windows + R για να ανοίξετε το παράθυρο διαλόγου "Εκτέλεση".</span><span class="sxs-lookup"><span data-stu-id="28fff-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="28fff-117">Πληκτρολογήστε wsreset.exe και επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="28fff-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="28fff-118">Ανοίγει ένα κενό παράθυρο γραμμής εντολών.</span><span class="sxs-lookup"><span data-stu-id="28fff-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="28fff-119">Μετά από περίπου 10 δευτερόλεπτα, το παράθυρο κλείνει και ανοίγει αυτόματα το Store.</span><span class="sxs-lookup"><span data-stu-id="28fff-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="28fff-120">**Βήμα 3: Επαναφορά του Windows Update**</span><span class="sxs-lookup"><span data-stu-id="28fff-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="28fff-121">Επιλέξτε **Έναρξη** > **Ρυθμίσεις** > **Ενημέρωση και ασφάλεια** > **Αντιμετώπιση προβλημάτων**.</span><span class="sxs-lookup"><span data-stu-id="28fff-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="28fff-122">Κάντε κύλιση προς τα κάτω και επιλέξτε **Windows Update** από τη λίστα και επιλέξτε **Εκτέλεση του προγράμματος αντιμετώπισης προβλημάτων**.</span><span class="sxs-lookup"><span data-stu-id="28fff-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="28fff-123">Επανεκκινήστε τον υπολογιστή σας και ελέγξτε εάν εξακολουθείτε να αντιμετωπίζετε το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="28fff-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

