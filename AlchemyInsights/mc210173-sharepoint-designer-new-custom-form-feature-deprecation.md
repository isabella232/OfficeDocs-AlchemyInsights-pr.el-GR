---
title: MC210173 - νέα προσαρμοσμένη δυνατότητα κατάργησης φόρμας του SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077662"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - νέα προσαρμοσμένη δυνατότητα κατάργησης φόρμας του SharePoint Designer

Εντοπίσαμε ένα πρόβλημα που επηρεάζει τη λειτουργικότητα του SharePoint Designer σχετικά με τη [δημιουργία προσαρμοσμένων φορμών](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) στο SharePoint Online. Μετά από προσεκτική εξέταση, διαπιστώσαμε ότι δεν υπάρχει γνωστή επιδιόρθωση για αυτό το πρόβλημα και επιλέξαμε να απενεργοποιήσουμε τη δυνατότητα "Δημιουργία προσαρμοσμένης φόρμας" με ισχύ από το Σάββατο 25 Απριλίου 2020 στις 3:00 Π.Μ. UTC. Αυτή η αλλαγή δεν επηρεάζει τη δυνατότητα επεξεργασίας φορμών που δημιουργήθηκαν στο παρελθόν ή άλλων υφιστάμενων δυνατοτήτων στο SharePoint Online Designer.

Μετά από αυτή την αλλαγή, οι χρήστες ενδέχεται να έχουν λάβει το μήνυμα σφάλματος: "Δεν ήταν δυνατή η αποθήκευση των αλλαγών λίστας στο διακομιστή" κατά τη δημιουργία νέων φορμών.

Οι χρήστες που έχουν αξιοποιήσει το SharePoint Designer, στο παρελθόν, για να δημιουργήσουν προσαρμοσμένες φόρμες, μπορούν, για τον ίδιο σκοπό και αντί αυτού να χρησιμοποιούν το [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

Το PowerApps είναι ένα εύκολο και ισχυρό εργαλείο που επιτρέπει στους χρήστες που λειτουργούν με τη σύγχρονη εμπειρία του SharePoint Online να δημιουργούν και να επεξεργάζονται προσαρμοσμένες φόρμες για λίστες και βιβλιοθήκες εγγράφων SharePoint, απευθείας από ένα παράθυρο προγράμματος περιήγησης. Το PowerApps δεν απαιτεί γνώσεις παραδοσιακής κωδικοποίησης ή τυχόν πρόσθετες λήψεις εφαρμογών, όπως το InfoPath.

**Σημείωση**: οι χρήστες του SharePoint Online Classic θα πρέπει να στραφούν προσωρινά στη σύγχρονη εμπειρία για να αποκτήσουν πρόσβαση και να χρησιμοποιήσουν το PowerApps. Ωστόσο, όλες οι προσαρμοσμένες φόρμες που έχουν δημιουργηθεί στο PowerApps είναι προσβάσιμες από χρήστες του SharePoint Online Classic.
