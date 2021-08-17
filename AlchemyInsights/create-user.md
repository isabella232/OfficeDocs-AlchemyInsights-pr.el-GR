---
title: Δημιουργία χρήστη
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: afba00ffc6ba082606e0071b41e2917b11e6a39d61cd0df7e468f0238f2ed8e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118744"
---
# <a name="create-user"></a>Δημιουργία χρήστη

**ΑΝΑΚΟΙΝΩΣΗ:**

- [Η απόσβεση της υποστήριξης για είσοδο WebView από την Google από τις 4 Ιανουαρίου 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Ελέγξτε εάν οι εφαρμογές σας ενδέχεται να επηρεαστούν [ακολουθώντας τις οδηγίες της Google σχετικά](https://go.microsoft.com/fwlink/?linkid=2157323) με τη συμβατότητα των δοκιμών.
- Βεβαιωθείτε ότι χρησιμοποιείτε το webview συστήματος ή το πρόγραμμα περιήγησης συστήματος κατά την είσοδο στους χρήστες σας με λογαριασμούς Google καταναλωτών. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Προβλήματα κατά την είσοδο σε εφαρμογές χρησιμοποιώντας μόνο το πρόγραμμα περιήγησης Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Δεν μπορώ να δημιουργήσω έναν νέο χρήστη στον κατάλογο Azure AD**

1. Βεβαιωθείτε ότι έχετε εξουσιοδότηση για τη δημιουργία ενός νέου τυπικού χρήστη. Μόνο ο καθολικός διαχειριστής ή ο ρόλος διαχειριστή χρήστη στο Azure Active Directory (AD) μπορεί να δημιουργήσει έναν νέο τυπικό χρήστη. Εάν δεν είστε σε έναν από αυτούς τους ρόλους, ζητήστε από ένα διαχειριστή να σας προσθέσει σε έναν από αυτούς τους ρόλους ή να δημιουργήσει το νέο λογαριασμό χρήστη για εσάς.
1. Βεβαιωθείτε ότι το όνομα χρήστη βρίσκεται σε έναν τομέα που έχει επαληθευτεί στο Azure AD. Εάν δεν έχετε επαληθευμένα προσαρμοσμένα ονόματα τομέων στο Azure AD, μπορείτε να χρησιμοποιήσετε τον αρχικό τομέα Azure AD, ο οποίος τελειώνει σε *.onmicrosoft.com.
1. Βεβαιωθείτε ότι το όνομα χρήστη βρίσκεται σε έναν τομέα που δεν είναι ομόσπονδος με το Azure AD από το AD εσωτερικής εγκατάστασης. Δεν είναι δυνατή η προσθήκη χρηστών στο cloud με ονόματα τομέων που είναι ομόσπονδα από την εσωτερική εγκατάσταση.
1. Βεβαιωθείτε ότι κανένας άλλος χρήστης ή επαφή δεν έχει ήδη το όνομα χρήστη που θέλετε να εκχωρήσετε στο νέο χρήστη. Τα ονόματα χρηστών πρέπει να είναι μοναδικά στο Azure AD.
1. Ανατρέξτε [στους ρόλους και τους διαχειριστές του Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) για το Azure AD.
1. Δείτε τα [ονόματα τομέων](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) για το Azure AD.
1. Εξετάστε [τα αρχεία καταγραφής](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) ελέγχου για να δείτε πιο λεπτομερείς πληροφορίες σχετικά με έναν χρήστη που δημιουργήθηκε ή διαγράφηκε πρόσφατα, όπως ποιος εκτέλεσε την ενέργεια και πότε.
1. Για περισσότερες πληροφορίες σχετικά με την προσθήκη νέων χρηστών, ανατρέξτε στο θέμα [Χρήση της πύλης Azure για τη δημιουργία ενός νέου χρήστη στο Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Ρόλοι διαχείρισης Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)Δικαιώματα ρόλων διαχειριστή σε Azure Active Directory
1. Μπορείτε επίσης να [χρησιμοποιήσετε το Azure AD PowerShell για να δημιουργήσετε ένα νέο χρήστη.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
