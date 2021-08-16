---
title: Exchange PowerShell και απόσυρση βασικού ελέγχου ταυτότητας
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069244"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell και απόσυρση βασικού ελέγχου ταυτότητας

Για τις πιο πρόσφατες πληροφορίες σχετικά με το πώς μπορείτε να συνδεθείτε στο Exchange Online PowerShell χωρίς τη χρήση Βασικού ελέγχου ταυτότητας, [μεταβείτε εδώ](https://aka.ms/exops-docs). Η λειτουργική μονάδα v2 PowerShell δεν κάνει χρήση βασικού ελέγχου ταυτότητας.

Σημειώστε ότι ο βασικός έλεγχος ταυτότητας εξακολουθεί να πρέπει να είναι ενεργοποιημένος στον υπολογιστή-πελάτη σας.
Η νέα λειτουργική μονάδα v2 PowerShell χρησιμοποιεί τον σύγχρονο έλεγχο ταυτότητας για να δημιουργήσει σύνδεση για την ενεργοποίηση όλων των cmdlet v2 που βασίζονται στο REST. Επιπλέον των cmdlets v2, σάς επιτρέπει να έχετε πρόσβαση σε παλαιότερες cmdlet απομακρυσμένης σύνδεσης PowerShell (RPS) για τα οποία απαιτείται η δημιουργία απομακρυσμένης περιόδου λειτουργίας PowerShell. Η δημιουργία μιας περιόδου λειτουργίας RPS στον υπολογιστή με Windows απαιτεί την ενεργοποίηση του WinRM BasicAuth στον υπολογιστή-πελάτη, παρόλο που η λειτουργική μονάδα χρησιμοποιεί τον σύγχρονο μηχανισμό ελέγχου ταυτότητας για τον έλεγχο ταυτότητας στην υπηρεσία. Η διοχέτευση βασικού ελέγχου ταυτότητας WinRM χρησιμοποιείται για τη μεταφορά διακριτικών σύγχρονου ελέγχου ταυτότητας. Εάν ο βασικός έλεγχος ταυτότητας WinRM έχει απενεργοποιηθεί στον υπολογιστή-πελάτη, τα νέα cmdlets v2 θα συνεχίσουν να λειτουργούν (αλλά οι παλαιότερες cmdlet RPS δεν θα λειτουργούν).
