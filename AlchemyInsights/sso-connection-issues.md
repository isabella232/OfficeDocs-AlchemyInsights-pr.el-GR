---
title: Ζητήματα σύνδεσης SSO
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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935113"
---
# <a name="sso-connection-issues"></a>Ζητήματα σύνδεσης SSO

1. Ακολουθήστε την γρήγορη [εκκίνηση: Ρυθμίστε τις παραμέτρους ιδιοτήτων για έναν οδηγό εφαρμογής για να](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ρυθμίσετε τις παραμέτρους της εφαρμογής σας.
2. Ανάλογα με την εφαρμογή και [την επιλογή "Μονή σύνδεση" που](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) επιλέξατε, ακολουθήστε τις κατάλληλες οδηγίες παρακάτω:
    - Για να **ρυθμίσετε** τις παραμέτρους μιας εφαρμογής εσωτερικής εγκατάστασης για την μεμονωμένη σύνδεση που βασίζεται σε **SAML,** ανατρέξτε στην ενότητα SAML για εφαρμογές εσωτερικής εγκατάστασης με διακομιστή [μεσολάβησης εφαρμογών.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Για να ρυθμίσετε **τις παραμέτρους μιας εφαρμογής cloud** για την ενιαία σύνδεση που βασίζεται σε κωδικό **πρόσβασης,** ανατρέξτε στο θέμα ["Ρύθμιση παραμέτρων της μεμονωμένης σύνδεσης με κωδικό πρόσβασης".](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Για να ρυθμίσετε **τις παραμέτρους** μιας εφαρμογής εσωτερικής εγκατάστασης για την ενιαία σύνδεση μέσω διακομιστή μεσολάβησης εφαρμογών, ανατρέξτε στο θέμα "Θυρίδα κωδικών πρόσβασης για την ενιαία σύνδεση με το διακομιστή [μεσολάβησης εφαρμογών".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 
3. **Αντιμετώπιση** προβλημάτων με το διακομιστή μεσολάβησης εφαρμογών: Συνιστάται να ξεκινήσετε με την εξέταση της ροής αντιμετώπισης [προβλημάτων,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)τα προβλήματα σύνδεσης διακομιστή μεσολάβησης εφαρμογών εντοπισμού σφαλμάτων, για να προσδιορίσετε εάν οι συνδέσεις διακομιστή μεσολάβησης εφαρμογών έχουν ρυθμιστεί σωστά. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα κατά τη σύνδεση με την εφαρμογή, ακολουθήστε τη ροή αντιμετώπισης προβλημάτων στα προβλήματα [εφαρμογής διακομιστή μεσολάβησης εφαρμογών εντοπισμού σφαλμάτων.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Μπορείτε να [προσδιορίσετε προβλήματα CORS χρησιμοποιώντας](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) εργαλεία εντοπισμού σφαλμάτων του προγράμματος περιήγησης:
    - Εκκινούν το πρόγραμμα περιήγησης και περιηγηθούν στην εφαρμογή web.
    - Πατήστε **το πλήκτρο F12** για να επάνω στην κονσόλα εντοπισμού σφαλμάτων.
    - Προσπαθήστε να αναπαραγάγετε τη συναλλαγή και ελέγξτε το μήνυμα της κονσόλας. Η παραβίαση CORS παράγει ένα σφάλμα κονσόλας σχετικά με την προέλευση.
    - Ορισμένα ζητήματα corS δεν μπορούν να επιλυθούν, όπως όταν η εφαρμογή σας ανακατευθύνει στο login.microsoft.com για έλεγχο ταυτότητας και το διακριτικό πρόσβασης λήξει. Η κλήση CORS, στη συνέχεια, αποτυγχάνει. Μια λύση για αυτό το σενάριο είναι να επεκτείνετε τη διάρκεια ζωής του διακριτικού πρόσβασης, για να αποτρέψετε τη λήξη του κατά τη διάρκεια μιας περιόδου λειτουργίας χρήστη. Για περισσότερες πληροφορίες σχετικά με το πώς να το κάνετε αυτό, ανατρέξτε στο θέμα "Διάρκεια ζωής διακριτικών με δυνατότητα [ρύθμισης" στην πλατφόρμα ταυτοτήτων Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. Αντιμετώπιση προβλημάτων της μοναδικής σύνδεσης που βασίζεται σε **SAML:** Συνιστάται να ελέγχετε τα προβλήματα κατά την είσοδο σε εφαρμογές με ρυθμισμένες τις παραμέτρους της μεμονωμένης σύνδεσης που βασίζονται σε [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)για να βρείτε τις λύσεις στα προβλήματα που είναι πιο πιθανό να αντιμετωπίσετε.
5. **Αντιμετώπιση** προβλημάτων της μοναδικής σύνδεσης που βασίζεται σε κωδικό πρόσβασης: Συνιστάται να ελέγξετε την αντιμετώπιση προβλημάτων της μοναδικής σύνδεσης που βασίζεται σε κωδικό πρόσβασης στο [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)για να βρείτε τις λύσεις στα προβλήματα που είναι πιο πιθανό να αντιμετωπίσετε.
6. Για προβλήματα σύνδεσης κατά τη χρήση VPN, ανατρέξτε στο θέμα Πώς μπορείτε να χρησιμοποιήσετε την ενιαία σύνδεση [(SSO) μέσω VPN και Wi-Fi σύνδεσης.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
