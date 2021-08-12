---
title: Δικαιώματα API και διαδικασία συγκατάθεσης
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932061"
---
# <a name="api-permissions-and-consent-process"></a>Δικαιώματα API και διαδικασία συγκατάθεσης

Για να έχει πρόσβαση η εφαρμογή σας σε δεδομένα στο Microsoft Graph, ο χρήστης ή ο διαχειριστής πρέπει να της εκχωρήσει τα σωστά δικαιώματα μέσω μιας διαδικασίας συγκατάθεσης. [Η Graph δικαιωμάτων της Microsoft παραθέτει](https://docs.microsoft.com/graph/permissions-reference) τα δικαιώματα που σχετίζονται με κάθε κύριο σύνολο API Graph Microsoft. Παρέχει επίσης οδηγίες σχετικά με τον τρόπο χρήσης των δικαιωμάτων.

**Ρύθμιση ή ενημέρωση της κύριας υπηρεσίας**

- [Δημιουργία serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να δημιουργήσετε ένα νέο αντικείμενο servicePrincipal.
- [Δημιουργήστε μια εφαρμογή Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) κύρια υπηρεσία στην πύλη - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να δημιουργήσετε μια νέα εφαρμογή και μια κύρια υπηρεσία του Azure Active Directory (Azure AD) που μπορούν να χρησιμοποιηθούν με τον έλεγχο πρόσβασης βάσει ρόλων.
- [Εφαρμογές &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) υπηρεσίες στο Azure AD - Αυτό το άρθρο περιγράφει την καταχώρηση εφαρμογών, τα αντικείμενα εφαρμογών και τις κύριες αρχές υπηρεσιών στο Azure Active Directory: τι είναι, πώς χρησιμοποιούνται και πώς σχετίζονται μεταξύ τους.

**Προσθήκη ή ενημέρωση εγγραφής εφαρμογής και παροχή συγκατάθεσης διαχειριστή**

- [Δημιουργία καταχώρησης εφαρμογής](https://docs.microsoft.com/graph/api/application-post-applications) - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να δημιουργήσετε ένα νέο αντικείμενο εφαρμογής.
- [Ενημέρωση καταχώρησης εφαρμογής - Δικαιώματα API](https://docs.microsoft.com/graph/api/application-update) - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να ενημερώσετε τις ιδιότητες ενός αντικειμένου εφαρμογής.
- [Παροχή συγκατάθεσης διαχειριστή](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Για τη συγκατάθεση και τη συγκατάθεση των διαχειριστών γενικά, απαιτούμε από έναν διαχειριστή να παραχωρεί ρητά τη συγκατάθεσή του.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Κοντέινερ διαχείρισης ρόλων για ενοποιημένους ορισμούς ρόλων και αναθέσεις ρόλων για τις υπηρεσίες παροχής RBAC του Microsoft 365 που υποστηρίζουν πολλές κύριες αρχές και πολλαπλές εμβέλειες σε μία ανάθεση ρόλων. Αυτό είναι διαφορετικό από *τον τύπο πόρου rbacApplication.* Microsoft Intune παράδειγμα μιας τέτοιας υπηρεσίας παροχής RBAC. Μια ανάθεση ρόλων στο Intune μπορεί να έχει έναν πίνακα εντολών και έναν πίνακα ομάδων εμβέλειας. **Αυτό είναι σε βήτα, που σημαίνει ότι βρίσκεται ακόμη σε εξέλιξη και δεν συνιστάται για χρήση στην παραγωγή.**
