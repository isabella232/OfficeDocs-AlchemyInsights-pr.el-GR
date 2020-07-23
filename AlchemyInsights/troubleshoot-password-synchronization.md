---
title: Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387877"
---
# <a name="troubleshoot-password-synchronization"></a>Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης

Για να αντιμετωπίσετε προβλήματα συγχρονισμού κωδικού πρόσβασης, ξεκινήστε χρησιμοποιώντας αυτήν την εργασία αντιμετώπισης προβλημάτων AAD Connect για να προσδιορίσετε γιατί οι κωδικοί πρόσβασης δεν συγχρονίζονται. Για να ξεκινήσετε, μεταβείτε στην ενότητα [Διαχείριση άμεσου συγχρονισμού](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Ανοίξτε μια νέα περίοδο λειτουργίας του Windows PowerShell στο διακομιστή Azure AD Connect και ενεργοποιήστε την επιλογή **Εκτέλεση ως διαχειριστής.**

2. Εκτελέστε το Set-ExecutionPolicy RemoteSigned ή Set-ExecutionPolicy Χωρίς περιορισμούς.

3. Ξεκινήστε τον "Οδηγό σύνδεσης Azure AD".

4. Μεταβείτε στη σελίδα "Πρόσθετες εργασίες" > **Αντιμετώπιση προβλημάτων**  >  **στο επόμενο**.

5. Επιλέξτε **Εκκίνηση** για να ανοίξετε το μενού αντιμετώπισης προβλημάτων του PowerShell.

6. Επιλέξτε **Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης**.

    Το ζήτημα είναι συνήθως ότι ένας κωδικός πρόσβασης δεν συγχρονίζεται για ένα συγκεκριμένο λογαριασμό χρήστη.

    **Σημειώσεις** Ο συγχρονισμός κωδικού πρόσβασης αποτυγχάνει εάν ο τελευταίος επιτυχής συγχρονισμός κωδικού πρόσβασης ήταν πριν από λίγο καιρό.

Για περισσότερη βοήθεια σχετικά με την αντιμετώπιση του συγχρονισμού κωδικών πρόσβασης, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων συγχρονισμού κατακερματισμού κωδικού πρόσβασης με το συγχρονισμό Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).