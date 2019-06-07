---
title: Επιτάχυνση της ηλεκτρονικής του SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761259"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="eb9b9-102">Επιτάχυνση της ηλεκτρονικής του SharePoint</span><span class="sxs-lookup"><span data-stu-id="eb9b9-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="eb9b9-103">Οι χρήστες ενδέχεται να εμφανιστεί ένα 503 ο διακομιστής είναι απασχολημένος σφάλμα κατά την προσπάθεια για να περιηγηθείτε σε τοποθεσίες του SharePoint ή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eb9b9-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="eb9b9-104">Αυτό το σφάλμα μπορεί να προκληθεί από επιτάχυνσης εντός της υπηρεσίας SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eb9b9-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="eb9b9-105">Ηλεκτρονική SharePoint χρησιμοποιεί επιτάχυνσης για να διατηρείτε βέλτιστες επιδόσεις και την αξιοπιστία της υπηρεσίας SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="eb9b9-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="eb9b9-106">Επιτάχυνση όρια ο αριθμός των ενεργειών χρήστη ή ταυτόχρονες κλήσεις (με δέσμες ενεργειών ή κώδικα) για να αποτρέψετε την υπερβολική χρήση των πόρων.</span><span class="sxs-lookup"><span data-stu-id="eb9b9-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="eb9b9-107">Εάν μπορείτε να επιταχυνθεί, 99% του χρόνου, αυτό οφείλεται σε προσαρμοσμένο κώδικα.</span><span class="sxs-lookup"><span data-stu-id="eb9b9-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="eb9b9-108">Για περισσότερες πληροφορίες σχετικά με την επιτάχυνση [Avoid λήψη επιταχύνει ή να αποκλειστεί με την ηλεκτρονική του SharePoint](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online), ανατρέξτε.</span><span class="sxs-lookup"><span data-stu-id="eb9b9-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="eb9b9-109">Εάν πιστεύετε ότι αυτό το σφάλμα δεν σχετίζεται με την επιτάχυνση, μπορείτε να ελέγξετε αν υπάρχει ενεργό συντήρησης που συμβαίνουν σε σας μίσθωσης, μεταβαίνοντας στο [Κέντρο μηνυμάτων](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="eb9b9-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="eb9b9-110">Τέλος, βεβαιωθείτε ότι επισκέπτεστε τη σελίδα [Εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth) για να ελέγξετε για τυχόν advisories/συμβάντων που ενδέχεται να παρουσιάζεται.</span><span class="sxs-lookup"><span data-stu-id="eb9b9-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

