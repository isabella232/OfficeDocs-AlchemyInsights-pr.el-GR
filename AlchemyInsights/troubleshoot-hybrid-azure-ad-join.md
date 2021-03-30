---
title: Αντιμετώπιση προβλημάτων του συνδέσμου Hybrid Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401907"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Αντιμετώπιση προβλημάτων του συνδέσμου Hybrid Azure AD

Συνιστάται ιδιαίτερα. Εξασφαλίστε ότι μια συσκευή έχει πρόσβαση στα τελικά σημεία εγγραφής συσκευής κάτω από τον λογαριασμό συστήματος, χρησιμοποιώντας τη [δέσμη ενεργειών "Δοκιμή συνδεσιμότητας εγγραφής συσκευής"](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Εάν ρυθμίζετε εγγραφές συσκευών για πρώτη φορά, φροντίστε να εξετάσετε την ενότητα [Εισαγωγή στη διαχείριση συσκευών στο Microsoft Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) για να μάθετε πώς μπορείτε να θέσετε τις συσκευές υπό τον έλεγχο του Microsoft Azure Active Directory.
1. Εάν καταχωρείτε συσκευές απευθείας στο Microsoft Azure Active Directory και τις έχετε εγγράψει στο Intune, βεβαιωθείτε ότι έχετε ρυθμίσει τις [παραμέτρους του Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) και έχετε στη θέση τους τις [άδειες χρήσης](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Microsoft Azure Active Directory και στην υπηρεσία καταλόγου AD εσωτερικής εγκατάστασης. Μόνο ένας καθολικός διαχειριστής στο Microsoft Azure Active Directory μπορεί να διαχειρίζεται τις ρυθμίσεις για εγγραφές συσκευών. Επιπλέον, εάν ρυθμίζετε τις αυτόματες εγγραφές στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, θα πρέπει να είστε διαχειριστής της υπηρεσίας καταλόγου Active Directory και των υπηρεσιών AD FS (εάν υπάρχουν).

Για περισσότερες λεπτομέρειες σχετικά με την επίλυση πιθανών προβλημάτων με τον σύνδεσμο Hybrid, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων του συνδέσμου Hybrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Για τη ρύθμιση σύνδεσης μέσω Hybrid Azure AD και τη Διαχείριση συσκευών χρησιμοποιώντας την πύλη Azure AD, ανατρέξτε στο θέμα [Ρύθμιση συσκευών σε σύνδεση μέσω Hybrid Azure AD (με σύνδεση τομέα εσωτερικής εγκατάστασης)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) και [Διαχείριση συσκευών χρησιμοποιώντας την πύλη Microsoft Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Για να επιλύσετε συνήθη ζητήματα σχετικά με τον σύνδεσμο Hybrid Azure Active Directory (AD), ανατρέξτε στο θέμα [Συνήθεις ερωτήσεις για τον σύνδεσμο Hybrid Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
