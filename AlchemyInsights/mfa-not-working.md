---
title: Ζητήματα με ΣΠΙ
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250165"
---
# <a name="issues-with-mfa"></a>Ζητήματα με ΣΠΙ
Υπάρχουν μερικά πράγματα που πρέπει να ελέγξετε αν οι χρήστες δεν είναι δυνατό να συνδεθεί χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ)

1. Ο χρήστης που έχει επηρεαστεί μπορεί να έχει αποκλειστεί στο Active Directory Azure στο εμπόριο. Εάν συμβαίνει αυτό, ο έλεγχος ταυτότητας επιχειρεί ότι συγκεκριμένος χρήστης δεν θα έχει αυτόματα. [Ακολουθήστε τα βήματα σε αυτό το άρθρο για να καταργήσετε τον αποκλεισμό τους.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Εάν η κατάργηση του αποκλεισμού του χρήστη δεν σας βοήθησε ή ο χρήστης δεν αποκλείεται να δοκιμάσετε να επαναφέρετε ΣΠΙ για το χρήστη και θα μεταβούν στη διαδικασία εγγραφή ξανά. [Ακολουθήστε τα βήματα σε αυτό το άρθρο.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Εάν αυτή είναι η πρώτη φορά που δεν ΣΠΙ ενεργοποιημένο και οι χρήστες σας είναι δυνατό να συνδεθείτε στους υπολογιστές-πελάτες δεν είναι προγράμματα περιήγησης όπως το Outlook, Skype, κλπ, ίσως ADAL (βιβλιοθήκη ελέγχου ταυτότητας Active Directory) δεν είναι ενεργοποιημένη για τη συνδρομή σας O365. Στην περίπτωση αυτή θα πρέπει να συνδεθείτε με το Exchange Online Powershell και να εκτελέσετε αυτό το cmdlet:  *σύνολο-OrganizationConfig-OAuth2ClientProfileEnabled: $true*