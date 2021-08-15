---
title: Ζητήματα ανάπτυξης εφαρμογών με API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013460"
---
# <a name="issues-developing-applications-with-apis"></a>Ζητήματα ανάπτυξης εφαρμογών με API

Για να ξεκινήσετε να χρησιμοποιείτε Azure Active Directory Graph API, ανατρέξτε στον οδηγό γρήγορης εκκίνησης του [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ή προβάλετε την αλληλεπιδραστική τεκμηρίωση αναφοράς azure [AD Graph API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Λήξη υποστήριξης για τη Azure Active Directory ελέγχου ταυτότητας (ADAL) και το Azure AD Graph API (AAD Graph)**

**Από τις 30 Ιουνίου 2020,** δεν θα προσθέτουμε πλέον νέες δυνατότητες στο ADAL και το Azure AD Graph. Θα συνεχίσουμε να παρέχουμε ενημερώσεις τεχνικής υποστήριξης και ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.

**Από τις 30 Ιουνίου 2022,** θα τερματίσουμε την υποστήριξη για το ADAL και το Azure AD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

Οι εφαρμογές που χρησιμοποιούν το ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα λαμβάνουν καμία τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

Οι εφαρμογές που χρησιμοποιούν το Azure AD Graph μετά από αυτό το χρονικό διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό Graph Azure AD.

**Μετεγκατάσταση ADAL**

Συνιστάται να κάνετε ενημέρωση στη [Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), η οποία διαθέτει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας.

Εάν χρησιμοποιείτε εφαρμογές της Microsoft, να γνωρίζετε ότι η Microsoft βρίσκεται σε διαδικασία μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι το τέλος της προθεσμίας υποστήριξης, εξασφαλίζοντας ότι θα επωφεληθούν από τις συνεχείς βελτιώσεις ασφάλειας και δυνατοτήτων της MSAL.

1. [Διαβάστε τις Συνήθεις ερωτήσεις για το ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές ανά πλατφόρμα.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε τον πηγαίο κώδικα όλων των εφαρμογών σας και, εάν υπάρχει, να χρησιμοποιήσετε τυχόν ISV ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παράσχει μια λίστα με όλες τις εφαρμογές ADAL που δεν είναι της Microsoft στον μισθωτή σας.

**Μετεγκατάσταση του AAD Graph**

Για εφαρμογές που χρησιμοποιούν το Azure AD Graph, ακολουθήστε τις οδηγίες μας για τη μετεγκατάσταση εφαρμογών [Azure AD Graph στο Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Η λίστα ελέγχου μετεγκατάστασης παρέχει ένα σημείο εκκίνησης](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Η πύλη καταχώρησης εφαρμογών Azure δείχνει ποιες εφαρμογές χρησιμοποιούν το AAD Graph. Συνιστάται να εξετάσετε ολόκληρο τον πηγαίο κώδικα των εφαρμογών σας και, εάν ισχύει, επικοινωνήστε με οποιονδήποτε ISV ή πάροχο εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα όλων των Graph AAD στο μισθωτή σας.
1. Για να έχει πρόσβαση η εφαρμογή σας σε δεδομένα στο Microsoft Graph, ο χρήστης ή ο διαχειριστής πρέπει να της εκχωρήσει τα σωστά δικαιώματα μέσω μιας διαδικασίας συγκατάθεσης. Η [αναφορά δικαιωμάτων Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) Microsoft παραθέτει τα δικαιώματα που σχετίζονται με κάθε κύριο σύνολο API Graph Microsoft. Παρέχει επίσης οδηγίες σχετικά με τον τρόπο χρήσης των δικαιωμάτων.
