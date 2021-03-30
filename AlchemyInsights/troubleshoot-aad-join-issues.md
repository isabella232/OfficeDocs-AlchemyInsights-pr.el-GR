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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405125"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Αντιμετώπιση προβλημάτων συμμετοχής στο Azure AD

1. Εάν ρυθμίζετε καταχωρήσεις συσκευών για πρώτη φορά, βεβαιωθείτε ότι έχετε ελέγξει την Εισαγωγή στη διαχείριση συσκευών στο [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) η οποία θα σας καθοδηγήσει σχετικά με τον τρόπο με τον οποίο μπορείτε να ρυθμίσετε τις συσκευές στο Azure AD. 
1. Εάν καταχωρείτε συσκευές απευθείας στο Azure AD και τις εγγράφετε στο Intune, θα πρέπει πρώτα [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) να βεβαιωθείτε ότι έχετε ρυθμίσει τις παραμέτρους του [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) και ότι έχετε ήδη ρυθμίσει τις άδειες χρήσης.
1. Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Azure AD. Μόνο ένας καθολικός διαχειριστής στο Azure AD μπορεί να διαχειριστεί τις ρυθμίσεις για τις καταχωρήσεις συσκευών.
1. Για να κάνετε την υλοποίηση συμμετοχής στο Azure AD, [ανατρέξτε στο θέμα Σχεδιασμός συμμετοχής στο Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Για περισσότερες λεπτομέρειες σχετικά με την επίλυση συνηθισμένων προβλημάτων με τη συμμετοχή στο Azure AD, ανατρέξτε στις Συνήθεις ερωτήσεις του [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) και για τη συσκευή Windows 10 Pro, ανατρέξτε στο θέμα Δεν είναι δυνατή η συμμετοχή του υπολογιστή Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) στο Azure AD - Πρέπει να κάνετε αναβάθμιση σε - Κοινότητα της Microsoft
