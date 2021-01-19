---
title: Προβλήματα κατά την είσοδο σε εφαρμογές
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901034"
---
# <a name="issues-signing-in-to-applications"></a>Προβλήματα κατά την είσοδο σε εφαρμογές

Για να εντοπίσετε την αιτία ή τη διάγνωση προβλημάτων που σχετίζονται με την είσοδο του χρήστη, ακολουθήστε τα παρακάτω βήματα:

1. Εκκινήστε το [διαγνωστικό εισόδου](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Εντοπίστε το συμβάν για ανάλυση, πληκτρολογώντας τις λεπτομέρειες που έχετε σχετικά με το χρήστη, την εφαρμογή, την ώρα εισόδου, το αναγνωριστικό αίτησης ή το αναγνωριστικό συσχέτισης.
3. Εξετάστε τα διαγνωστικά αποτελέσματα που δείχνουν τις λεπτομέρειες σχετικά με το τι συνέβη και ποιες ενέργειες μπορείτε να ακολουθήσετε για να κάνετε αλλαγές, εάν χρειάζονται αλλαγές.

Ακολουθούν ορισμένα συνηθισμένα προβλήματα που ενδέχεται να αντιμετωπίσετε κατά την είσοδο σε εφαρμογές:

1. Εσείς ή ο χρήστης έχετε **ολοκληρώσει μια σύνδεση AD Azure, αλλά εμφανίζεται μια μη αναμενόμενη ερώτηση** -ανατρέξτε στα άρθρα [μη αναμενόμενη συναίνεση, όταν συνδέεστε σε μια εφαρμογή](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) και [μη αναμενόμενο σφάλμα κατά την εκτέλεση συναίνεσης σε μια εφαρμογή](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Εσείς ή ένας χρήστης έχετε **εισέλθει απευθείας σε μια εφαρμογή, αλλά δεν μπορείτε να εισέλθετε σε αυτό από ένα deeplink στην προσαρμοσμένη πύλη ή στον πίνακα της Access**: ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων εισόδου σε μια εφαρμογή από τις εφαρμογές Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Εσείς ή ένας χρήστης έχετε **ολοκληρώσει μια σύνδεση AD Azure, αλλά η εφαρμογή εμφανίζει ένα μήνυμα σφάλματος και δεν επιτρέπει στο χρήστη να ολοκληρώσει τη ροή εισόδου**: το πρόβλημα είναι ότι η εφαρμογή δεν αποδέχτηκε την απόκριση που εκδόθηκε από το Azure AD. Ακολουθήστε [τα παρακάτω βήματα](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) για την αντιμετώπιση προβλημάτων.
4. Εσείς ή ένας χρήστης **δεν μπορείτε να εισέλθετε σε μια εφαρμογή χωρίς συλλογή που έχει ρυθμιστεί για καθολική σύνδεση με κωδικό πρόσβασης**: ακολουθήστε τις οδηγίες σε [αυτά τα βήματα](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) για την αντιμετώπιση προβλημάτων.
5. Εσείς ή ένας χρήστης **δεν μπορείτε να εισέλθετε σε μια εφαρμογή συλλογής Azure AD που έχει ρυθμιστεί για καθολική σύνδεση με κωδικό πρόσβασης**: ακολουθήστε [τα παρακάτω βήματα](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) για την αντιμετώπιση προβλημάτων.
6. Εσείς ή ένας χρήστης **δεν μπορείτε να εισέλθετε σε μια εφαρμογή της Microsoft**: ακολουθήστε [τα παρακάτω βήματα](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) για την αντιμετώπιση προβλημάτων.
7. Εσείς ή ένας χρήστης **δεν μπορείτε να εισέλθετε σε μια εφαρμογή μη συλλογής που έχει ρυθμιστεί για ομόσπονδη καθολική σύνδεση**: ακολουθήστε [τα παρακάτω βήματα](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) για την αντιμετώπιση προβλημάτων.
8. Εσείς ή ένας χρήστης **δεν μπορείτε να εισέλθετε σε μια εφαρμογή συλλογής Azure AD που έχει ρυθμιστεί για ομόσπονδη καθολικής σύνδεσης**: ακολουθήστε [τα παρακάτω βήματα](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) για την αντιμετώπιση προβλημάτων.
9. Εσείς ή ένας χρήστης **δεν μπορείτε να εισέλθετε σε μια προσαρμοσμένη εφαρμογή**: ακολουθήστε [τα παρακάτω βήματα](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) για την αντιμετώπιση προβλημάτων.
10. Εσείς ή ένας χρήστης **δεν μπορείτε να εισέλθετε σε μια εφαρμογή εσωτερικής εγκατάστασης χρησιμοποιώντας το διακομιστή μεσολάβησης εφαρμογής Azure AD**: ακολουθήστε [τα παρακάτω βήματα](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) για την αντιμετώπιση προβλημάτων.

