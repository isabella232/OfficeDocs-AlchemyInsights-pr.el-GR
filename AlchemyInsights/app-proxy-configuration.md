---
title: Ρύθμιση παραμέτρων διακομιστή μεσολάβησης εφαρμογών
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951565"
---
# <a name="app-proxy-configuration"></a>Ρύθμιση παραμέτρων διακομιστή μεσολάβησης εφαρμογών

1. Για να κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους μιας εφαρμογής διακομιστή μεσολάβησης εφαρμογών μέσα στο Azure AD για να εκθέσετε τις εφαρμογές εσωτερικής εγκατάστασης στο cloud, ανατρέξτε στο θέμα Τρόπος ρύθμισης [παραμέτρων μιας εφαρμογής διακομιστή μεσολάβησης εφαρμογών.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Η ενιαία σύνδεση (SSO) επιτρέπει στους χρήστες σας να αποκτήσουν πρόσβαση σε μια εφαρμογή χωρίς να ελεγχθεί ο έλεγχος ταυτότητας πολλές φορές. Επιτρέπει την ολοκλήρωση του μεμονωμένου ελέγχου ταυτότητας στο cloud, σε σχέση με το Azure Active Directory και επιτρέπει στην υπηρεσία ή το Connector να μιμεί το χρήστη για να ολοκληρώσει τυχόν πρόσθετες προκλήσεις ελέγχου ταυτότητας από την εφαρμογή. Για να μάθετε περισσότερα, ανατρέξτε στο θέμα Πώς μπορείτε να ρυθμίσετε τις παραμέτρους της μεμονωμένης [sign-on σε μια εφαρμογή διακομιστή μεσολάβησης εφαρμογών.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Χρησιμοποιήστε αυτό [το άρθρο για](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) να αντιμετωπίσετε συνήθη προβλήματα που αντιμετωπίζουν οι χρήστες κατά τη δημιουργία μιας νέας εφαρμογής διακομιστή μεσολάβησης εφαρμογών.
4. Εάν αντιμετωπίζετε πρόβλημα με τη ρύθμιση του ελέγχου ταυτότητας back-end στην εφαρμογή σας, ίσως χρειαστεί να αντιμετωπίσετε τις περιορισμένες ρυθμίσεις παραμέτρων ανάθεσης [kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) για το διακομιστή μεσολάβησης εφαρμογών ή να ακολουθήσετε οδηγίες σχετικά με τη ρύθμιση παραμέτρων της εφαρμογής [με το PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) για να επιλύσετε το πρόβλημά σας.
