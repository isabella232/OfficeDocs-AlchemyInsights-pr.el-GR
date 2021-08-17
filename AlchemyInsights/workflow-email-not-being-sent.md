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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072520"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Το μήνυμα ηλεκτρονικού ταχυδρομείου ροής εργασίας δεν αποστέλλεται για μια SharePoint ή βιβλιοθήκη

1. Τα μηνύματα ηλεκτρονικού ταχυδρομείου από ροές εργασιών δεν αποστέλλονται σε όλους τους χρήστες ή μόνο σε συγκεκριμένους χρήστες ή εμφανίζεται το σφάλμα Δεν είναι δυνατή η αποστολή του μηνύματος ηλεκτρονικού ταχυδρομείου. Βεβαιωθείτε ότι το μήνυμα ηλεκτρονικού ταχυδρομείου **έχει έναν έγκυρο παραλήπτη.**

    Ελέγξτε εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων **"Όλα τα άτομα"** (λίστα πληροφοριών χρήστη) για τη συλλογή τοποθεσιών.  Δείγμα άμεσης διεύθυνσης URL: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx; MembershipGroupId=0

    - Εάν ο χρήστης δεν υπάρχει, βεβαιωθείτε ότι ο χρήστης έχει εισέλθει στη σελίδα. 
    - Εάν είναι εξωτερικός χρήστης, βεβαιωθείτε ότι η πρόσκλησή του έχει γίνει αποδεκτή.
    - Εάν ο χρήστης υπάρχει στην ομάδα δικαιωμάτων, βεβαιωθείτε ότι η διεύθυνση ηλεκτρονικού ταχυδρομείου είναι σωστή.
    - Εάν η διεύθυνση ηλεκτρονικού ταχυδρομείου των χρηστών δεν έχει οριστεί εδώ, δημιουργήστε ένα δείγμα ειδοποίησης για αυτόν το χρήστη, το οποίο επιβάλλει τον συγχρονισμό αυτού του λογαριασμού χρήστη από τα προφίλ χρηστών του SharePoint σε αυτήν τη συλλογή τοποθεσιών.
 
2. Τα μηνύματα ηλεκτρονικού ταχυδρομείου από ροές εργασιών αποστέλλονται στους διαχειριστές συλλογής τοποθεσιών, αλλά όχι σε άλλους χρήστες και εμφανίζεται το σφάλμα **HTTP Forbidden σε <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail.**
 

    Ανατρέξτε [στο θέμα "Δεν επιτρέπεται η πρόσβαση" όταν στέλνετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε SharePoint ομάδας.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Επίσης, βεβαιωθείτε ότι η δυνατότητα **συλλογής τοποθεσιών λειτουργίας** κλειδώματος δικαιωμάτων χρήστη περιορισμένης πρόσβασης δεν είναι ενεργή.


## <a name="related-topics"></a>Σχετικά θέματα
Θέλετε να δοκιμάσετε Microsoft Flow στο SharePoint Online;
- [Δημιουργία Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint και Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


