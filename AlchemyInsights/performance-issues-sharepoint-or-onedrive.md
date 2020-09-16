---
title: Προβλήματα επιδόσεων-SharePoint ή OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771901"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a8ae5-102">Το SharePoint ή το OneDrive είναι αργά, απρόσιτα ή μη διαθέσιμα για πολλούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="a8ae5-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="a8ae5-103">Το SharePoint ή το OneDrive μπορεί να είναι αργά, απρόσιτα ή μη διαθέσιμα ή μπορεί να εμφανίζουν σφάλματα υπηρεσίας ή σφάλματα του 503, για διάφορους λόγους:</span><span class="sxs-lookup"><span data-stu-id="a8ae5-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="a8ae5-104">Εάν η τοποθεσία σας στο SharePoint ή στο OneDrive είναι αργή ή καθυστερεί για πολλούς χρήστες, μπορεί να υπάρχει ένα πρόβλημα προσωρινής υπηρεσίας όπου οι χρήστες αντιμετωπίζουν περιοδικές καθυστερήσεις ή σφάλματα περιήγησης κατά την πρόσβαση σε τοποθεσίες του SharePoint ή σε περιεχόμενο του OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a8ae5-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="a8ae5-105">Επιλέξτε τον [πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) για να δείτε εάν ο οργανισμός σας επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="a8ae5-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="a8ae5-106">Οι χρήστες ενδέχεται να λάβουν έναν *διακομιστή του 503 που είναι απασχολημένος* κατά την προσπάθεια περιήγησης σε τοποθεσίες του SharePoint ή του OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a8ae5-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="a8ae5-107">Αυτό το σφάλμα μπορεί να προκληθεί από τον περιορισμό εντός της υπηρεσίας SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a8ae5-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="a8ae5-108">Το SharePoint Online χρησιμοποιεί την επιβράδυνση για να διατηρήσει τις βέλτιστες επιδόσεις και την αξιοπιστία της υπηρεσίας SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="a8ae5-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a8ae5-109">Η επιβράδυνση περιορίζει τον αριθμό των ενεργειών χρήστη ή των ταυτόχρονων κλήσεων (κατά δέσμες ενεργειών ή κώδικα) για την αποτροπή της υπερβολικής χρήσης πόρων.</span><span class="sxs-lookup"><span data-stu-id="a8ae5-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="a8ae5-110">Για περισσότερες πληροφορίες σχετικά με τον περιορισμό, ανατρέξτε [στο θέμα αποφυγή περιορισμού ή αποκλεισμού στο SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="a8ae5-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="a8ae5-111">Εάν αντιμετωπίζετε αργές επιδόσεις με μια **κλασική** ή **σύγχρονη** τοποθεσία ή σελίδα του SharePoint, χρησιμοποιήστε το [εργαλείο διάγνωσης σελίδας](https://aka.ms/perftool) για να αναλύσετε τις σελίδες.</span><span class="sxs-lookup"><span data-stu-id="a8ae5-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="a8ae5-112">Εάν εξακολουθείτε να αντιμετωπίζετε γενικές αργές επιδόσεις, ελέγξτε τους πόρους στο κάτω μέρος αυτού του άρθρου: [Εισαγωγή στη ρύθμιση επιδόσεων για το SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="a8ae5-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  