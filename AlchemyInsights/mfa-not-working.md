---
title: Θέματα με τη ΜΧΣ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768837"
---
# <a name="issues-with-azure-mfa"></a>Ζητήματα με τη ΜΧΣ Azure
Υπάρχουν μερικά πράγματα για να ελέγξετε αν οι χρήστες δεν μπορούν να συνδεθούν χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ)

1. Ο χρήστης που επηρεάζεται ενδέχεται να αποκλειστεί στην πύλη Azure Active Directory. Σε αυτήν την περίπτωση, οι απόπειρες ελέγχου ταυτότητας για τον συγκεκριμένο χρήστη θα απορρίπτονται αυτόματα. [Ακολουθήστε τα βήματα σε αυτό το άρθρο για να καταργήσετε τον αποκλεισμό τους.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Εάν ξεμπλοκάρισμα ο χρήστης δεν βοήθησε ή ο χρήστης δεν είναι αποκλεισμένη μπορείτε να προσπαθήσετε να επαναφέρετε ΣΠΙ για το χρήστη και θα περάσουν από τη διαδικασία εγγραφής και πάλι. [Ακολουθήστε τα βήματα σε αυτό το άρθρο.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Εάν αυτή είναι η πρώτη φορά που ενεργοποιήσατε τη ΜΧΣ και οι χρήστες σας δεν είναι σε θέση να συνδεθείτε σε προγράμματα-πελάτες που δεν είναι προγράμματα περιήγησης, όπως το Outlook, Skype, κλπ, ίσως δεν είναι ενεργοποιημένο (βιβλιοθήκη ελέγχου ταυτότητας Active Directory) στη συνδρομή σας O365. Σε αυτήν την περίπτωση θα πρέπει να συνδεθείτε με το Exchange Online PowerShell και να εκτελέσετε αυτό το cmdlet:  *set-οργάνωση config-OAuth2ClientProfileEnabled: $True*