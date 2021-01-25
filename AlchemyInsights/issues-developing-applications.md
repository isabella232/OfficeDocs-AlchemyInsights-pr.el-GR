---
title: Προβλήματα με την ανάπτυξη εφαρμογών
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974476"
---
# <a name="issues-developing-applications"></a>Προβλήματα με την ανάπτυξη εφαρμογών

Για να αντιμετωπίσετε τα πιο συνηθισμένα προβλήματα κατά τη δημιουργία εφαρμογών Azure Active Directory (AD), ανατρέξτε στα ακόλουθα άρθρα:

- [Αντιμετωπίζω προβλήματα κατά την είσοδο σε εφαρμογές χρησιμοποιώντας μόνο το πρόγραμμα περιήγησης Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Δεν γνωρίζω πώς να αλλάξω τις προεπιλογές διάρκειας ζωής διακριτικού για την εφαρμογή μου](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Είμαι σε σύγχυση σχετικά με τον τρόπο λειτουργίας της συγκατάθεσης εφαρμογών](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Δεν γνωρίζω πώς να εκχωρήσω δικαιώματα στην εφαρμογή μου](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Δεν κατανοώ τη διαφορά μεταξύ των δικαιωμάτων ανάθεσης και εφαρμογής](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Λήξη υποστήριξης για τη βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και το API του Azure AD Graph (AAD Graph)** _

- Ξεκινώντας στις 30 Ιουνίου, 2020, δεν θα προσθέτουμε πλέον νέες δυνατότητες στη βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και στο Azure AD Graph API (AAD Graph). Θα συνεχίσουμε να παρέχουμε τεχνική υποστήριξη και ενημερώσεις ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.

- Ξεκινώντας στις 30 Ιουνίου 2022, θα τερματίσουμε την υποστήριξη για το ADAL και το AAD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας. Ως αποτέλεσμα αυτής της Συνθήκης, οι συνέπειες είναι οι εξής:

    - Οι εφαρμογές που χρησιμοποιούν το ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα έχουν οποιαδήποτε τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

    - Οι εφαρμογές που χρησιμοποιούν το AAD Graph μετά από αυτό το χρονικό διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό σημείο του AAD Graph

_ *ADAL μετεγκατάστασης**

Εάν χρησιμοποιείτε τις εφαρμογές Microsoft, συνιστούμε να κάνετε ενημέρωση στη βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL), η οποία έχει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας. Αυτή η σύσταση βρίσκεται στο πλαίσιο της Microsoft για την έναρξη της διαδικασίας μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι την λήξη της προθεσμίας υποστήριξης. 

Η μετεγκατάσταση από τη Microsoft των εφαρμογών της στο MSAL διασφαλίζει ότι οι εφαρμογές επωφελούνται από τη συνεχιζόμενη βελτίωση της ασφάλειας και των δυνατοτήτων του MSAL.

1. [Διαβάστε τις συνήθεις ερωτήσεις για το ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές σε βάση ανά πλατφόρμα](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιουσδήποτε ανεξάρτητους προμηθευτές λογισμικού (ISV) ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα με όλες τις εφαρμογές που δεν ανήκουν στη Microsoft ADAL στον μισθωτή σας.

**Μετεγκατάσταση γραφήματος AAD**

Για εφαρμογές που χρησιμοποιούν το AAD Graph, ακολουθήστε τις οδηγίες μας για να μετεγκαταστήσετε τις εφαρμογές Graph του AAD στο Microsoft Graph:

1. [Ο πίνακας ελέγχου μετεγκατάστασης παρέχει ένα χρονικό ξεκίνημα](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Η πύλη δήλωσης της εφαρμογής Azure εμφανίζει ποιες εφαρμογές χρησιμοποιούν το AAD Graph. Σας συνιστούμε να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιουσδήποτε ανεξάρτητους προμηθευτές λογισμικού (ISV) ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει πληροφορίες σχετικά με τη χρήση του AAD Graph στον μισθωτή σας.







