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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404869"
---
# <a name="api-permissions-and-consent-process"></a>Δικαιώματα API και διαδικασία συγκατάθεσης

Για να αποκτήσει πρόσβαση η εφαρμογή σας σε δεδομένα στο Microsoft Graph, ο χρήστης ή ο διαχειριστής πρέπει να του εκχωρήσει τα σωστά δικαιώματα μέσω μιας διαδικασίας συγκατάθεσης. [Η αναφορά δικαιωμάτων του Microsoft Graph παραθέτει](https://docs.microsoft.com/graph/permissions-reference) τα δικαιώματα που σχετίζονται με κάθε κύριο σύνολο API του Microsoft Graph. Παρέχει επίσης οδηγίες σχετικά με τον τρόπο χρήσης των δικαιωμάτων.

**Ρύθμιση ή ενημέρωση της κύριας υπηρεσίας**

- [Δημιουργία serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να δημιουργήσετε ένα νέο αντικείμενο servicePrincipal.
- [Δημιουργήστε μια εφαρμογή Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) κύρια υπηρεσία στην πύλη - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να δημιουργήσετε μια νέα εφαρμογή azure Active Directory (Azure AD) και μια κύρια υπηρεσία που μπορεί να χρησιμοποιηθεί με τον έλεγχο πρόσβασης βάσει ρόλων.
- [Εφαρμογές &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) υπηρεσίες στο Azure AD - Αυτό το άρθρο περιγράφει την καταχώρηση εφαρμογών, τα αντικείμενα εφαρμογών και τις κύριες αρχές υπηρεσίας στο Azure Active Directory: τι είναι, πώς χρησιμοποιούνται και πώς σχετίζονται μεταξύ τους.

**Προσθήκη ή ενημέρωση εγγραφής εφαρμογής και παροχή συγκατάθεσης διαχειριστή**

- [Δημιουργία καταχώρησης εφαρμογής](https://docs.microsoft.com/graph/api/application-post-applications) - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να δημιουργήσετε ένα νέο αντικείμενο εφαρμογής.
- [Ενημέρωση καταχώρησης εφαρμογής - Δικαιώματα API](https://docs.microsoft.com/graph/api/application-update) - Αυτό το άρθρο σάς δείχνει πώς μπορείτε να ενημερώσετε τις ιδιότητες ενός αντικειμένου εφαρμογής.
- [Παροχή συγκατάθεσης διαχειριστή](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Για τη συγκατάθεση και τη συγκατάθεση των διαχειριστών γενικά, απαιτούμε από έναν διαχειριστή να παραχωρεί ρητά τη συγκατάθεσή του.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Κοντέινερ διαχείρισης ρόλων για ενοποιημένους ορισμούς ρόλων και αναθέσεις ρόλων για υπηρεσίες παροχής RBAC του Microsoft 365 που υποστηρίζουν πολλές κύριες αρχές και πολλαπλές εμβέλειες σε μία ανάθεση ρόλων. Αυτό είναι διαφορετικό από *τον τύπο πόρου rbacApplication.* Το Microsoft Intune είναι ένα παράδειγμα μιας τέτοιας υπηρεσίας παροχής RBAC. Μια ανάθεση ρόλων στο Intune μπορεί να έχει έναν πίνακα εντολών και έναν πίνακα ομάδων εμβέλειας. **Αυτό είναι σε βήτα, που σημαίνει ότι βρίσκεται ακόμη σε εξέλιξη και δεν συνιστάται για χρήση στην παραγωγή.**
