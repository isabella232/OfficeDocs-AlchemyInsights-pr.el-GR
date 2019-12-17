---
title: Το μήνυμα ηλεκτρονικού ταχυδρομείου της ροής εργασίας δεν αποστέλλεται
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049373"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Δεν αποστέλλεται μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας για μια λίστα ή βιβλιοθήκη του SharePoint

1. Τα μηνύματα ηλεκτρονικού ταχυδρομείου από ροές εργασίας δεν αποστέλλονται σε όλους τους χρήστες ή μόνο σε συγκεκριμένους χρήστες ή μπορείτε να δείτε το σφάλμα **δεν είναι δυνατή η αποστολή του μηνύματος ηλεκτρονικού ταχυδρομείου. Βεβαιωθείτε ότι το μήνυμα ηλεκτρονικού ταχυδρομείου έχει έγκυρο παραλήπτη**.

    Ελέγξτε εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων **όλων των ατόμων** (λίστα πληροφοριών χρήστη) για αυτήν τη συλλογή τοποθεσιών.  Δείγμα άμεσης διεύθυνσης URL:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/Loot.MCA; Κράτος μέλους = 0

    - Εάν ο χρήστης δεν υπάρχει, βεβαιωθείτε ότι ο χρήστης είναι συνδεδεμένος στη σελίδα. 
    - Εάν πρόκειται για εξωτερικό χρήστη, βεβαιωθείτε ότι η πρόσκλησή τους έχει γίνει δεκτή.
    - Εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων, βεβαιωθείτε ότι η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σωστή.
    - Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου των χρηστών δεν έχει οριστεί εδώ, τότε Δημιουργήστε ένα δείγμα ειδοποίησης για αυτόν το χρήστη που αναγκάζει τον συγχρονισμό αυτού του λογαριασμού χρήστη από προφίλ χρήστη του SharePoint σε αυτήν τη συλλογή τοποθεσιών.
 
2. Μηνύματα ηλεκτρονικού ταχυδρομείου από ροές εργασίας αποστέλλονται στους διαχειριστές συλλογής τοποθεσιών, αλλά όχι σε άλλους χρήστες και να δείτε το σφάλμα **http απαγορεύεται σε <span>https:</span>/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.
 

    Δείτε [δεν επιτρέπεται η πρόσβαση όταν στέλνετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Επίσης, επαληθεύστε ότι η δυνατότητα συλλογής τοποθεσιών της **λειτουργίας κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης** δεν είναι ενεργή.


## <a name="related-topics"></a>Σχετικά θέματα
Θέλετε να δοκιμάσετε το Microsoft Flow στο SharePoint Online;
- [Δημιουργία ροής](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint και ροή](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


