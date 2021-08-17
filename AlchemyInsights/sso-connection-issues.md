---
title: Προβλήματα σύνδεσης SSO
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084346"
---
# <a name="sso-connection-issues"></a>Προβλήματα σύνδεσης SSO

1. Ακολουθήστε τη Γρήγορη [εκκίνηση: Ρυθμίστε τις παραμέτρους ιδιοτήτων για έναν οδηγό εφαρμογής για να](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ρυθμίσετε τις παραμέτρους της εφαρμογής σας.
2. Ανάλογα με την εφαρμογή και [την επιλογή "Ενιαία σύνδεση"](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) που επιλέξατε, ακολουθήστε τις κατάλληλες οδηγίες παρακάτω:
    - Για να **ρυθμίσετε** τις παραμέτρους μιας εφαρμογής εσωτερικής εγκατάστασης για μεμονωμένη σύνδεση που βασίζεται **σε SAML,** ανατρέξτε στο θέμα "Ενιαία σύνδεση SAML" για εφαρμογές εσωτερικής [εγκατάστασης με διακομιστή μεσολάβησης εφαρμογών.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Για να ρυθμίσετε **τις παραμέτρους μιας εφαρμογής** cloud για μία σύνδεση που βασίζεται σε κωδικό **πρόσβασης,** ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων μονής σύνδεσης με κωδικό πρόσβασης.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Για να **ρυθμίσετε τις παραμέτρους μιας εφαρμογής εσωτερικής** εγκατάστασης για μία είσοδο μέσω του διακομιστή μεσολάβησης εφαρμογών, ανατρέξτε στο θέμα Θησαυροφυλάκιο κωδικών πρόσβασης για μεμονωμένη σύνδεση με το διακομιστή [μεσολάβησης εφαρμογών.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Αντιμετώπιση προβλημάτων διακομιστή μεσολάβησης** εφαρμογών: συνιστάται να ξεκινήσετε με την εξέταση των προβλημάτων ροής [αντιμετώπισης](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)προβλημάτων, προβλημάτων σύνδεσης διακομιστή μεσολάβησης εφαρμογών εντοπισμού σφαλμάτων, για να προσδιορίσετε εάν οι συνδέσεις διακομιστή μεσολάβησης εφαρμογών έχουν ρυθμιστεί σωστά. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα κατά τη σύνδεση με την εφαρμογή, ακολουθήστε τη ροή αντιμετώπισης προβλημάτων στα [ζητήματα της εφαρμογής διακομιστή μεσολάβησης εφαρμογών εντοπισμού σφαλμάτων.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Μπορείτε να [προσδιορίσετε προβλήματα CORS χρησιμοποιώντας](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) τα εργαλεία εντοπισμού σφαλμάτων του προγράμματος περιήγησης:
    - Εκκινηθείτε το πρόγραμμα περιήγησης και μεταβείτε στην εφαρμογή web.
    - Πατήστε **το πλήκτρο F12** για να αναφέρετε την κονσόλα εντοπισμού σφαλμάτων.
    - Προσπαθήστε να αναπαραγάγετε τη συναλλαγή και εξετάστε το μήνυμα κονσόλας. Μια παραβίαση CORS προκαλεί ένα σφάλμα κονσόλας σχετικά με την προέλευση.
    - Ορισμένα ζητήματα CORS δεν είναι δυνατό να επιλυθούν, όπως όταν η εφαρμογή σας ανακατευθύνει στο login.microsoft.com για έλεγχο ταυτότητας και το διακριτικό πρόσβασης λήγει. Η κλήση CORS, στη συνέχεια, αποτυγχάνει. Μια λύση για αυτό το σενάριο είναι να επεκτείνετε τη διάρκεια ζωής του διακριτικού πρόσβασης, για να αποτρέψετε τη λήξη του κατά τη διάρκεια της περιόδου λειτουργίας ενός χρήστη. Για περισσότερες πληροφορίες σχετικά με τον τρόπο για να το κάνετε αυτό, ανατρέξτε στο θέμα "Διάρκεια ζωής διακριτικών με [δυνατότητα ρύθμισης παραμέτρων" Πλατφόρμα ταυτοτήτων της Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **Αντιμετώπιση προβλημάτων μεμονωμένης** σύνδεσης που βασίζεται σε SAML: συνιστάται να ελέγχετε τα προβλήματα κατά την είσοδο σε εφαρμογές που βασίζονται σε μία είσοδο που βασίζεται σε [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)για να βρείτε τις λύσεις στα προβλήματα που είναι πιο πιθανό να αντιμετωπίσετε.
5. **Αντιμετώπιση προβλημάτων** μονής σύνδεσης που βασίζεται σε κωδικό πρόσβασης: συνιστάται να ελέγχετε την αντιμετώπιση προβλημάτων της μεμονωμένης σύνδεσης που βασίζεται σε κωδικό πρόσβασης στο [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)για να βρείτε τις λύσεις στα προβλήματα που είναι πιο πιθανό να αντιμετωπίσετε.
6. Για προβλήματα σύνδεσης κατά τη χρήση vpn, ανατρέξτε στο θέμα Τρόπος χρήσης της μεμονωμένης σύνδεσης [(SSO) μέσω VPN και Wi-Fi συνδέσεων.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
