---
title: Κρυπτογράφηση με κανόνες μεταφοράς
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915179"
---
# <a name="encryption-with-transport-rules"></a>Κρυπτογράφηση με κανόνες μεταφοράς

Στο [Κέντρο διαχείρισης του Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), μπορείτε να χρησιμοποιήσετε τις δυνατότητες κρυπτογράφησης μηνυμάτων του Office (OME) στους κανόνες ροής αλληλογραφίας σας, για να ενεργοποιήσετε την κρυπτογράφηση μηνυμάτων. Από τη συνθήκη "Κανόνα μεταφοράς", επιλέξτε την **Εφαρμογή της Κρυπτογράφησης μηνυμάτων του Office 365 και της προστασίας δικαιωμάτων**.

- Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ορισμός κανόνα ροής αλληλογραφίας για κρυπτογράφηση](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Στο PowerShell, χρησιμοποιήστε την εντολή cmdlet [Νέος-ΚανόναςΜεταφοράς](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) και ορίστε την παράμετρο *ApplyOME* στο $true.
