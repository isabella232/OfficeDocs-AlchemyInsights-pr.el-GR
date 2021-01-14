---
title: Προβλήματα με την ενοποίηση των αδιάλειπτων SSO με τις εφαρμογές εσωτερικής εγκατάστασης
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868677"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Προβλήματα με την ενοποίηση των αδιάλειπτων SSO με τις εφαρμογές εσωτερικής εγκατάστασης

Για να αντιμετωπίσετε προβλήματα με την ενοποίηση χωρίς προβλήματα SSO με τις εφαρμογές εσωτερικής εγκατάστασης, κάντε τα εξής:

**Συνιστώμενα βήματα**

1. Για να ρυθμίσετε τις παραμέτρους μιας **εφαρμογής εσωτερικής εγκατάστασης** για **καθολική σύνδεση μέσω του διακομιστή μεσολάβησης εφαρμογής**, ανατρέξτε στο θέμα [θόλος κωδικών πρόσβασης για καθολική σύνδεση με το διακομιστή μεσολάβησης εφαρμογής](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Αντιμετώπιση προβλημάτων διακομιστή μεσολάβησης εφαρμογής**: συνιστούμε να ξεκινήσετε με την αναθεώρηση της ροής αντιμετώπισης προβλημάτων, [προβλήματα σύνδεσης διακομιστή μεσολάβησης εφαρμογής εντοπισμού σφαλμάτων](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), για να προσδιορίσετε εάν οι συνδέσεις του διακομιστή μεσολάβησης εφαρμογής έχουν ρυθμιστεί σωστά. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα με τη σύνδεση με την εφαρμογή, ακολουθήστε τα βήματα αντιμετώπισης προβλημάτων στα [θέματα εφαρμογής του διακομιστή μεσολάβησης εφαρμογής εντοπισμού σφαλμάτων](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Μπορείτε να [προσδιορίσετε τα προβλήματα του Cors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) , χρησιμοποιώντας τα παρακάτω εργαλεία εντοπισμού σφαλμάτων του προγράμματος περιήγησης:
    1. Εκκινήστε το πρόγραμμα περιήγησης και μεταβείτε στην εφαρμογή Web.
    1. Πατήστε το πλήκτρο **F12** για να εμφανιστεί η κονσόλα εντοπισμού σφαλμάτων.
    1. Προσπαθήστε να αναπαραγάγετε τη συναλλαγή και εξετάστε το μήνυμα της κονσόλας. Μια παραβίαση CORS δημιουργεί ένα σφάλμα κονσόλας σχετικά με την προέλευση.
    1. Δεν είναι δυνατή η επίλυση ορισμένων ζητημάτων του CORS, όπως όταν η εφαρμογή σας ανακατευθύνει σε login.microsoftonline.com για τον έλεγχο ταυτότητας και το διακριτικό πρόσβασης λήγει. Η πρόσκληση CORS αποτυγχάνει. Μια λύση για αυτό το σενάριο είναι να επεκτείνετε τη διάρκεια ζωής του διακριτικού πρόσβασης, για να αποτρέψετε τη λήξη του κατά τη διάρκεια της περιόδου λειτουργίας ενός χρήστη. Για περισσότερες πληροφορίες σχετικά με τον τρόπο για να το κάνετε αυτό, ανατρέξτε [στο θέμα διάρκεια ζωής διακριτικού με δυνατότητα ρύθμισης παραμέτρων στην πλατφόρμα ταυτοτήτων της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Προτεινόμενα έγγραφα**

- [Πώς μπορείτε να ρυθμίσετε τις παραμέτρους καθολικής σύνδεσης σε μια εφαρμογή διακομιστή μεσολάβησης εφαρμογής](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML καθολικής σύνδεσης για εφαρμογές εσωτερικής εγκατάστασης με το διακομιστή μεσολάβησης εφαρμογής](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Κατανόηση και επίλυση ζητημάτων του διακομιστή μεσολάβησης εφαρμογής Azure Active Directory CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Αντιμετώπιση προβλημάτων ρύθμισης παραμέτρων αντιπροσώπευσης Kerberos με περιορισμούς για το διακομιστή μεσολάβησης εφαρμογής](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)