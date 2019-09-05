---
title: Ηλεκτρονική επιτάχυνση του SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751888"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="c7220-102">Ηλεκτρονική επιτάχυνση του SharePoint</span><span class="sxs-lookup"><span data-stu-id="c7220-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="c7220-103">Οι χρήστες ενδέχεται να λάβετε ένα διακομιστή 503 είναι κατειλημμένο σφάλμα κατά την προσπάθεια περιήγησης σε τοποθεσίες του SharePoint ή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c7220-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="c7220-104">Αυτό το σφάλμα μπορεί να προκληθεί από επιτάχυνση εντός της υπηρεσίας SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c7220-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c7220-105">Ηλεκτρονική SharePoint χρησιμοποιεί επιτάχυνσης για να διατηρήσετε τη βέλτιστη απόδοση και την αξιοπιστία της υπηρεσίας SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c7220-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c7220-106">Ο περιορισμός περιορίζει τον αριθμό των ενεργειών χρήστη ή των ταυτόχρονων κλήσεων (με δέσμη ενεργειών ή κώδικα) για την αποτροπή της υπερβολικής χρήσης πόρων.</span><span class="sxs-lookup"><span data-stu-id="c7220-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c7220-107">Εάν έχετε επιβραδύνει, 99% του χρόνου που οφείλεται σε προσαρμοσμένο κώδικα.</span><span class="sxs-lookup"><span data-stu-id="c7220-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="c7220-108">Για περισσότερες πληροφορίες σχετικά με την επιτάχυνση δείτε, [Αποφύγετε να έχετε επιβραδύνει ή να αποκλειστεί στο SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c7220-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="c7220-109">Εάν πιστεύετε ότι αυτό το σφάλμα δεν σχετίζεται με τον περιορισμό, μπορείτε να ελέγξετε αν υπάρχει ενεργή συντήρηση που συμβαίνει στον μισθωτή σας, μεταβαίνοντας στο [Κέντρο μηνυμάτων](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="c7220-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="c7220-110">Τέλος, βεβαιωθείτε ότι επισκέπτεστε τη σελίδα [Health Service](https://portal.office.com/adminportal/home#/servicehealth) για να ελέγξετε για τυχόν προειδοποιήσεις/συμβάντα που ενδέχεται να συμβούν.</span><span class="sxs-lookup"><span data-stu-id="c7220-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

