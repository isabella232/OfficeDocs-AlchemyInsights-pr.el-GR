---
title: Αντιμετώπιση προβλημάτων απλής σύνδεσης (SSO) που βασίζονται σε κωδικό πρόσβασης
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
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972824"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Αντιμετώπιση προβλημάτων απλής σύνδεσης (SSO) που βασίζονται σε κωδικό πρόσβασης

Για να μάθετε τις βασικές αρχές της SSO που βασίζεται σε κωδικό πρόσβασης, ανατρέξτε στο θέμα Έλεγχος ταυτότητας που βασίζεται σε [κωδικό πρόσβασης με Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Ρύθμιση παραμέτρων SSO που βασίζεται σε κωδικό πρόσβασης**

1. [Ρύθμιση παραμέτρων μονής σύνδεσης που βασίζεται](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) σε κωδικό πρόσβασης - Αυτό το άρθρο περιγράφει περισσότερες λεπτομέρειες σχετικά με την επιλογή SSO που βασίζεται σε κωδικό πρόσβασης. Εάν η εφαρμογή που προσθέτετε απαιτεί προσαρμοσμένη ρύθμιση παραμέτρων και πρέπει να χρησιμοποιήσετε SSO που βασίζεται σε κωδικό πρόσβασης, αυτό το άρθρο είναι για εσάς.
2. [Ρύθμιση παραμέτρων μονής σύνδεσης που βασίζεται σε κωδικό πρόσβασης](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) για εφαρμογές εσωτερικής προ-σύνδεσης - Ο διακομιστής μεσολάβησης εφαρμογών υποστηρίζει πολλές λειτουργίες μονής σύνδεσης. Η σύνδεση που βασίζεται σε κωδικό πρόσβασης προορίζεται για εφαρμογές που χρησιμοποιούν συνδυασμό ονόματος χρήστη/κωδικού πρόσβασης για τον έλεγχο ταυτότητας. Όταν ρυθμίζετε τις παραμέτρους της σύνδεσης που βασίζεται σε κωδικό πρόσβασης για την εφαρμογή σας, οι χρήστες σας πρέπει να πραγματοποιήσουν είσοδο στην εφαρμογή εσωτερικής εγκατάστασης μία φορά. Στη συνέχεια, Azure Active Directory αποθηκεύει τις πληροφορίες για την είσοδο και τις παρέχει αυτόματα στην εφαρμογή όταν οι χρήστες έχουν πρόσβαση σε αυτές από απόσταση.
    - Θα πρέπει να έχετε ήδη δημοσιεύσει και να ελέγξετε την εφαρμογή σας με το διακομιστή μεσολάβησης εφαρμογών. Εάν όχι, ακολουθήστε τα βήματα στο πλαίσιο "Δημοσίευση εφαρμογών με χρήση του διακομιστή μεσολάβησης εφαρμογών [Azure AD"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) και, στη συνέχεια, συνεχίστε τη ρύθμιση παραμέτρων SSO που βασίζεται σε κωδικό πρόσβασης για τις εφαρμογές on-prem.

Για την αντιμετώπιση προβλημάτων SSO που βασίζεται σε κωδικό πρόσβασης, ανατρέξτε στο θέμα Αντιμετώπιση προβλημάτων μεμονωμένης [σύνδεσης που βασίζεται σε κωδικό πρόσβασης στο Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
