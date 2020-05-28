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
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354052"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="daefc-102">Σφάλματα στο πρόγραμμα-πελάτη Teams;</span><span class="sxs-lookup"><span data-stu-id="daefc-102">Teams client crashing?</span></span>

<span data-ttu-id="daefc-103">Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="daefc-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="daefc-104">Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="daefc-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="daefc-105">Βεβαιωθείτε ότι είναι προσβάσιμες όλες οι [διευθύνσεις URL και οι περιοχές διευθύνσεων του Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)</span><span class="sxs-lookup"><span data-stu-id="daefc-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="daefc-106">Συνδεθείτε με το λογαριασμό διαχειριστή μισθωτή και ελέγξτε [τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://docs.microsoft.com/office365/enterprise/view-service-health) για να βεβαιωθείτε ότι δεν υπάρχει διακοπή ρεύματος ή υποβάθμιση της υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="daefc-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="daefc-107">Κατάργηση εγκατάστασης και επανεγκατάσταση της εφαρμογής teams (link)</span><span class="sxs-lookup"><span data-stu-id="daefc-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="daefc-108">Μεταβείτε στο φάκελο %appdata%\Microsoft\teams\ στον υπολογιστή σας και διαγράψτε όλα τα αρχεία σε αυτόν τον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="daefc-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="daefc-109">[Κατεβάστε και εγκαταστήστε την εφαρμογή Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)και, εάν είναι δυνατόν, εγκαταστήστε το Teams ως διαχειριστή (κάντε δεξί κλικ στο πρόγραμμα εγκατάστασης ομάδων και επιλέξτε "Εκτέλεση ως διαχειριστής" εάν είναι διαθέσιμο).</span><span class="sxs-lookup"><span data-stu-id="daefc-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="daefc-110">Εάν το πρόγραμμα-πελάτης του Teams εξακολουθεί να είναι σε αιφνίδια διακοπή λειτουργίας, μπορείτε να αναπαραγάγετε το ζήτημα;</span><span class="sxs-lookup"><span data-stu-id="daefc-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="daefc-111">Αν ναι:</span><span class="sxs-lookup"><span data-stu-id="daefc-111">If so:</span></span>

1. <span data-ttu-id="daefc-112">Χρησιμοποιήστε την Καταγραφή βημάτων για να καταγράψετε τα βήματά σας.</span><span class="sxs-lookup"><span data-stu-id="daefc-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="daefc-113">Κλείστε όλες τις περιττές ή εμπιστευτικές εφαρμογές.</span><span class="sxs-lookup"><span data-stu-id="daefc-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="daefc-114">Εκκινήστε την Καταγραφή βημάτων και αναπαράγνατε το ζήτημα ενώ είστε συνδεδεμένοι με το λογαριασμό χρήστη που επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="daefc-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="daefc-115">[Συλλέξτε τα αρχεία καταγραφής ομάδων που αποτυπώνουν τα καταγεγραμμένα βήματα αναπαραγωγής](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="daefc-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="daefc-116">**Σημείωση**: Βεβαιωθείτε ότι καταγράφετε τη διεύθυνση εισόδου του χρήστη που επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="daefc-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="daefc-117">Συλλέξτε τις πληροφορίες κάδο χωματερή ς ή/και βλαβών (Windows).</span><span class="sxs-lookup"><span data-stu-id="daefc-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="daefc-118">Εκκίνηση του Windows Powershell στον υπολογιστή όπου παρουσιάζεται η αιφνίδια διακοπή λειτουργίας και εκτελέστε τις ακόλουθες εντολές:</span><span class="sxs-lookup"><span data-stu-id="daefc-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="daefc-119">Επισυνάψτε το αρχείο στην υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="daefc-119">Attach the file to your support case.</span></span>
