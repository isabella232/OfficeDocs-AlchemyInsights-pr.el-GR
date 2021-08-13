---
title: Αντιμετώπιση προβλημάτων συγκατάθεσης χρήστη
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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007898"
---
# <a name="troubleshoot-user-consent"></a>Αντιμετώπιση προβλημάτων συγκατάθεσης χρήστη

1. Μπορείτε να ρυθμίσετε τον τρόπο με τον οποίο οι τελικοί χρήστες συναινούν σε εφαρμογές μέσω της Πύλης Azure ή του PowerShell. Ανατρέξτε [στις ρυθμίσεις συγκατάθεσης](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) χρήστη για περισσότερες πληροφορίες.
1. Ένας διαχειριστής μπορεί επίσης να χρησιμοποιήσει [το MICROSOFT Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) για να εκχωρήσει συγκατάθεση σε δικαιώματα που έχουν ανατεθεί εκ μέρους ενός μεμονωμένου χρήστη. Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα Λήψη πρόσβασης εκ μέρους ενός χρήστη.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Σφάλματα συγκατάθεσης χρήστη:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)αυτό το άρθρο περιγράφει σφάλματα που μπορεί να προκύψουν κατά τη διαδικασία συγκατάθεσης σε μια εφαρμογή. Εάν αντιμετωπίζετε μη αναμενόμενα μηνύματα συγκατάθεσης που δεν περιέχουν μηνύματα σφάλματος, ανατρέξτε στο θέμα [Σενάρια ελέγχου ταυτότητας για το Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)