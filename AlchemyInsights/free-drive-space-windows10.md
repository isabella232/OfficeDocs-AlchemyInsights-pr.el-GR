---
title: Ελευθερώστε χώρο στη μονάδα δίσκου στα Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036585"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="71658-102">Ελευθερώστε χώρο στη μονάδα δίσκου στα Windows 10</span><span class="sxs-lookup"><span data-stu-id="71658-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="71658-103">Ακολουθούν δύο επιλογές για να ελευθερώσετε χώρο στη μονάδα δίσκου στα Windows:</span><span class="sxs-lookup"><span data-stu-id="71658-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="71658-104">Ελευθερώστε χώρο στη μονάδα δίσκου στα Windows 10.</span><span class="sxs-lookup"><span data-stu-id="71658-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="71658-105">Ελευθερώστε χώρο για ενημερώσεις των Windows 10 με εξωτερική συσκευή αποθήκευσης.</span><span class="sxs-lookup"><span data-stu-id="71658-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="71658-106">Εάν εξακολουθείτε να έχετε χαμηλό χώρο στο δίσκο μετά τη χρήση της Εκκαθάρισης Δίσκου, είναι πιθανό ο φάκελος Temp να γεμίζει γρήγορα με αρχεία εφαρμογών (.appx) που χρησιμοποιούνται από το Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="71658-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="71658-107">Για να διορθώσετε αυτό το πρόβλημα, επαναφέρετε το Store, καταργήστε την επιλογή του cache του Store και, στη συνέχεια, εκτελέστε το πρόγραμμα αντιμετώπισης προβλημάτων του Windows Update.</span><span class="sxs-lookup"><span data-stu-id="71658-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="71658-108">Βεβαιωθείτε ότι το Microsoft Store είναι κλειστό πριν να προχωρήσετε σε αυτά τα βήματα.</span><span class="sxs-lookup"><span data-stu-id="71658-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="71658-109">**Βήμα 1: Επαναφορά του Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="71658-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="71658-110">**Σημείωση** Με αυτόν τον τρόπο διαγράφονται οριστικά τα δεδομένα της εφαρμογής στη συσκευή, συμπεριλαμβανομένων των προτιμήσεων και των λεπτομερειών σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="71658-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="71658-111">Επιλέξτε **"Έναρξη**  >    >  **εφαρμογών**  >  **ρυθμίσεων" & δυνατότητες.**</span><span class="sxs-lookup"><span data-stu-id="71658-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="71658-112">Στη λίστα των εφαρμογών, εντοπίστε και επιλέξτε το Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="71658-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="71658-113">Επιλέξτε **"Επιλογές για προχωρημένους".**</span><span class="sxs-lookup"><span data-stu-id="71658-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="71658-114">Κάντε κύλιση προς τα κάτω και **επιλέξτε "Επαναφορά"** και, στη συνέχεια, **"Επιβεβαίωση επαναφοράς".**</span><span class="sxs-lookup"><span data-stu-id="71658-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="71658-115">**Βήμα 2: Απαλοιφή του cache του Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="71658-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="71658-116">Πατήστε το πλήκτρο με το λογότυπο των Windows + R για να ανοίξετε το παράθυρο διαλόγου "Εκτέλεση".</span><span class="sxs-lookup"><span data-stu-id="71658-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="71658-117">Πληκτρολογήστε wsreset.exe και επιλέξτε **OK.**</span><span class="sxs-lookup"><span data-stu-id="71658-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="71658-118">Ανοίγει ένα κενό παράθυρο γραμμής εντολών.</span><span class="sxs-lookup"><span data-stu-id="71658-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="71658-119">Μετά από περίπου 10 δευτερόλεπτα, το παράθυρο κλείνει και το Store ανοίγει αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="71658-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="71658-120">**Βήμα 3: Επαναφορά του Windows Update**</span><span class="sxs-lookup"><span data-stu-id="71658-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="71658-121">Επιλέξτε **"Ενημέρωση**  >  **ρυθμίσεων**  >  **έναρξης" & αντιμετώπιση προβλημάτων**  >  **ασφαλείας.**</span><span class="sxs-lookup"><span data-stu-id="71658-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="71658-122">Κάντε κύλιση προς τα κάτω και **επιλέξτε το Windows Update** από τη λίστα και επιλέξτε **"Εκτέλεση του προγράμματος αντιμετώπισης προβλημάτων".**</span><span class="sxs-lookup"><span data-stu-id="71658-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="71658-123">Επανεκκινήστε τον υπολογιστή σας και ελέγξτε εάν εξακολουθείτε να αντιμετωπίζετε το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="71658-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

