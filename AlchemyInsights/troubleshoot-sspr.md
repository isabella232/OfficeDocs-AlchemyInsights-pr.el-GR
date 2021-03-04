---
title: Αντιμετώπιση προβλημάτων SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429720"
---
# <a name="troubleshoot-sspr"></a>Αντιμετώπιση προβλημάτων SSPR

**Δεν μπορώ να ρυθμίσω τις παραμέτρους της επαναφοράς κωδικού πρόσβασης**

- Εάν είστε διαχειριστής και αναζητάτε τρόπο για να ενεργοποιήσετε την επαναφορά κωδικού πρόσβασης από το χρήστη, ανατρέξτε στο θέμα "Πρόγραμμα εκμάθησης" για να ενεργοποιήσετε το [SSPR,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)για να ρυθμίσετε τις παραμέτρους επαναφοράς κωδικού πρόσβασης για τον οργανισμό σας. Μπορείτε επίσης να εξετάσετε τις απαιτήσεις [άδειας χρήσης.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Πρέπει να έχετε εκχωρήσει τουλάχιστον μία άδεια χρήσης στον οργανισμό σας.
    - **Μόνο για χρήστες cloud** - Οποιαδήποτε SKU επί πληρωμή για το Office 365 (O365) ή Azure AD Basic
    - **Χρήστες cloud ή/και** εσωτερικής εγκατάστασης - Azure AD Premium P1 ή P2, Φορητότητα για μεγάλες επιχειρήσεις + Ασφάλεια (EMS) ή Secure Productive Enterprise (SPE)
- Για πρόσθετες ερωτήσεις σχετικά με την επαναφορά κωδικού πρόσβασης από το χρήστη, διαβάστε τις [Συνήθεις ερωτήσεις.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Εμφανίζεται ένα μήνυμα σφάλματος**

Διαβάστε αυτό το άρθρο για να βρείτε συνηθισμένα σφάλματα και τις λύσεις τους: Αντιμετώπιση [προβλημάτων επαναφοράς κωδικού πρόσβασης από το χρήστη](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Έχω πρόβλημα με την πολιτική επαναφοράς κωδικού πρόσβασης**

- Εάν η πολιτική επαναφοράς κωδικού πρόσβασης δεν είναι η αναμενόμενη ή εάν έχετε απορίες σχετικά με τις πολιτικές επαναφοράς κωδικού πρόσβασης, διαβάστε αυτό το άρθρο: Πολιτικές και περιορισμοί κωδικών πρόσβασης [στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Οι πολιτικές επαναφοράς κωδικού πρόσβασης δεν ισχύουν για διαχειριστές. Η Microsoft επιβάλλει μια ισχυρή προεπιλεγμένη πολιτική επαναφοράς κωδικού πρόσβασης δύο πυλών για οποιονδήποτε ρόλο διαχειριστή Azure. Βεβαιωθείτε ότι κάνετε δοκιμές με ένα χρήστη που δεν είναι διαχειριστής. Για περισσότερες πληροφορίες σχετικά με την πολιτική επαναφοράς διαχειριστή, ανατρέξτε σε αυτό το άρθρο: Διαφορές πολιτικής [επαναφοράς διαχειριστή.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Δεν θέλω οι χρήστες μου να καταχωρήσουν πρόσθετες πληροφορίες ασφάλειας για επαναφορά κωδικού πρόσβασης**

Μπορείτε να προ-συμπληρώσετε τα δεδομένα (χαρακτηριστικά ηλεκτρονικού ταχυδρομείου και τηλεφώνου) για τους χρήστες σας χρησιμοποιώντας ένα API, το PowerShell ή το Azure AD Connect. Για να μάθετε πώς να διαβάζετε:

- [Ανάπτυξη επαναφοράς κωδικού πρόσβασης χωρίς να απαιτείται καταχώρηση από τους χρήστες](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Ποια δεδομένα χρησιμοποιούνται από την επαναφορά κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Θέλω οι χρήστες μου να καταχωρήσουν τις πρόσθετες πληροφορίες ασφαλείας τους για επαναφορά του κωδικού πρόσβασης**

1. Κατευθύνετε τους χρήστες σας να καταχωρήσουν τις πληροφορίες ασφαλείας τους για επαναφορά κωδικού πρόσβασης από το [χρήστη, κατευθύνοντας τους aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Μετά τη συμπλήρωση των δεδομένων για το χρήστη (από το χρήστη ή από το διαχειριστή), κατευθύνετε το χρήστη στο [aka.ms/sspr](https://passwordreset.microsoftonline.com/) ώστε οι χρήστες σας να έχουν τη δυνατότητα να επαναφέρουν τους δικούς τους κωδικούς πρόσβασης.
1. Εάν οι χρήστες εξακολουθούν να αντιμετωπίζουν προβλήματα, είναι πολύ πιθανό να έχουν **ομόσπονδο συγχρονισμό** ή **να συγχρονίζονται με τον κωδικό πρόσβασης χρήστες.** Αυτό σημαίνει ότι ενδέχεται να υπάρχει πρόβλημα με την υπηρεσία writeback κωδικού πρόσβασης.