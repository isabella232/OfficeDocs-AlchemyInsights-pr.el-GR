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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069964"
---
# <a name="conditional-access-issues"></a>Προβλήματα πρόσβασης υπό όρους

**Επίλυση προβλημάτων με τα Διαγνωστικά σύνδεσης**

Μπορείτε να μάθετε γρήγορα τι συνέβη ή να διαγνώσετε προβλήματα που σχετίζονται με την είσοδο χρήστη, χρησιμοποιώντας το [Διαγνωστικό σύνδεσης:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Εκκινεί το Διαγνωστικό είσοδο.
1. Βρείτε το συμβάν για ανάλυση εισάγοντας τις λεπτομέρειες που έχετε σχετικά με το χρήστη, την εφαρμογή, την ώρα της σύνδεσης, το αναγνωριστικό αίτησης ή το αναγνωριστικό συσχέτισης.
1. Εξετάστε τα διαγνωστικά αποτελέσματα που δείχνουν τις λεπτομέρειες του τι συνέβη και τις ενέργειες που μπορείτε να κάνετε για να κάνετε αλλαγές (εάν απαιτούνται αλλαγές).

**Βήματα για την αντιμετώπιση προβλημάτων μιας σύνδεσης** 

1. Μεταβείτε στη σελίδα "Είσοδος Azure AD".
1. Φιλτράρετε τις είσοδοι κατά χρήστη, εύρος χρόνου, εφαρμογή, κατάσταση, εφαρμογή-πελάτη και άλλα.
1. Επιλέξτε ένα συμβάν είσοδος και προβάλετε την καρτέλα "Πρόσβαση υπό όρους" για να δείτε ποιες πολιτικές έχουν υπολογιστεί.
1. Κάντε κλικ στη γραμμή μιας πολιτικής για να προβάλετε τις λεπτομέρειες της πολιτικής και να κατανοήσετε γιατί εφαρμόστηκε.

**Εργαλεία για την αντιμετώπιση προβλημάτων μιας πολιτικής πρόσβασης υπό όρους**

- Η λειτουργία μόνο για αναφορά σάς επιτρέπει να αξιολογήσετε μια πολιτική χωρίς να επηρεάζει τους χρήστες.
- Το εργαλείο what-if σάς επιτρέπει να προσομοιώνετε συμβάντα είσοδος και να βλέπετε ποιες πολιτικές εφαρμόζονται.
- Πληροφορίες και το βιβλίο εργασίας αναφοράς εμφανίζει τις επιπτώσεις κάθε πολιτικής σε πραγματικό χρόνο.

**Πολιτικές προστασίας γραμμής βάσης**

Οι πολιτικές προστασίας γραμμής βάσης έχουν υποτιμηθεί. Δεν επιβάλλονται πλέον και σύντομα θα καταργηθούν από την πύλη Azure. Συνιστάται να ενεργοποιήσετε [τις προεπιλογές ασφαλείας.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Για περισσότερες πληροφορίες σχετικά με την πρόσβαση υπό όρους, ανατρέξτε στο θέμα:

[Βέλτιστες πρακτικές για την πρόσβαση υπό όρους Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Συνθήκες στην πρόσβαση υπό όρους](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Στοιχεία ελέγχου στην πρόσβαση υπό όρους](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Θέσεις στην πρόσβαση υπό όρους](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
