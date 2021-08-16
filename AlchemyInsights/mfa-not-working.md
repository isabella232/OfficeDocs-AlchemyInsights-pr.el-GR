---
title: Προβλήματα με το MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098602"
---
# <a name="issues-with-azure-mfa"></a>Προβλήματα με το Azure MFA
Υπάρχουν μερικά πράγματα που πρέπει να ελέγξετε εάν οι χρήστες δεν μπορούν να συνδεθούν χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων (MFA)

1. Ο χρήστης που επηρεάζεται ενδέχεται να αποκλειστεί στην Azure Active Directory πύλης. Σε αυτή την περίπτωση, οι προσπάθειες ελέγχου ταυτότητας για τον συγκεκριμένο χρήστη θα αποτεφράονται αυτόματα. [Ακολουθήστε τα βήματα σε αυτό το άρθρο για να τα ξεμπλοκάρει.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Εάν η κατάργηση του αποκλεισμού του χρήστη δεν βοήθησε ή ο χρήστης δεν αποκλειστεί, μπορείτε να προσπαθήσετε να επαναφέρετε το MFA για το χρήστη και θα περάσει ξανά τη διαδικασία εγγραφής. [Ακολουθήστε τα βήματα σε αυτό το άρθρο.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Εάν αυτή είναι η πρώτη φορά που έχετε ενεργοποιήσει το MFA και οι χρήστες σας δεν μπορούν να συνδεθείτε σε προγράμματα-πελάτες που δεν είναι προγράμματα περιήγησης, όπως το Outlook, το Skype κ.λπ., ίσως το ADAL (Βιβλιοθήκη ελέγχου ταυτότητας Active Directory) να μην είναι ενεργοποιημένο στη συνδρομή σας στο O365. Σε αυτή την περίπτωση, θα πρέπει να συνδεθείτε στο Exchange Online Powershell και να εκτελέσετε αυτό το cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*