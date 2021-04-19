---
title: Σφάλματα στο πρόγραμμα-πελάτη Teams;
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826271"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="541d7-102">Σφάλματα στο πρόγραμμα-πελάτη Teams;</span><span class="sxs-lookup"><span data-stu-id="541d7-102">Teams client crashing?</span></span>

<span data-ttu-id="541d7-103">Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="541d7-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="541d7-104">Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="541d7-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="541d7-105">Βεβαιωθείτε ότι όλες οι διευθύνσεις URL και οι περιοχές διευθύνσεων του [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) είναι προσβάσιμες.</span><span class="sxs-lookup"><span data-stu-id="541d7-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="541d7-106">Συνδεθείτε με το λογαριασμό διαχειριστή μισθωτή και ελέγξτε τον πίνακα εργαλείων της υπηρεσίας [υγείας](https://docs.microsoft.com/office365/enterprise/view-service-health) για να βεβαιωθείτε ότι δεν υπάρχει καμία υποβάθμιση της υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="541d7-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="541d7-107">Κατάργηση εγκατάστασης και επανεγκατάσταση της εφαρμογής Teams (σύνδεση)</span><span class="sxs-lookup"><span data-stu-id="541d7-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="541d7-108">Μεταβείτε στο φάκελο %appdata%\Microsoft\teams\ στον υπολογιστή σας και διαγράψτε όλα τα αρχεία σε αυτόν τον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="541d7-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="541d7-109">[Κάντε λήψη και εγκατάσταση της εφαρμογής Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)και, εάν είναι δυνατό, εγκαταστήστε το Teams ως διαχειριστή (κάντε δεξί κλικ στο πρόγραμμα εγκατάστασης του Teams και επιλέξτε "Εκτέλεση ως διαχειριστής", εάν είναι διαθέσιμο).</span><span class="sxs-lookup"><span data-stu-id="541d7-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="541d7-110">Εάν το πρόγραμμα-πελάτης του Teams εξακολουθεί να παρουσιάζει σφάλμα, μπορείτε να αναπαραγάγετε το πρόβλημα;</span><span class="sxs-lookup"><span data-stu-id="541d7-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="541d7-111">Εάν ναι:</span><span class="sxs-lookup"><span data-stu-id="541d7-111">If so:</span></span>

1. <span data-ttu-id="541d7-112">Χρησιμοποιήστε την Καταγραφή βημάτων για να καταγράψετε τα βήματά σας.</span><span class="sxs-lookup"><span data-stu-id="541d7-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="541d7-113">Κλείστε ΌΛΕς τις περιττές ή εμπιστευτικές εφαρμογές.</span><span class="sxs-lookup"><span data-stu-id="541d7-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="541d7-114">Εκκινηθείτε την Καταγραφή βημάτων και αναπαραγάγετε το πρόβλημα ενώ είστε συνδεδεμένοι με το λογαριασμό χρήστη που επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="541d7-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="541d7-115">[Συλλέξτε τα αρχεία καταγραφής ομάδων που καταγραφούν τα βήματα της καταγεγραμμένης διαδικασίας repro.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="541d7-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="541d7-116">**Σημείωση:** Βεβαιωθείτε ότι καταγράψετε τη διεύθυνση της είσοδος του χρήστη που έχει επιπτώσεις.</span><span class="sxs-lookup"><span data-stu-id="541d7-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="541d7-117">Συλλέξτε πληροφορίες κάδου απόρριψης ή/και σφάλματος (Windows).</span><span class="sxs-lookup"><span data-stu-id="541d7-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="541d7-118">Εκκινήστε το Windows Powershell στον υπολογιστή όπου παρουσιάζεται το σφάλμα και εκτελέστε τις ακόλουθες εντολές:</span><span class="sxs-lookup"><span data-stu-id="541d7-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="541d7-119">Επισυνάψτε το αρχείο στην υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="541d7-119">Attach the file to your support case.</span></span>
