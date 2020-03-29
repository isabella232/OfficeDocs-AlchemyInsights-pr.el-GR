---
title: Σφάλματα στο πρόγραμμα-πελάτη Teams;
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030583"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="ef9b8-102">Σφάλματα στο πρόγραμμα-πελάτη Teams;</span><span class="sxs-lookup"><span data-stu-id="ef9b8-102">Teams client crashing?</span></span>

<span data-ttu-id="ef9b8-103">Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="ef9b8-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="ef9b8-104">Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="ef9b8-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="ef9b8-105">Βεβαιωθείτε ότι έχετε πρόσβαση σε όλες τις [περιοχές διευθύνσεων URL και διευθύνσεις του Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues).</span><span class="sxs-lookup"><span data-stu-id="ef9b8-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="ef9b8-106">Συνδεθείτε με τον λογαριασμό διαχειριστή σας και ελέγξτε τον [Πίνακα ελέγχου εύρυθμης λειτουργίας υπηρεσιών](https://docs.microsoft.com/office365/enterprise/view-service-health) για να επαληθεύσετε ότι δεν υπάρχει διακοπή λειτουργίας ή υποβάθμιση υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="ef9b8-107">Ως τελευταίο βήμα, μπορείτε να επιχειρήσετε την εκκαθάριση της μνήμης cache του προγράμματος-πελάτη Teams:</span><span class="sxs-lookup"><span data-stu-id="ef9b8-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="ef9b8-108">Τερματίστε πλήρως το πρόγραμμα-πελάτη υπολογιστή Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="ef9b8-109">Μπορείτε να κάνετε δεξί κλικ στο **Teams** από τον δίσκο εικονιδίων και να κάνετε κλικ στην επιλογή **Κλείσιμο** ή να εκτελέσετε τη Διαχείριση εργασιών και να σταματήσετε πλήρως τη διαδικασία.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="ef9b8-110">Μεταβείτε στην Εξερεύνηση αρχείων και πληκτρολογήστε "%appdata%\Microsoft\teams".</span><span class="sxs-lookup"><span data-stu-id="ef9b8-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="ef9b8-111">Αφού βρεθείτε στον κατάλογο, θα δείτε μερικούς από τους ακόλουθους φακέλους:</span><span class="sxs-lookup"><span data-stu-id="ef9b8-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="ef9b8-112">Μέσα από το **Μνήμη cache εφαρμογών**, μεταβείτε στη Μνήμη cache και διαγράψτε οποιοδήποτε από τα αρχεία στη θέση cache: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="ef9b8-113">Μέσα από το **Blob_storage**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="ef9b8-114">Μέσα από τη **Μνήμη cache**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="ef9b8-115">Μέσα από τις **βάσεις δεδομένων**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="ef9b8-116">Μέσα από τη **Μνήμη GPUcache**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="ef9b8-117">Μέσα από το **IndexedDB**, διαγράψτε το αρχείο .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="ef9b8-118">Μέσα από τον **Τοπικό χώρο αποθήκευσης**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="ef9b8-119">Τέλος, μέσα από το **tmp**, διαγράψτε οποιοδήποτε αρχείο: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="ef9b8-120">Επανεκκινήστε το πρόγραμμα-πελάτη Teams.</span><span class="sxs-lookup"><span data-stu-id="ef9b8-120">Restart your Teams client.</span></span>
