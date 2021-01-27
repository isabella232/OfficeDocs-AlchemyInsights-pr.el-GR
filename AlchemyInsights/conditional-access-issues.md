---
title: Προβλήματα πρόσβασης υπό όρους
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014790"
---
# <a name="conditional-access-issues"></a>Προβλήματα πρόσβασης υπό όρους

**Επίλυση προβλημάτων με το διαγνωστικό εισόδου**

Μπορείτε να μάθετε γρήγορα τι συνέβη ή να διαγνώσετε προβλήματα που σχετίζονται με την είσοδο του χρήστη, χρησιμοποιώντας το [διαγνωστικό εισόδου](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Εκκινήστε το διαγνωστικό εισόδου.
1. Εντοπίστε το συμβάν για ανάλυση, πληκτρολογώντας τις λεπτομέρειες που έχετε σχετικά με το χρήστη, την εφαρμογή, την ώρα εισόδου, το αναγνωριστικό αίτησης ή το αναγνωριστικό συσχέτισης.
1. Εξετάστε τα διαγνωστικά αποτελέσματα που δείχνουν τις λεπτομέρειες σχετικά με το τι συνέβη και ποιες ενέργειες μπορείτε να ακολουθήσετε για να κάνετε αλλαγές (εάν χρειάζονται αλλαγές).

**Βήματα για την αντιμετώπιση προβλημάτων εισόδου** 

1. Μεταβείτε στη σελίδα εισόδου του Azure AD.
1. Φιλτράρισμα εισόδου ανά χρήστη, χρονική περιοχή, εφαρμογή, κατάσταση, εφαρμογή προγράμματος-πελάτη και ούτω καθεξής.
1. Επιλέξτε ένα συμβάν εισόδου και προβάλετε την καρτέλα "πρόσβαση υπό όρους" για να δείτε ποιες πολιτικές έχουν αξιολογηθεί.
1. Κάντε κλικ στη γραμμή μιας πολιτικής για να δείτε τις λεπτομέρειες της πολιτικής και να καταλάβετε γιατί εφαρμόστηκε.

**Εργαλεία για την αντιμετώπιση μιας πολιτικής πρόσβασης υπό όρους**

- Η λειτουργία "μόνο αναφορά" σάς επιτρέπει να αξιολογείτε μια πολιτική χωρίς να επηρεάζονται οι χρήστες.
- Το εργαλείο what-if σάς επιτρέπει να προσομοιώσετε συμβάντα εισόδου και να δείτε ποιες πολιτικές ισχύουν.
- Το βιβλίο εργασίας "Insights and Reporting" εμφανίζει τις επιπτώσεις σε πραγματικό χρόνο κάθε πολιτικής.

**Πολιτικές προστασίας γραμμής βάσης**

Οι πολιτικές προστασίας γραμμής βάσης έχουν καταργηθεί. Δεν εφαρμόζονται πλέον και σύντομα θα καταργηθούν από την πύλη Azure. Συνιστούμε να ενεργοποιήσετε τις [προεπιλογές ασφαλείας](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Για περισσότερες πληροφορίες σχετικά με την πρόσβαση υπό όρους, ανατρέξτε στα θέματα:

[Βέλτιστες πρακτικές για την υπό όρους πρόσβαση στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Συνθήκες στην πρόσβαση](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 υπό όρους [Στοιχεία ελέγχου σε πρόσβαση](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 υπό όρους [Θέσεις στην πρόσβαση υπό όρους](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
