---
title: Αντιμετώπιση προβλημάτων μονής σύνδεσης για συσκευές που είναι συνδεδεμένες στο Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039246"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Αντιμετώπιση προβλημάτων μονής σύνδεσης για συσκευές που είναι συνδεδεμένες στο Azure AD

Εάν έχετε ένα περιβάλλον υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης (AD) και θέλετε να συμμετάσχετε στους υπολογιστές που είναι συνδεδεμένοι με τομέα AD στο Azure AD, μπορείτε να το επιτύχετε αυτό κάνοντας υβριδικό σύνδεσμο Azure AD. [Τρόπος: Σχεδιάστε την υβριδική Azure Active Directory σας](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) παρέχει τα σχετικά βήματα για την υλοποίηση ενός υβριδικού συνδέσμου Azure AD στο περιβάλλον σας.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων συσκευών που είναι συνδεδεμένες με το Azure AD για [Single-Sign εσωτερικής εγκατάστασης χρησιμοποιώντας Windows Hello για επιχειρήσεις.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Ζητήματα διακριτικού κύριας ανανέωσης (PRT)**

Το Διακριτικό κύριας ανανέωσης (PRT) είναι ένα βασικό τεχνούργημα του ελέγχου ταυτότητας Azure AD σε συσκευές Windows 10, Windows Server 2016 και νεότερες εκδόσεις, iOS και Android. Πρόκειται για ένα Διακριτικό Web JSON (JWT) που έχει εκδοθεί ειδικά για τους μεσίτες διακριτικών πρώτου μέρους της Microsoft για την ενεργοποίηση της μεμονωμένης εισόδου (SSO) σε όλες τις εφαρμογές που χρησιμοποιούνται σε αυτές τις συσκευές. Για λεπτομέρειες σχετικά με τον τρόπο με τον οποίο εκδίδεται, χρησιμοποιείται και προστατεύεται μια PRT σε Windows 10 συσκευές, ανατρέξτε στο θέμα Τι είναι [το Διακριτικό κύριας ανανέωσης;](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: ΝΑΙ και AzureADPrt: ΝΑΙ**

Αυτά τα πεδία υποδεικνύουν εάν ο χρήστης έχει πραγματοποιήσει επιτυχή έλεγχο ταυτότητας στο Azure AD κατά την είσοδο στη συσκευή. Εάν οι τιμές είναι **NO,** αυτό μπορεί να οφείλεται στα εξής:

- Λάθος κλειδί χώρου αποθήκευσης στο TPM που σχετίζεται με τη συσκευή κατά την καταχώρηση (ελέγξτε το KeySignTest κατά την εκτέλεση αναβαθμισμένων)
- Εναλλακτικό αναγνωριστικό σύνδεσης
- Ο διακομιστής μεσολάβησης HTTP δεν βρέθηκε

Για να αντιμετωπίσετε προβλήματα με συσκευές που χρησιμοποιούν την εντολή dsregcmd, ανατρέξτε [στο θέμα Κατάσταση SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
