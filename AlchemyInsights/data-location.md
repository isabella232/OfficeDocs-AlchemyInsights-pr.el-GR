---
title: Θέση δεδομένων
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655282"
---
# <a name="data-location"></a>Θέση δεδομένων

Μπορείτε να προβάλετε τη θέση του μισθωτή σας στο κέντρο διαχείρισης ή συνδέοντας στο Exchange Online μέσω του PowerShell.


**Κέντρο διαχείρισης:**
1. Συνδεθείτε στο [κέντρο διαχείρισης](https://admin.microsoft.com/Adminportal/Home).
2. Επιλέξτε**προφίλ οργάνωσης** **ρυθμίσεων** > .
3. Στην περιοχή **Θέση δεδομένων**, επιλέξτε **Προβολή λεπτομερειών**.


**Powershell:**
1. Συνδεθείτε στο Exchange Online χρησιμοποιώντας το Windows PowerShell.
2. Εκτελέστε το cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) για να εμφανίσετε μια λίστα με τις ιδιότητες του μισθωτή σας. 
3. Κοιτάξτε την ιδιότητα OrganizationId.

Όταν έχετε τη θέση δεδομένων για EXO και SPO, μπορείτε να προσδιορίσετε τη θέση δεδομένων για άλλες υπηρεσίες που μπορείτε να χρησιμοποιήσετε από [το σημείο όπου βρίσκονται τα δεδομένα σας](https://products.office.com/where-is-your-data-located).