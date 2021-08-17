---
title: Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105750"
---
# <a name="troubleshoot-password-synchronization"></a>Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης

Για να αντιμετωπίσετε προβλήματα συγχρονισμού κωδικών πρόσβασης, ξεκινήστε χρησιμοποιώντας αυτή την εργασία Σύνδεση AAD για να προσδιορίσετε γιατί δεν συγχρονίζονται οι κωδικοί πρόσβασης. Για να ξεκινήσετε, μεταβείτε στην [επιλογή Διαχείριση άμεσου συγχρονισμού.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Ανοίξτε μια νέα Windows PowerShell στο διακομιστή Azure AD Σύνδεση και επιλέξτε "Εκτέλεση **ως διαχειριστής".**

2. Εκτελέστε Set-ExecutionPolicy απομακρυσμένης υπογραφής Set-ExecutionPolicy χωρίς έλεγχο.

3. Ξεκινήστε τον οδηγό Σύνδεση Azure AD.

4. Μεταβείτε στη σελίδα "Πρόσθετες εργασίες" > **"Αντιμετώπιση προβλημάτων**  >  **στο επόμενο".**

5. Επιλέξτε **"Εκκίνηση"** για να ανοίξετε το μενού αντιμετώπισης προβλημάτων του PowerShell.

6. Επιλέξτε **"Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης".**

    Το πρόβλημα είναι συνήθως ότι ένας κωδικός πρόσβασης δεν συγχρονίζεται για ένα συγκεκριμένο λογαριασμό χρήστη.

    **Σημειώσεις** Ο συγχρονισμός κωδικού πρόσβασης αποτυγχάνει εάν ο τελευταίος επιτυχημένος συγχρονισμός κωδικού πρόσβασης ήταν πριν από κάποιο χρονικό διάστημα.

Για περισσότερη βοήθεια σχετικά με την αντιμετώπιση προβλημάτων συγχρονισμού κωδικών πρόσβασης, ανατρέξτε στο θέμα Αντιμετώπιση προβλημάτων συγχρονισμού [hash κωδικού πρόσβασης με το Azure AD Σύνδεση συγχρονισμού.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)