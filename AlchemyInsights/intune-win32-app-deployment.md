---
title: Ανάπτυξη εφαρμογών Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461796"
---
# <a name="intune-win32-app-deployment"></a>Ανάπτυξη εφαρμογών Intune Win32

Το Microsoft Intune επιτρέπει τις εφαρμογές Win32, συμπεριλαμβανομένων, ενδεικτικά, του MSI και του. Το EXE θα αναπτυχθεί σε συσκευές με Windows 10. Ο μηχανισμός ανάπτυξης που χρησιμοποιείται απαιτεί την επέκταση διαχείρισης Intune (IME) να υπάρχει στη συσκευή προορισμού. Το IME θα εγκατασταθεί αυτόματα ως αποτέλεσμα της στόχευσης μιας δέσμης ενεργειών PowerShell ή μιας ανάπτυξης εφαρμογών Win32 σε ένα χρήστη/συσκευή.

Υπάρχουν επίσης ορισμένα προαπαιτούμενα που πρέπει να πληρούνται προκειμένου να αναπτυχθούν εφαρμογές Win32 που περιλαμβάνουν:

- Υποστηριζόμενες πλατφόρμες: Windows 10 έκδοση 1607 ή νεότερη έκδοση (εκδόσεις Enterprise, Pro και Education).
- Υποστηριζόμενη αρχιτεκτονική: x86 και x64.
- Διαχείριση συσκευών: AAD και αυτόματη εγγραφή (συμπεριλαμβανομένων των υβριδικών τομέων που είναι συνδεδεμένοι και της πολιτικής ομάδας που έχουν εγγραφεί αυτόματα).
- Μορφή πακέτου εφαρμογής:. αρχείο **intunewin**  που εκπονήθηκε από το [εργαλείο προετοιμασίας περιεχομένου του Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Περιορισμοί
    - Μέγιστο μέγεθος: 8GB.
    - Μη υποστηριζόμενη αρχιτεκτονική: όπλα.

Εξετάστε το έγγραφο "[Προσθήκη, εκχώρηση και παρακολούθηση μιας εφαρμογής Win32 στο Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" για πληροφορίες σχετικά με αυτά τα βήματα.

Λεπτομέρειες σχετικά με την αντιμετώπιση προβλημάτων ανάπτυξης εφαρμογών στα Windows, συμπεριλαμβανομένων των εφαρμογών Win32, μπορούν να αναθεωρηθούν στα ακόλουθα έγγραφα

- [Αντιμετώπιση προβλημάτων εγκατάστασης εφαρμογών](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Αντιμετώπιση προβλημάτων εφαρμογών Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)