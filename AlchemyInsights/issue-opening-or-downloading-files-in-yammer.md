---
title: Ζήτημα ανοίγματος ή λήψης αρχείων στο Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148251"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Ζήτημα ανοίγματος ή λήψης αρχείων στο Yammer

Το Κλασικό Yammer υποστηρίζει πολλές επιλογές για αποστολές αρχείων σε μηνύματα και ομάδες. Ανάλογα με τη ρύθμιση παραμέτρων δικτύου, τα αρχεία είναι προεπιλεγμένα για αποθήκευση στο SharePoint.

Ο επιλογέας αρχείων στο νέο Yammer δεν υποστηρίζει ακόμα όλες τις επιλογές που είναι διαθέσιμες στο κλασικό Yammer. Μια μελλοντική ενημερωμένη έκδοση θα προσθέσει πρόσθετες δυνατότητες. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Επισύναψη αρχείου ή εικόνας σε μια δημοσίευση συνομιλίας yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Δεν είναι δυνατό το άνοιγμα ή η λήψη ενός αρχείου**  

Ένα αρχείο μπορεί να αποσταλεί στο Yammer, αλλά και να συνδεθεί με ένα αρχείο στο SharePoint Online. Για να αντιμετωπίσετε προβλήματα, πρέπει πρώτα να προσδιορίσετε τη θέση του αρχείου. Εάν το αρχείο έχει αποσταλεί στο Yammer, θα έχει διεύθυνση URL *.yammer.com. Βεβαιωθείτε ότι οι απαιτούμενες διευθύνσεις URL και διευθύνσεις IP έχουν καταργηθεί. Για περισσότερες πληροφορίες, ανατρέξτε στην καταχώρηση ιστολογίου [Η χρήση διευθύνσεων IP με σκληρό κώδικα για το Yammer δεν συνιστάται](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Ελέγξτε αν ένας χρήστης που είναι επίσης καθολικός διαχειριστής μπορεί να κάνει λήψη του αρχείου. Εάν το αρχείο είναι ιδιωτικό, ίσως χρειαστεί να χρησιμοποιήσετε τη λειτουργία ιδιωτικού περιεχομένου. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Παρακολούθηση ιδιωτικού περιεχομένου στο Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Επισκέπτες και αρχεία σε επίπεδο δικτύου Yammer στο SharePoint Online**  

[Οι επισκέπτες σε επίπεδο δικτύου στο Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) δεν χρησιμοποιούν το Azure AD B2B και είναι εσωτερικοί στην υπηρεσία Yammer, επομένως δεν μπορούν να αποκτήσουν πρόσβαση σε αρχεία Yammer που είναι αποθηκευμένα στο SharePoint. Δημιουργήστε έναν εξωτερικό χρήστη AAD B2B, ο οποίος μπορεί να έχει πρόσβαση σε βιβλιοθήκες εγγράφων στο SharePoint Online, χρησιμοποιώντας αυτήν την ταυτότητα. Για πληροφορίες σχετικά με τη μελλοντική υποστήριξη επισκεπτών Azure AD B2B στο Yammer, ανατρέξτε στο θέμα Υποστήριξη επισκέπτη από [επιχείρηση σε επιχειρήσεις (B2B) στην Προεπισκόπηση Yammer - Όροι πελατών και Συνήθεις ερωτήσεις](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).