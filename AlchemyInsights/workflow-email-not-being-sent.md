---
title: Το μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας δεν αποστέλλεται
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766133"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Το μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας δεν αποστέλλεται για λίστα ή βιβλιοθήκη του SharePoint

1. Το ηλεκτρονικό ταχυδρομείο από ροές εργασίας δεν αποστέλλεται σε όλους τους χρήστες ή μόνο σε συγκεκριμένους χρήστες ή βλέπετε το σφάλμα Δεν είναι δυνατή η αποστολή του **μηνύματος ηλεκτρονικού ταχυδρομείου. Βεβαιωθείτε ότι το μήνυμα ηλεκτρονικού ταχυδρομείου έχει έγκυρο παραλήπτη**.

    Ελέγξτε εάν ο χρήστης υπάρχει στην ομάδα **"Όλα τα άτομα"** (λίστα πληροφοριών χρήστη) για αυτήν τη συλλογή τοποθεσιών.  Δείγμα άμεσης<tenant>διεύθυνσης<sitename>URL: https:// .sharepoint.com/sites/ /_layouts/15/people.aspx; Αναγνωριστικό ομάδας μελών=0

    - Εάν ο χρήστης δεν υπάρχει, βεβαιωθείτε ότι ο χρήστης είναι συνδεδεμένος στη σελίδα. 
    - Εάν πρόκειται για εξωτερικό χρήστη, βεβαιωθείτε ότι η πρόσκλησή του έχει γίνει αποδεκτή.
    - Εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων, βεβαιωθείτε ότι η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σωστή.
    - Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου των χρηστών δεν έχει οριστεί εδώ, δημιουργήστε ένα δείγμα ειδοποίησης για αυτόν το χρήστη, το οποίο επιβάλλει το συγχρονισμό αυτού του λογαριασμού χρήστη από προφίλ χρηστών του SharePoint σε αυτήν τη συλλογή τοποθεσιών.
 
2. Το ηλεκτρονικό ταχυδρομείο από ροές εργασίας αποστέλλεται στους διαχειριστές συλλογής τοποθεσιών, αλλά όχι σε άλλους χρήστες και δείτε το σφάλμα **HTTP Απαγορεύεται να <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Ανατρέξτε [στο θέμα Δεν επιτρέπεται η πρόσβαση όταν στέλνετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Επίσης, βεβαιωθείτε ότι η δυνατότητα συλλογής τοποθεσιών **λειτουργίας κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης** δεν είναι ενεργή.


## <a name="related-topics"></a>Σχετικά θέματα
Θέλετε να δοκιμάσετε το Microsoft Flow στο SharePoint Online;
- [Δημιουργία ροής](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Το SharePoint και η ροή](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


