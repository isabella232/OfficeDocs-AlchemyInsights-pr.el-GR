---
title: Αντιμετώπιση προβλημάτων συμμετοχής στο Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939919"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Αντιμετώπιση προβλημάτων συμμετοχής στο Azure AD

1. Εάν ρυθμίζετε καταχωρήσεις συσκευών για πρώτη φορά, βεβαιωθείτε ότι έχετε ελέγξει την Εισαγωγή στη διαχείριση συσκευών στο [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) που θα σας καθοδηγήσει σχετικά με τον τρόπο με τον οποίο μπορείτε να ρυθμίσετε τις συσκευές στο Azure AD. 
1. Εάν καταχωρείτε συσκευές απευθείας στο Azure AD και τις εγγράφετε στο Intune, θα πρέπει πρώτα [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) να βεβαιωθείτε ότι έχετε ρυθμίσει τις παραμέτρους του [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) και ότι έχετε ήδη ρυθμίσει τις άδειες χρήσης.
1. Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Azure AD. Μόνο ένας καθολικός διαχειριστής στο Microsoft Azure Active Directory μπορεί να διαχειρίζεται τις ρυθμίσεις για εγγραφές συσκευών.
1. Για να κάνετε την υλοποίηση συμμετοχής στο Azure AD, [ανατρέξτε στο θέμα Σχεδιασμός συμμετοχής στο Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Για περισσότερες λεπτομέρειες σχετικά με την επίλυση συνηθισμένων προβλημάτων με τη συμμετοχή στο Azure AD, ανατρέξτε στο θέμα Συνήθεις ερωτήσεις για τη συμμετοχή στο [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) και για τη συσκευή Windows 10 pro, ανατρέξτε στο θέμα Δεν είναι δυνατή η συμμετοχή του υπολογιστή Windows 10 Pro στο Azure AD - Πρέπει να κάνετε αναβάθμιση σε - Κοινότητα της [Microsoft](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
