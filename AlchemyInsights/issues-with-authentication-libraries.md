---
title: Προβλήματα με τις βιβλιοθήκες ελέγχου ταυτότητας
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028004"
---
# <a name="issues-with-authentication-libraries"></a>Προβλήματα με τις βιβλιοθήκες ελέγχου ταυτότητας

1. [Πλατφόρμα ταυτοτήτων της Microsoft βιβλιοθήκες ελέγχου ταυτότητας παραθέτει](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) βιβλιοθήκες προγράμματος-πελάτη και middleware που υποστηρίζονται από τη Microsoft.
2. Η Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL) υποστηρίζει πολλές [ροές ελέγχου ταυτότητας](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) για χρήση σε διαφορετικά σενάρια εφαρμογών.
3. Για τον έλεγχο ταυτότητας και την απόκτηση διακριτικών, μπορείτε να αρχικοποιήσετε μια νέα δημόσια ή εμπιστευτική εφαρμογή-πελάτη στον κώδικά σας. Μπορείτε να ορίσετε διάφορες επιλογές ρύθμισης παραμέτρων κατά την προετοιμασία της εφαρμογής-πελάτη στη Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL). Για να μάθετε περισσότερα, ανατρέξτε στο [θέμα Επιλογές ρύθμισης παραμέτρων εφαρμογής.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Λήξη υποστήριξης για τη Azure Active Directory ελέγχου ταυτότητας (ADAL) και το Azure AD Graph API (AAD Graph)**

**Από τις 30 Ιουνίου 2020,** δεν θα προσθέτουμε πλέον νέες δυνατότητες στο ADAL και το Azure AD Graph. Θα συνεχίσουμε να παρέχουμε ενημερώσεις τεχνικής υποστήριξης και ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.

**Από τις 30 Ιουνίου 2022,** θα τερματίσουμε την υποστήριξη για το ADAL και το Azure AD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

Οι εφαρμογές που χρησιμοποιούν ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα λάβετε *τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.*

Οι εφαρμογές που χρησιμοποιούν το Azure AD Graph μετά από αυτό το χρονικό διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό Graph Azure AD.

**Μετεγκατάσταση ADAL**

Συνιστάται να κάνετε ενημέρωση στη [Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), η οποία διαθέτει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας.

Εάν χρησιμοποιείτε εφαρμογές της Microsoft, να γνωρίζετε ότι η Microsoft βρίσκεται σε διαδικασία μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι το τέλος της προθεσμίας υποστήριξης, εξασφαλίζοντας ότι θα επωφεληθούν από τις συνεχείς βελτιώσεις ασφάλειας και δυνατοτήτων της MSAL.

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

1. [Διαβάστε τις Συνήθεις ερωτήσεις του ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές ανά πλατφόρμα](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε τον πηγαίο κώδικα όλων των εφαρμογών σας και, εάν υπάρχει, να χρησιμοποιήσετε τυχόν ISV ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παράσχει μια λίστα με όλες τις εφαρμογές ADAL που δεν είναι της Microsoft στον μισθωτή σας.

**Μετεγκατάσταση του AAD Graph**

Για εφαρμογές που χρησιμοποιούν το Azure AD Graph, ακολουθήστε τις οδηγίες μας για τη μετεγκατάσταση εφαρμογών [Azure AD Graph στο Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Η λίστα ελέγχου μετεγκατάστασης παρέχει ένα σημείο γρήγορα αποτελέσματα.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Η πύλη καταχώρησης εφαρμογών Azure δείχνει ποιες εφαρμογές χρησιμοποιούν το AAD Graph. Συνιστάται να εξετάσετε ολόκληρο τον πηγαίο κώδικα των εφαρμογών σας και, εάν ισχύει, επικοινωνήστε με οποιονδήποτε ISV ή πάροχο εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα όλων των Graph AAD στο μισθωτή σας.
3. Για να έχει πρόσβαση η εφαρμογή σας σε δεδομένα στο Microsoft Graph, ο χρήστης ή ο διαχειριστής πρέπει να της εκχωρήσει τα σωστά δικαιώματα μέσω μιας διαδικασίας συγκατάθεσης. Η [αναφορά δικαιωμάτων Graph](https://docs.microsoft.com/graph/permissions-reference) Microsoft παραθέτει τα δικαιώματα που σχετίζονται με κάθε κύριο σύνολο API Graph Microsoft. Παρέχει επίσης οδηγίες σχετικά με τον τρόπο χρήσης των δικαιωμάτων.
