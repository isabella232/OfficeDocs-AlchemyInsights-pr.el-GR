---
title: Λύσεις για προβλήματα σχετικά με την εγκατάσταση του office σε έναν Terminal Server
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: 28ebe2b1375b142ca63dc686c7afbbe88abfd539a93780cff3861f80de40b411
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021848"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a>Λύσεις για προβλήματα σχετικά με την εγκατάσταση του office σε έναν Terminal Server

Για να χρησιμοποιήσετε την ενεργοποίηση κοινόχρηστου υπολογιστή, πρέπει να έχετε μια συνδρομή που περιλαμβάνει Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.
  
- Επαλήθευση ότι η ενεργοποίηση κοινόχρηστου υπολογιστή είναι ενεργοποιημένη
- Επαλήθευση ότι η ενεργοποίηση ολοκληρώθηκε με επιτυχία
- Εξετάστε τα μηνύματα σφάλματος για την ενεργοποίηση κοινόχρηστου υπολογιστή:
- "Τα προϊόντα που βρέθηκαν στο λογαριασμό σας δεν μπορούν να χρησιμοποιηθούν για την ενεργοποίηση Office σε σενάρια κοινόχρηστου υπολογιστή"
  
Αυτό το σφάλμα σημαίνει ότι δεν έχετε συνδρομή που να περιλαμβάνει Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.

"Προϊόν χωρίς άδεια άδειας"

- Ελέγξτε ότι στο χρήστη έχει εκχωρηθεί μια άδεια χρήσης για Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.
- Ελέγξτε ότι ο χρήστης έχει κάνει check-in με το λογαριασμό χρήστη του.
- Ελέγξτε ότι υπάρχει σύνδεση μεταξύ του κοινόχρηστου υπολογιστή και του Internet.

Για άλλες συμβουλές αντιμετώπισης προβλημάτων, ανατρέξτε στο θέμα: [Αντιμετώπιση προβλημάτων με την ενεργοποίηση κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)