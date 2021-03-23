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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036169"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Αντιμετώπιση προβλημάτων μονής σύνδεσης για συσκευές που είναι συνδεδεμένες στο Azure AD

Εάν έχετε ένα περιβάλλον υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης (AD) και θέλετε να συμμετάσχετε στους υπολογιστές που είναι συνδεδεμένοι με τομέα AD στο Azure AD, μπορείτε να το επιτύχετε αυτό κάνοντας υβριδικό σύνδεσμο Azure AD. [Τρόπος: Ο σχεδιασμός της υβριδικής](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) εφαρμογής συμμετοχής στο Azure Active Directory σάς παρέχει τα σχετικά βήματα για την υλοποίηση ενός υβριδικού συνδέσμου Azure AD στο περιβάλλον σας.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων συσκευών που είναι συνδεδεμένες στο [Azure AD για Single-Sign εσωτερικής εγκατάστασης χρησιμοποιώντας το Windows Hello για επιχειρήσεις.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Ζητήματα διακριτικού κύριας ανανέωσης (PRT)**

Το Διακριτικό κύριας ανανέωσης (PRT) είναι ένα βασικό τεχνούργημα του ελέγχου ταυτότητας Azure AD σε συσκευές Windows 10, Windows Server 2016 και νεότερες εκδόσεις, iOS και Android. Πρόκειται για ένα Διακριτικό Web JSON (JWT) που έχει εκδοθεί ειδικά για τους μεσίτες διακριτικών πρώτου μέρους της Microsoft για την ενεργοποίηση της μεμονωμένης εισόδου (SSO) σε όλες τις εφαρμογές που χρησιμοποιούνται σε αυτές τις συσκευές. Για λεπτομέρειες σχετικά με τον τρόπο με τον οποίο εκδίδεται, χρησιμοποιείται και προστατεύεται μια PRT σε συσκευές Windows 10, ανατρέξτε στο θέμα Τι είναι το [Διακριτικό κύριας ανανέωσης;](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: ΝΑΙ και AzureADPrt: ΝΑΙ**

Αυτά τα πεδία υποδεικνύουν εάν ο χρήστης έχει πραγματοποιήσει επιτυχή έλεγχο ταυτότητας στο Azure AD κατά την είσοδο στη συσκευή. Εάν οι τιμές είναι **NO,** αυτό μπορεί να οφείλεται στα εξής:

- Λάθος κλειδί χώρου αποθήκευσης στο TPM που σχετίζεται με τη συσκευή κατά την καταχώρηση (ελέγξτε το KeySignTest κατά την εκτέλεση αναβαθμισμένων)
- Εναλλακτικό αναγνωριστικό σύνδεσης
- Ο διακομιστής μεσολάβησης HTTP δεν βρέθηκε

Για να αντιμετωπίσετε προβλήματα με συσκευές που χρησιμοποιούν την εντολή dsregcmd, ανατρέξτε [στο θέμα Κατάσταση SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
