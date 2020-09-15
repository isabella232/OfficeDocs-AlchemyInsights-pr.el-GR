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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664926"
---
# <a name="troubleshoot-password-synchronization"></a>Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης

Για να αντιμετωπίσετε προβλήματα συγχρονισμού κωδικών πρόσβασης, ξεκινήστε χρησιμοποιώντας αυτήν την εργασία αντιμετώπισης προβλημάτων του AAD Connect για να προσδιορίσετε γιατί οι κωδικοί πρόσβασης δεν συγχρονίζονται. Για να ξεκινήσετε, μεταβείτε στη [Διαχείριση άμεσου συγχρονισμού](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Ανοίξτε μια νέα περίοδο λειτουργίας του Windows PowerShell στο διακομιστή Azure AD Connect και επιλέξτε την επιλογή **Εκτέλεση ως διαχειριστής** .

2. Εκτελέστε την ExecutionPolicy RemoteSigned ή τον ορισμό ExecutionPolicy χωρίς περιορισμούς.

3. Ξεκινήστε τον Οδηγό σύνδεσης Azure AD.

4. Μεταβείτε στη σελίδα πρόσθετες εργασίες > **αντιμετωπίσετε**το  >  **Επόμενο**θέμα.

5. Επιλέξτε **εκκίνηση** για να ανοίξετε το μενού αντιμετώπισης προβλημάτων του PowerShell.

6. Επιλέξτε **Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης**.

    Το πρόβλημα συνήθως είναι ότι δεν έχει συγχρονιστεί ένας κωδικός πρόσβασης για έναν συγκεκριμένο λογαριασμό χρήστη.

    **Σημειώσεις** Ο συγχρονισμός κωδικού πρόσβασης αποτυγχάνει εάν ο τελευταίος επιτυχημένος συγχρονισμός κωδικού πρόσβασης ήταν πριν από λίγο καιρό.

Για περισσότερη βοήθεια σχετικά με την αντιμετώπιση προβλημάτων συγχρονισμού κωδικών πρόσβασης, ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων συγχρονισμού κατακερματισμού κωδικού πρόσβασης με το Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).