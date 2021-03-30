---
title: Single-Sign για συνδεδεμένες συσκευές Azure Active Directory
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
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405045"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Σύνδεση μίας μόνο υπηρεσίας καταλόγου για συσκευές που είναι συνδεδεμένες στο Azure Active Directory

Εάν έχετε ένα περιβάλλον υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης (AD) και θέλετε να συμμετάσχετε στους υπολογιστές που είναι συνδεδεμένοι με τομέα AD στο Azure AD, μπορείτε να το επιτύχετε αυτό κάνοντας υβριδικό σύνδεσμο Azure AD. [Τρόπος: Ο σχεδιασμός της υβριδικής](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) εφαρμογής συμμετοχής στο Azure Active Directory σάς παρέχει τα σχετικά βήματα για την υλοποίηση ενός υβριδικού συνδέσμου Azure AD στο περιβάλλον σας.

[Ρύθμιση παραμέτρων συσκευών που είναι συνδεδεμένες στο Azure AD για Single-Sign εσωτερικής εγκατάστασης χρησιμοποιώντας το Windows Hello για επιχειρήσεις](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Ζητήματα διακριτικού κύριας ανανέωσης (PRT)** Το Διακριτικό κύριας ανανέωσης (PRT) είναι ένα βασικό τεχνούργημα του ελέγχου ταυτότητας Azure AD σε συσκευές Windows 10, Windows Server 2016 και νεότερες εκδόσεις, iOS και Android. Πρόκειται για ένα Διακριτικό Web JSON (JWT) που έχει εκδοθεί ειδικά για τους μεσίτες διακριτικών πρώτου μέρους της Microsoft για την ενεργοποίηση της μεμονωμένης εισόδου (SSO) σε όλες τις εφαρμογές που χρησιμοποιούνται σε αυτές τις συσκευές. [Σε τι είναι το Διακριτικό](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)κύριας ανανέωσης; Θα σας παρέχουμε λεπτομέρειες σχετικά με τον τρόπο με τον οποίο εκδίδεται, χρησιμοποιείται και προστατεύεται μια PRT σε συσκευές Windows 10.

**WamDefaultSet: ΝΑΙ και AzureADPrt: ΝΑΙ** Αυτά τα πεδία υποδεικνύουν εάν ο χρήστης έχει πραγματοποιήσει επιτυχή έλεγχο ταυτότητας στο Azure AD κατά την είσοδο στη συσκευή. Εάν οι τιμές είναι **NO,** αυτό μπορεί να οφείλεται:

- Λάθος κλειδί χώρου αποθήκευσης στο TPM που σχετίζεται με τη συσκευή κατά την εγγραφή (ελέγξτε το KeySignTest ενώ εκτελείται αναβαθμισμένο).
- Εναλλακτικό αναγνωριστικό σύνδεσης
- Ο διακομιστής μεσολάβησης HTTP δεν βρέθηκε

Αντιμετώπιση προβλημάτων συσκευών με χρήση της εντολής dsregcmd - [Κατάσταση SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
