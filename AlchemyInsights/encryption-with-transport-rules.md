---
title: Κρυπτογράφηση με κανόνες μεταφοράς
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813868"
---
# <a name="encryption-with-transport-rules"></a>Κρυπτογράφηση με κανόνες μεταφοράς

Στο [Κέντρο διαχείρισης του Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), μπορείτε να χρησιμοποιήσετε τις δυνατότητες κρυπτογράφησης μηνυμάτων του Office (OME) στους κανόνες ροής αλληλογραφίας σας, για να ενεργοποιήσετε την κρυπτογράφηση μηνυμάτων. Από τη συνθήκη "Κανόνα μεταφοράς", επιλέξτε την **Εφαρμογή της Κρυπτογράφησης μηνυμάτων του Office 365 και της προστασίας δικαιωμάτων**.

- Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ορισμός κανόνα ροής αλληλογραφίας για κρυπτογράφηση](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Στο PowerShell, χρησιμοποιήστε την εντολή cmdlet [Νέος-ΚανόναςΜεταφοράς](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) και ορίστε την παράμετρο *ApplyOME* στο $true.
