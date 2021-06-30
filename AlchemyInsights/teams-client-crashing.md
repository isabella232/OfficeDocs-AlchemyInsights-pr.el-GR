---
title: Teams προγράμματος-πελάτη παρουσιάζει σφάλμα
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187721"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="35945-102">Teams προγράμματος-πελάτη παρουσιάζει σφάλμα</span><span class="sxs-lookup"><span data-stu-id="35945-102">Teams client crashing</span></span>

<span data-ttu-id="35945-103">Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="35945-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="35945-104">Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="35945-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="35945-105">Βεβαιωθείτε ότι όλες οι Microsoft 365 διευθύνσεων URL [και οι περιοχές διευθύνσεων](/microsoftteams/connectivity-issues) είναι προσβάσιμες.</span><span class="sxs-lookup"><span data-stu-id="35945-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="35945-106">Συνδεθείτε με το λογαριασμό διαχειριστή μισθωτή και ελέγξτε τον πίνακα εργαλείων της υπηρεσίας [υγείας](/office365/enterprise/view-service-health) για να βεβαιωθείτε ότι δεν υπάρχει καμία υποβάθμιση της υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="35945-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="35945-107">Κατάργηση εγκατάστασης και επανεγκατάσταση της Teams εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="35945-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="35945-108">Μεταβείτε στο φάκελο %appdata%\Microsoft\Teams\ στον υπολογιστή σας και διαγράψτε όλα τα αρχεία σε αυτόν τον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="35945-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="35945-109">[Κάντε λήψη και εγκατάσταση της Teams και,](https://www.microsoft.com/microsoft-teams/download-app)εάν είναι δυνατό, εγκαταστήστε το Teams ως διαχειριστής  (κάντε δεξί κλικ στο πρόγραμμα εγκατάστασης του Teams και επιλέξτε "Εκτέλεση ως διαχειριστής", εάν είναι διαθέσιμο).</span><span class="sxs-lookup"><span data-stu-id="35945-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="35945-110">Εάν το πρόγραμμα Teams εξακολουθεί να παρουσιάζει σφάλμα, προσπαθήστε να αναπαραγάγετε το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="35945-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="35945-111">Εάν μπορείτε να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="35945-111">If you can:</span></span>

1. <span data-ttu-id="35945-112">Χρησιμοποιήστε την Καταγραφή βημάτων για να καταγράψετε τα βήματά σας.</span><span class="sxs-lookup"><span data-stu-id="35945-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="35945-113">Κλείστε ΌΛΕς τις περιττές ή εμπιστευτικές εφαρμογές.</span><span class="sxs-lookup"><span data-stu-id="35945-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="35945-114">Εκκινηθείτε την Καταγραφή βημάτων και αναπαραγάγετε το πρόβλημα ενώ είστε συνδεδεμένοι με το λογαριασμό χρήστη που επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="35945-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="35945-115">[Συλλέξτε τα αρχεία καταγραφής ομάδων που καταγραφούν τα βήματα της καταγεγραμμένης διαδικασίας repro.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="35945-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="35945-116">**Σημείωση:** Βεβαιωθείτε ότι καταγράψετε τη διεύθυνση της είσοδος του χρήστη που έχει επιπτώσεις.</span><span class="sxs-lookup"><span data-stu-id="35945-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="35945-117">Συλλέξτε πληροφορίες κάδου απόρριψης ή/και σφάλματος (Windows).</span><span class="sxs-lookup"><span data-stu-id="35945-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="35945-118">Ξεκινήστε Windows Powershell στον υπολογιστή όπου παρουσιάζεται το σφάλμα και εκτελέστε τις ακόλουθες εντολές (μετά από κάθε εντολή, πατήστε το πλήκτρο Enter):</span><span class="sxs-lookup"><span data-stu-id="35945-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="35945-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="35945-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="35945-120">Αφού δημιουργηθεί το αρχείο κειμένου και εμφανιστεί στην οθόνη σας, αποθηκεύστε το αρχείο και επισυνάψτε το στην αίτηση υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="35945-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
