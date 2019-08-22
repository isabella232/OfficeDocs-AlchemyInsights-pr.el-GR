---
title: Δεν γίνεται αποστολή email ροής εργασίας
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530873"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Ροή εργασίας ηλεκτρονικού ταχυδρομείου δεν αποστέλλονται για μια λίστα ή βιβλιοθήκη SharePoint

1. Μήνυμα ηλεκτρονικού ταχυδρομείου από τις ροές εργασίας δεν αποστέλλονται σε όλους τους χρήστες ή μόνο σε συγκεκριμένους χρήστες ή μπορείτε να δείτε το σφάλμα **του μηνύματος ηλεκτρονικού ταχυδρομείου δεν μπορεί να αποσταλεί. Βεβαιωθείτε ότι το μήνυμα ηλεκτρονικού ταχυδρομείου έχει έγκυρο παραλήπτη**.

    Ελέγξτε εάν υπάρχει ο χρήστης στην ομάδα δικαιώματα **Όλων των ατόμων** (λίστα πληροφοριών χρήστη) για αυτήν τη συλλογή τοποθεσιών.  Δείγμα απευθείας URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx; MembershipGroupId = 0

    - Εάν ο χρήστης δεν υπάρχει, βεβαιωθείτε ότι ο χρήστης έχει υπογραφή σε αυτήν τη σελίδα. 
    - Εάν πρόκειται για έναν εξωτερικό χρήστη, βεβαιωθείτε ότι έχει γίνει αποδεκτή την πρόσκληση.
    - Εάν ο χρήστης υπάρχει στην ομάδα δικαιώματα, βεβαιωθείτε ότι η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σωστή.
    - Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου "χρήστες" δεν έχει οριστεί εδώ, στη συνέχεια, δημιουργήστε ένα υπόδειγμα ειδοποίησης για αυτόν το χρήστη που επιβάλλει ο συγχρονισμός από αυτόν το λογαριασμό χρήστη από το προφίλ χρήστη του SharePoint σε αυτήν τη συλλογή τοποθεσιών.
 
2. Μήνυμα ηλεκτρονικού ταχυδρομείου από ροές εργασίας αποστέλλονται οι διαχειριστές συλλογής τοποθεσιών, αλλά όχι σε άλλους χρήστες και να δείτε το σφάλμα **HTTP, δεν επιτρέπεται να <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Ανατρέξτε στο θέμα [Πρόσβαση όταν στέλνετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Επίσης, βεβαιωθείτε ότι η δυνατότητα συλλογής τοποθεσιών **κατάσταση λειτουργίας κλειδώματος δικαιωμάτων περιορισμένης πρόσβασης χρήστη** δεν είναι ενεργό.


## <a name="related-topics"></a>Σχετικά θέματα
Θέλετε να δοκιμάσετε τη ροή της Microsoft με την ηλεκτρονική του SharePoint;
- [Δημιουργία ροής](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Του SharePoint και ροής](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


