---
title: Single-Sign για Azure Active Directory συνδεδεμένες συσκευές
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050010"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Μονή είσοδος για Azure Active Directory συνδεδεμένες συσκευές

Εάν έχετε ένα περιβάλλον υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης (AD) και θέλετε να συμμετάσχετε στους υπολογιστές που είναι συνδεδεμένοι με τομέα AD στο Azure AD, μπορείτε να το επιτύχετε αυτό κάνοντας υβριδικό σύνδεσμο Azure AD. [Τρόπος: Σχεδιάστε την υβριδική Azure Active Directory σας](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) παρέχει τα σχετικά βήματα για την υλοποίηση ενός υβριδικού συνδέσμου Azure AD στο περιβάλλον σας.

[Ρύθμιση παραμέτρων συσκευών που είναι συνδεδεμένες στο Azure AD για Single-Sign εσωτερικής εγκατάστασης με χρήση Windows Hello για επιχειρήσεις](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Ζητήματα διακριτικού κύριας ανανέωσης (PRT)** Το Διακριτικό κύριας ανανέωσης (PRT) είναι ένα βασικό τεχνούργημα του ελέγχου ταυτότητας Azure AD σε συσκευές Windows 10, Windows Server 2016 και νεότερες εκδόσεις, iOS και Android. Πρόκειται για ένα Διακριτικό Web JSON (JWT) που έχει εκδοθεί ειδικά για τους μεσίτες διακριτικών πρώτου μέρους της Microsoft για την ενεργοποίηση της μεμονωμένης εισόδου (SSO) σε όλες τις εφαρμογές που χρησιμοποιούνται σε αυτές τις συσκευές. [Σε τι είναι το Διακριτικό](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)κύριας ανανέωσης; θα σας παρέχουμε λεπτομέρειες σχετικά με τον τρόπο με τον οποίο εκδίδεται, χρησιμοποιείται και προστατεύεται μια PRT σε Windows 10 σας.

**WamDefaultSet: ΝΑΙ και AzureADPrt: ΝΑΙ** Αυτά τα πεδία υποδεικνύουν εάν ο χρήστης έχει πραγματοποιήσει επιτυχή έλεγχο ταυτότητας στο Azure AD κατά την είσοδο στη συσκευή. Εάν οι τιμές είναι **NO,** αυτό μπορεί να οφείλεται:

- Λάθος κλειδί χώρου αποθήκευσης στο TPM που σχετίζεται με τη συσκευή κατά την εγγραφή (ελέγξτε το KeySignTest ενώ εκτελείται αναβαθμισμένο).
- Εναλλακτικό αναγνωριστικό σύνδεσης
- Ο διακομιστής μεσολάβησης HTTP δεν βρέθηκε

Αντιμετώπιση προβλημάτων συσκευών με χρήση της εντολής dsregcmd - [Κατάσταση SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
