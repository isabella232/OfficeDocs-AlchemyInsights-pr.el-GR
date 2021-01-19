---
title: Αντιμετώπιση προβλημάτων συναίνεσης χρήστη
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901192"
---
# <a name="troubleshoot-user-consent"></a>Αντιμετώπιση προβλημάτων συναίνεσης χρήστη

1. Μπορείτε να ρυθμίσετε τον τρόπο με τον οποίο οι τελικοί χρήστες συναινούν σε εφαρμογές μέσω της πύλης Azure ή του PowerShell. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [ρυθμίσεις συναίνεσης χρήστη](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Ένας διαχειριστής μπορεί επίσης να χρησιμοποιήσει το [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) για να εκχωρήσει τη συγκατάθεσή του για την ανάθεση δικαιωμάτων εκ μέρους ενός μεμονωμένου χρήστη. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Λήψη πρόσβασης εκ μέρους ενός χρήστη](https://docs.microsoft.com/graph/auth-v2-user).
1. [Σφάλματα συναίνεσης χρήστη](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): αυτό το άρθρο περιγράφει τα σφάλματα που μπορεί να προκύψουν κατά τη διαδικασία της συναίνεσης σε μια εφαρμογή. Εάν αντιμετωπίζετε μη αναμενόμενα μηνύματα συναίνεσης που δεν περιέχουν μηνύματα σφάλματος, ανατρέξτε στο θέμα [σενάρια ελέγχου ταυτότητας για το Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).