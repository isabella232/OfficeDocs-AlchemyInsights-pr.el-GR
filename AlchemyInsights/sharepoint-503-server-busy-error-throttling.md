---
title: Επιτάχυνση του SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773847"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="48f14-102">Επιτάχυνση του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="48f14-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="48f14-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="48f14-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="48f14-104">**σφάλμα "ο διακομιστής 503 είναι απασχολημένος"**</span><span class="sxs-lookup"><span data-stu-id="48f14-104">**503 server is busy error**</span></span>

<span data-ttu-id="48f14-105">Οι χρήστες ενδέχεται να λάβουν έναν διακομιστή του 503 που είναι απασχολημένος κατά την προσπάθεια περιήγησης σε τοποθεσίες του SharePoint ή του OneDrive.</span><span class="sxs-lookup"><span data-stu-id="48f14-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="48f14-106">Αυτό το σφάλμα μπορεί να προκληθεί από τον περιορισμό εντός της υπηρεσίας SharePoint.</span><span class="sxs-lookup"><span data-stu-id="48f14-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="48f14-107">Το SharePoint Online χρησιμοποιεί την επιβράδυνση για να διατηρήσει τις βέλτιστες επιδόσεις και την αξιοπιστία της υπηρεσίας SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="48f14-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="48f14-108">Η επιβράδυνση περιορίζει τον αριθμό των ενεργειών χρήστη ή των ταυτόχρονων κλήσεων (κατά δέσμες ενεργειών ή κώδικα) για την αποτροπή της υπερβολικής χρήσης πόρων.</span><span class="sxs-lookup"><span data-stu-id="48f14-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="48f14-109">Για περισσότερες πληροφορίες σχετικά με τον περιορισμό, ανατρέξτε [στο θέμα αποφυγή περιορισμού ή αποκλεισμού στο SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="48f14-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="48f14-110">Εάν πιστεύετε ότι αυτό το σφάλμα δεν σχετίζεται με τον περιορισμό, μπορείτε να επιλέξετε εάν υπάρχει ενεργή συντήρηση που εμφανίζεται στον μισθωτή σας, μεταβαίνοντας στο [Κέντρο μηνυμάτων](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="48f14-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="48f14-111">Τέλος, βεβαιωθείτε ότι επισκέπτεστε τη σελίδα [εύρυθμης λειτουργίας υπηρεσιών](https://portal.office.com/adminportal/home#/servicehealth) για να δείτε τυχόν συμβουλές/συμβάντα που μπορεί να προκύψουν.</span><span class="sxs-lookup"><span data-stu-id="48f14-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

