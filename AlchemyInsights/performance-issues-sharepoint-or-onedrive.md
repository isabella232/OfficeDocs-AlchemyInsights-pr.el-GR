---
title: Ζητήματα επιδόσεων-SharePoint ή OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068402"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="05166-102">Το SharePoint ή το OneDrive αργή, απρόσιτη ή μη διαθέσιμη για πολλούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="05166-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="05166-103">Το SharePoint ή το OneDrive ενδέχεται να είναι αργή, απρόσιτη ή μη διαθέσιμη ή μπορεί να εμφανίσει μη διαθέσιμα ή 503 σφάλματα υπηρεσίας, για διάφορους λόγους:</span><span class="sxs-lookup"><span data-stu-id="05166-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="05166-104">Εάν η τοποθεσία του SharePoint ή του OneDrive είναι αργή ή καθυστερεί για πολλούς χρήστες, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας όπου οι χρήστες αντιμετωπίζουν διακοπτόμενες καθυστερήσεις ή σφάλματα περιήγησης κατά την πρόσβαση σε τοποθεσίες του SharePoint ή περιεχόμενο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="05166-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="05166-105">Ελέγξτε τον [πίνακα εργαλείων εύρυθμης λειτουργίας της υπηρεσίας](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , για να δείτε αν επηρεάζεται ο οργανισμός σας.</span><span class="sxs-lookup"><span data-stu-id="05166-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="05166-106">Οι χρήστες ενδέχεται να λάβετε ένα *503 διακομιστή είναι απασχολημένος* σφάλμα κατά την προσπάθεια περιήγησης σε τοποθεσίες του SharePoint ή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="05166-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="05166-107">Αυτό το σφάλμα μπορεί να προκληθεί από επιτάχυνση εντός της υπηρεσίας SharePoint.</span><span class="sxs-lookup"><span data-stu-id="05166-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="05166-108">Ηλεκτρονική SharePoint χρησιμοποιεί επιτάχυνσης για να διατηρήσετε τη βέλτιστη απόδοση και την αξιοπιστία της υπηρεσίας SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="05166-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="05166-109">Ο περιορισμός περιορίζει τον αριθμό των ενεργειών χρήστη ή των ταυτόχρονων κλήσεων (με δέσμη ενεργειών ή κώδικα) για την αποτροπή της υπερβολικής χρήσης πόρων.</span><span class="sxs-lookup"><span data-stu-id="05166-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="05166-110">Για περισσότερες πληροφορίες σχετικά με την επιτάχυνση δείτε, [Αποφύγετε να έχετε επιβραδύνει ή να αποκλειστεί στο SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="05166-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="05166-111">Εάν αντιμετωπίζετε χαμηλές επιδόσεις με μια **κλασική** ή **σύγχρονη** τοποθεσία ή σελίδα του SharePoint, χρησιμοποιήστε το [διαγνωστικό εργαλείο σελίδας](https://aka.ms/perftool) για να αναλύσετε τις σελίδες.</span><span class="sxs-lookup"><span data-stu-id="05166-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="05166-112">Εάν εξακολουθείτε να αντιμετωπίζετε γενικές χαμηλές επιδόσεις, ελέγξτε τους πόρους στο κάτω μέρος αυτού του άρθρου: [Εισαγωγή στο συντονισμό επιδόσεων για το SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="05166-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  