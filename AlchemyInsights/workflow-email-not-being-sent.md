---
title: Το μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας δεν αποστέλλεται
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748989"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Το μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας δεν αποστέλλεται για μια λίστα ή βιβλιοθήκη του SharePoint

1. Το ηλεκτρονικό ταχυδρομείο από τις ροές εργασίας δεν αποστέλλεται σε όλους τους χρήστες ή μόνο σε συγκεκριμένους χρήστες ή εμφανίζεται το σφάλμα **δεν είναι δυνατή η αποστολή του μηνύματος ηλεκτρονικού ταχυδρομείου. Βεβαιωθείτε ότι το ηλεκτρονικό ταχυδρομείο έχει έναν έγκυρο παραλήπτη**.

    Βεβαιωθείτε ότι ο χρήστης υπάρχει στην ομάδα δικαιώματα " **όλα τα άτομα** " (λίστα πληροφοριών χρήστη) για τη συγκεκριμένη συλλογή τοποθεσιών.  Δείγμα απευθείας διεύθυνσης URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx; MembershipGroupId = 0

    - Εάν ο χρήστης δεν υπάρχει, βεβαιωθείτε ότι ο χρήστης έχει εισέλθει στη σελίδα. 
    - Εάν πρόκειται για εξωτερικό χρήστη, βεβαιωθείτε ότι η πρόσκλησή του έχει γίνει δεκτή.
    - Εάν ο χρήστης υπάρχει στην ομάδα "δικαιώματα", βεβαιωθείτε ότι η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σωστή.
    - Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου των χρηστών δεν έχει καθοριστεί εδώ, δημιουργήστε ένα δείγμα ειδοποίησης για αυτόν το χρήστη, το οποίο επιβάλλει τον συγχρονισμό αυτού του λογαριασμού χρήστη από τα προφίλ χρηστών του SharePoint σε αυτήν τη συλλογή τοποθεσιών.
 
2. Τα μηνύματα ηλεκτρονικού ταχυδρομείου από τις ροές εργασίας αποστέλλονται στους διαχειριστές της συλλογής τοποθεσιών, αλλά όχι σε άλλους χρήστες και βλέπουν το σφάλμα **http απαγορευμένο στο <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.
 

    Ανατρέξτε [στο θέμα δεν επιτρέπεται η πρόσβαση όταν στέλνετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Επίσης, βεβαιωθείτε ότι η δυνατότητα " **λειτουργία κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης** " δεν είναι ενεργή.


## <a name="related-topics"></a>Σχετικά θέματα
Θέλετε να δοκιμάσετε το Microsoft Flow στο SharePoint Online;
- [Δημιουργία ροής](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint και Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


