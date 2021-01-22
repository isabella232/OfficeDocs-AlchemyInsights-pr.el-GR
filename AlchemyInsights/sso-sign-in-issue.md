---
title: Απρόσκοπτα προβλήματα σύνδεσης χρήστη SSO
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935123"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Απρόσκοπτα προβλήματα σύνδεσης χρήστη SSO

Μετά τον έλεγχο ταυτότητας του χρήστη, το πρόγραμμα περιήγησης θα αποθηκεύει στο cache τα διαπιστευτήρια του χρήστη, ώστε στο ίδιο πρόγραμμα περιήγησης η εφαρμογή να κάνει αυτόματα είσοδο με τον ίδιο λογαριασμό. Αυτό μπορεί να δυσχερανει τη σύνδεση ενός άλλου χρήστη ή ενός μεμονωμένου χρήστη σε πολλούς λογαριασμούς σε μία συσκευή. Για να επιλύσετε αυτό το πρόβλημα: 1. Δοκιμάστε να εισέλθετε σε άλλο πρόγραμμα περιήγησης. 2. Κάντε εκκαθάριση της μνήμης cache ή/και των cookies του προγράμματος περιήγησης και προσπαθήστε να εισέλθετε ξανά.

Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα σύνδεσης, συνιστάται να κάνετε τα εξής για τη διάγνωση και αυτοματοποίηση των βημάτων επίλυσης:

1. Εγκαταστήστε την [επέκταση ασφαλούς](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) προγράμματος περιήγησης "Οι εφαρμογές μου" για να βοηθήσετε το Azure Active Directory (Azure AD) να παρέχει καλύτερες διάγνωση και αναλύσεις κατά τη χρήση της εμπειρίας δοκιμής στην πύλη Azure.
2. Αναπαραγάγετε το σφάλμα χρησιμοποιώντας την εμπειρία δοκιμής στη σελίδα ρύθμισης παραμέτρων εφαρμογής στην πύλη Azure. Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Εντοπισμός σφαλμάτων μεμονωμένων εφαρμογών υπογραφής που βασίζονται σε SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Εάν χρησιμοποιείτε την εμπειρία δοκιμής στην πύλη Azure με την επέκταση ασφαλούς περιήγησης "Οι εφαρμογές μου", μπορείτε να **παραλείψετε το βήμα 4.**
4. Για να ανοίξετε τη σελίδα ρύθμισης παραμέτρων μίας σύνδεσης που βασίζεται σε SAML:
    - Ανοίξτε την [πύλη Azure και](https://portal.azure.com/) συνδεθείτε ως **καθολικός διαχειριστής ή** **διαχειριστής.**
    - Ανοίξτε την **επέκταση της υπηρεσίας καταλόγου Azure Active Directory** **επιλέγοντας όλες τις** υπηρεσίες στο επάνω μέρος του κύριου μενού περιήγησης στα αριστερά.
    - Πληκτρολογήστε "Azure Active Directory" στο πλαίσιο αναζήτησης φίλτρου και επιλέξτε το στοιχείο **του Azure Active Directory.**
    - Επιλέξτε **"Μεγάλες εφαρμογές"** από το αριστερό μενού περιήγησης του Azure Active Directory.
    - Επιλέξτε **"Όλες οι εφαρμογές"** για να δείτε μια λίστα με όλες τις εφαρμογές σας. Εάν δεν βλέπετε την εφαρμογή που θέλετε να  εμφανίζεται εδώ, χρησιμοποιήστε  το στοιχείο ελέγχου  "Φίλτρο" στο επάνω μέρος της λίστας "Όλες οι εφαρμογές" και ορίστε την επιλογή "Εμφάνιση" σε "Όλες **οι εφαρμογές".**
    - Επιλέξτε την εφαρμογή για την οποία θέλετε να ρυθμίσετε τις παραμέτρους για την ενιαία σύνδεση.
    - Μετά τη φόρτωση της εφαρμογής, **επιλέξτε "Μονή σύνδεση"** από το αριστερό μενού περιήγησης της εφαρμογής.
    - Επιλέξτε **SSO που βασίζεται σε SAML.**
5. Ανάλογα με το σφάλμα, για να μάθετε περισσότερα σχετικά με τα συνιστώμενα βήματα που πρέπει να ακολουθήσετε, ανατρέξτε στο θέμα "Προβλήματα κατά την είσοδο σε εφαρμογές με ρυθμισμένες παραμέτρους σύνδεσης που βασίζονται [σε SAML".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Για την αντιμετώπιση προβλημάτων υπογραφής άλλου χρήστη ανατρέξτε στις παρακάτω οδηγίες:
    - [Πρωτόκολλο SAML Sign-On μεμονωμένου Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Οδηγίες: Αντιμετώπιση σφαλμάτων κατά την είσοδο με αναφορές του Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Μη αναμενόμενη προτροπή συγκατάθεσης](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Σφάλμα συγκατάθεσης χρήστη](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Προβλήματα κατά την είσοδο από την εφαρμογή "Οι εφαρμογές μου"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Σφάλμα στη σελίδα σύνδεσης της εφαρμογής](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Πρόβλημα κατά την είσοδο σε μια εφαρμογή της Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
