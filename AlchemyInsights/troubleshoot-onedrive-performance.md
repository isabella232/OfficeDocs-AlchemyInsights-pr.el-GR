---
title: Αντιμετώπιση προβλημάτων απόδοσης του OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757885"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="a20c9-102">Αντιμετώπιση προβλημάτων απόδοσης του OneDrive</span><span class="sxs-lookup"><span data-stu-id="a20c9-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="a20c9-103">Εάν αντιμετωπίζετε έναν βραδύτερο από τον αναμενόμενο συγχρονισμό ή παρόμοια προβλήματα επιδόσεων με το OneDrive:</span><span class="sxs-lookup"><span data-stu-id="a20c9-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="a20c9-104">Επιβεβαιώστε ότι δεν υπάρχουν γνωστά προβλήματα με τη χρήση του [πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a20c9-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="a20c9-105">[Ενεργοποιήστε αρχεία](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) κατ ' απαίτηση, ώστε να μπορείτε να έχετε πρόσβαση σε όλα τα αρχεία σας στο OneDrive χωρίς να χρειάζεται να κάνετε λήψη όλων των αρχείων και να χρησιμοποιήσετε χώρο αποθήκευσης στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="a20c9-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="a20c9-106">[Εξετάστε τις βέλτιστες πρακτικές](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) για το σχεδιασμό και την απόδοση δικτύου.</span><span class="sxs-lookup"><span data-stu-id="a20c9-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="a20c9-107">[Μεγιστοποιήστε την ταχύτητα αποστολής και λήψης](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), ειδικά εάν συγχρονίζετε μια συσκευή για πρώτη φορά.</span><span class="sxs-lookup"><span data-stu-id="a20c9-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="a20c9-108">Εάν συγχρονίζετε μια βιβλιοθήκη με περισσότερα από 100.000 στοιχεία, ο συγχρονισμός του OneDrive μπορεί να φαίνεται ότι έχει κολλήσει για μεγάλο χρονικό διάστημα ή η κατάσταση εμφανίζει την επεξεργασία 0KB του xMB. "</span><span class="sxs-lookup"><span data-stu-id="a20c9-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="a20c9-109">[Μάθετε περισσότερα σχετικά με το συγχρονισμό περισσότερων από 100.000 αρχείων](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , καθώς και [το όριο υποστηριζόμενων αρχείων 300.000 του OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="a20c9-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="a20c9-110">Όταν ένας χρήστης υπερβεί τα όρια χρήσης, το SharePoint Online ρυθμίζει τυχόν περαιτέρω αιτήσεις από αυτόν τον λογαριασμό χρήστη για ένα σύντομο χρονικό διάστημα.</span><span class="sxs-lookup"><span data-stu-id="a20c9-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="a20c9-111">Όλες οι ενέργειες χρήστη επιταχύνονται ενώ το γκάζι είναι σε ισχύ.</span><span class="sxs-lookup"><span data-stu-id="a20c9-111">All user actions are throttled while the throttle is in effect.</span></span>
