---
title: Προβλήματα με την ανάπτυξη εφαρμογών με API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974617"
---
# <a name="issues-developing-applications-with-apis"></a>Προβλήματα με την ανάπτυξη εφαρμογών με API

Για να ξεκινήσετε να χρησιμοποιείτε το API γραφήματος Azure Active Directory, ανατρέξτε στο θέμα [Οδηγός γρήγορης εκκίνησης του Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ή προβολή της [τεκμηρίωσης της αλληλεπιδραστικής αναφοράς αναφοράς API του Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Λήξη υποστήριξης για τη βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και το API του Azure AD Graph (AAD Graph)**

**Ξεκινώντας στις 30 Ιουνίου, 2020**, δεν θα προσθέτουμε πλέον νέες ΔΥΝΑΤΌΤΗΤΕς στο ADAL και το Azure AD Graph. Θα συνεχίσουμε να παρέχουμε τεχνική υποστήριξη και ενημερώσεις ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.

**Ξεκινώντας στις 30 Ιουνίου, 2022**, θα τερματίσουμε την υποστήριξη για το ADAL και το Azure AD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

Οι εφαρμογές που χρησιμοποιούν το ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα έχουν οποιαδήποτε τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

Οι εφαρμογές που χρησιμοποιούν το Azure AD Graph μετά από αυτό το διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό σημείο του Azure AD Graph.

**Μετεγκατάσταση ADAL**

Συνιστούμε να κάνετε ενημέρωση στη [βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), η οποία έχει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας.

Εάν χρησιμοποιείτε τις εφαρμογές της Microsoft, να γνωρίζετε ότι η Microsoft βρίσκεται στη διαδικασία μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι την λήξη της προθεσμίας υποστήριξης, εξασφαλίζοντας ότι θα επωφεληθούν από τις συνεχιζόμενες βελτιώσεις ασφαλείας και δυνατοτήτων του MSAL.

1. [Διαβάστε τις συνήθεις ερωτήσεις για το ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές σε βάση ανά πλατφόρμα](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιαδήποτε ISV ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα με όλες τις εφαρμογές που δεν ανήκουν στη Microsoft ADAL στον μισθωτή σας.

**Μετεγκατάσταση γραφήματος AAD**

Για τις εφαρμογές που χρησιμοποιούν το Azure AD Graph, ακολουθήστε τις οδηγίες για τη μετεγκατάσταση [εφαρμογών Azure AD Graph στο Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Ο πίνακας ελέγχου μετεγκατάστασης παρέχει ένα χρονικό ξεκίνημα](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Η πύλη δήλωσης της εφαρμογής Azure εμφανίζει ποιες εφαρμογές χρησιμοποιούν το AAD Graph. Σας συνιστούμε να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιαδήποτε ISV ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα με όλες AAD τη χρήση γραφημάτων στο μισθωτή σας.
1. Για την εφαρμογή σας για την πρόσβαση σε δεδομένα στο Microsoft Graph, ο χρήστης ή ο διαχειριστής πρέπει να του εκχωρήσει τα κατάλληλα δικαιώματα μέσω μιας διαδικασίας συγκατάθεσης. Η [αναφορά δικαιωμάτων του Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) παραθέτει τα δικαιώματα που σχετίζονται με κάθε κύριο πρόγραμμα API του Microsoft Graph. Παρέχει επίσης οδηγίες σχετικά με τον τρόπο χρήσης των δικαιωμάτων.
