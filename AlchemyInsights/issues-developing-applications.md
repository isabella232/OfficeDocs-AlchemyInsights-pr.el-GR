---
title: Ζητήματα ανάπτυξης εφαρμογών
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013424"
---
# <a name="issues-developing-applications"></a>Ζητήματα ανάπτυξης εφαρμογών

Για να αντιμετωπίσετε τα πιο συνηθισμένα προβλήματα κατά τη δημιουργία Azure Active Directory (AD), ανατρέξτε στα ακόλουθα άρθρα:

- [Βλέπω προβλήματα κατά την είσοδο σε εφαρμογές χρησιμοποιώντας μόνο το πρόγραμμα περιήγησης Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Δεν ξέρω πώς να αλλάξω τις προεπιλογές διάρκειας ζωής διακριτικού για την εφαρμογή μου](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Έχω μπερδευτεί σχετικά με τον τρόπο με τον οποίο λειτουργεί η συγκατάθεση της εφαρμογής](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Δεν ξέρω πώς να εκ παραχωρώ δικαιώματα στην εφαρμογή μου](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Δεν κατανοώ τη διαφορά μεταξύ δικαιωμάτων ανάθεσης και εφαρμογής](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Λήξη υποστήριξης για τη Azure Active Directory ελέγχου ταυτότητας (ADAL) και το Azure AD Graph API (AAD Graph)***

- Από τις 30 Ιουνίου 2020, δεν θα προσθέσουμε άλλες νέες δυνατότητες στη Βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και του Azure AD Graph API (AAD Graph). Θα συνεχίσουμε να παρέχουμε ενημερώσεις τεχνικής υποστήριξης και ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.

- Από τις 30 Ιουνίου 2022, θα τερματίσουμε την υποστήριξη για το ADAL και το AAD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας. Ως αποτέλεσμα αυτής της συνθήκης, οι επιπτώσεις είναι οι εξής:

    - Οι εφαρμογές που χρησιμοποιούν το ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα λαμβάνουν καμία τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

    - Οι εφαρμογές που χρησιμοποιούν Graph AAD μετά από αυτό το χρονικό διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό Graph AAD

**Μετεγκατάσταση ADAL**

Εάν χρησιμοποιείτε εφαρμογές της Microsoft, συνιστάται να κάνετε ενημέρωση στη Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL), η οποία διαθέτει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας. Αυτή η σύσταση βρίσκεται στο πλαίσιο της προετοιμασίας από τη Microsoft της διαδικασίας μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι το τέλος της προθεσμίας υποστήριξης. 

Η μετεγκατάσταση από τη Microsoft των εφαρμογών της στο MSAL εξασφαλίζει ότι οι εφαρμογές επωφελούνται από τις συνεχείς βελτιώσεις ασφάλειας και δυνατοτήτων της MSAL.

1. [Διαβάστε τις Συνήθεις ερωτήσεις του ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές ανά πλατφόρμα](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε τον πηγαίο κώδικα όλων των εφαρμογών σας και, εάν υπάρχει, να προσεγγίσετε τυχόν ανεξάρτητους προμηθευτές λογισμικού (ISV) ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παράσχει μια λίστα με όλες τις εφαρμογές ADAL που δεν είναι της Microsoft στον μισθωτή σας.

**Μετεγκατάσταση του AAD Graph**

Για εφαρμογές που χρησιμοποιούν εφαρμογές AAD Graph, ακολουθήστε τις οδηγίες μας για να μετεγκαταστήσετε Graph AAD στο Microsoft Graph:

1. [Η λίστα ελέγχου μετεγκατάστασης παρέχει ένα σημείο εκκίνησης](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Η πύλη καταχώρησης εφαρμογών Azure δείχνει ποιες εφαρμογές χρησιμοποιούν το AAD Graph. Συνιστάται να εξετάσετε τον πηγαίο κώδικα όλων των εφαρμογών σας και, εάν υπάρχει, να ηχείτε σε όλους τους ανεξάρτητους προμηθευτές λογισμικού (ISV) ή τις υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει πληροφορίες σχετικά με Graph AAD στον μισθωτή σας.







