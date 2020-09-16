---
title: Προβλήματα με το ΣΠΙ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755131"
---
# <a name="issues-with-azure-mfa"></a>Προβλήματα με το Azure ΣΠΙ
Υπάρχουν μερικά πράγματα που πρέπει να εξετάσετε εάν οι χρήστες δεν μπορούν να συνδεθούν χρησιμοποιώντας τον έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ)

1. Ο χρήστης που επηρεάζεται μπορεί να αποκλειστεί στην πύλη του Azure Active Directory. Σε αυτή την περίπτωση, οι προσπάθειες ελέγχου ταυτότητας για τον συγκεκριμένο χρήστη θα απορριφθούν αυτόματα. [Ακολουθήστε τα βήματα που περιέχετε σε αυτό το άρθρο για να καταργήσετε τον αποκλεισμό τους.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Εάν ο αποκλεισμός του χρήστη δεν βοήθησε ή ο χρήστης δεν αποκλειστεί, μπορείτε να δοκιμάσετε να επαναφέρετε το ΣΠΙ για το χρήστη και θα περάσουν από τη διαδικασία εγγραφής ξανά. [Ακολουθήστε τα βήματα που περιλάβετε σε αυτό το άρθρο.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Εάν αυτή είναι η πρώτη φορά που ενεργοποιήσατε το ΣΠΙ και οι χρήστες σας δεν μπορούν να συνδεθούν σε προγράμματα-πελάτες που δεν χρησιμοποιούν προγράμματα περιήγησης, όπως το Outlook, το Skype, το κ. λπ., ίσως το ADAL (βιβλιοθήκη ελέγχου ταυτότητας της υπηρεσίας καταλόγου Active Directory) δεν είναι ενεργοποιημένο στη συνδρομή σας στο O365. Σε αυτή την περίπτωση, θα πρέπει να συνδεθείτε στο Exchange Online PowerShell και να εκτελέσετε αυτό το cmdlet:  *OrganizationConfig-OAuth2ClientProfileEnabled: $True*