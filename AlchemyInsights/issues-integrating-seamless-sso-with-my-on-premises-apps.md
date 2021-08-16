---
title: Προβλήματα με την ενοποίηση της απρόσκοπτης SSO με τις εφαρμογές εσωτερικής εγκατάστασης
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028292"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Προβλήματα με την ενοποίηση της απρόσκοπτης SSO με τις εφαρμογές εσωτερικής εγκατάστασης

Για να αντιμετωπίσετε προβλήματα με την ενοποίηση της απρόσκοπτης SSO με εφαρμογές εσωτερικής εγκατάστασης, κάντε τα εξής:

**Προτεινόμενα βήματα**

1. Για να **ρυθμίσετε τις παραμέτρους μιας εφαρμογής εσωτερικής** εγκατάστασης για μία είσοδο μέσω του διακομιστή μεσολάβησης εφαρμογών, ανατρέξτε στο θέμα Θησαυροφυλάκιο κωδικών πρόσβασης για μεμονωμένη σύνδεση με το διακομιστή [μεσολάβησης εφαρμογών.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Αντιμετώπιση προβλημάτων διακομιστή μεσολάβησης** εφαρμογών: συνιστάται να ξεκινήσετε με την εξέταση των προβλημάτων ροής αντιμετώπισης προβλημάτων, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)προβλημάτων σύνδεσης διακομιστή μεσολάβησης εφαρμογών εντοπισμού σφαλμάτων, για να προσδιορίσετε εάν οι συνδέσεις διακομιστή μεσολάβησης εφαρμογών έχουν ρυθμιστεί σωστά. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα κατά τη σύνδεση με την εφαρμογή, ακολουθήστε τα βήματα αντιμετώπισης προβλημάτων στα [ζητήματα της εφαρμογής διακομιστή μεσολάβησης εφαρμογών εντοπισμού σφαλμάτων.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Μπορείτε να [προσδιορίσετε προβλήματα CORS χρησιμοποιώντας](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) τα ακόλουθα εργαλεία εντοπισμού σφαλμάτων του προγράμματος περιήγησης:
    1. Εκκινηθείτε το πρόγραμμα περιήγησης και μεταβείτε στην εφαρμογή web.
    1. Πατήστε **το πλήκτρο F12** για να αναφέρετε την κονσόλα εντοπισμού σφαλμάτων.
    1. Προσπαθήστε να αναπαραγάγετε τη συναλλαγή και εξετάστε το μήνυμα κονσόλας. Μια παραβίαση CORS προκαλεί ένα σφάλμα κονσόλας σχετικά με την προέλευση.
    1. Ορισμένα ζητήματα CORS δεν είναι δυνατό να επιλυθούν, όπως όταν η εφαρμογή σας ανακατευθύνει στο login.microsoftonline.com για έλεγχο ταυτότητας και το διακριτικό πρόσβασης λήγει. Η κλήση CORS, στη συνέχεια, αποτυγχάνει. Μια λύση για αυτό το σενάριο είναι να επεκτείνετε τη διάρκεια ζωής του διακριτικού πρόσβασης, για να αποτρέψετε τη λήξη του κατά τη διάρκεια της περιόδου λειτουργίας ενός χρήστη. Για περισσότερες πληροφορίες σχετικά με τον τρόπο για να το κάνετε αυτό, ανατρέξτε στο θέμα "Διάρκεια ζωής διακριτικών με [δυνατότητα ρύθμισης παραμέτρων" Πλατφόρμα ταυτοτήτων της Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Προτεινόμενα έγγραφα**

- [Τρόπος ρύθμισης παραμέτρων της μεμονωμένης sign-on σε μια εφαρμογή διακομιστή μεσολάβησης εφαρμογών](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Μεμονωμένη σύνδεση SAML για εφαρμογές εσωτερικής εγκατάστασης με διακομιστή μεσολάβησης εφαρμογών](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Κατανόηση και επίλυση προβλημάτων Azure Active Directory διακομιστή μεσολάβησης εφαρμογών CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Αντιμετώπιση προβλημάτων με περιορισμένες ρυθμίσεις παραμέτρων ανάθεσης kerberos για το διακομιστή μεσολάβησης εφαρμογών](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)