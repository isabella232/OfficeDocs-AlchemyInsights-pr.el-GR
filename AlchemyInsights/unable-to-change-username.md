---
title: Δεν είναι δυνατή η αλλαγή του ονόματος χρήστη
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439553"
---
# <a name="unable-to-change-username"></a>Δεν είναι δυνατή η αλλαγή του ονόματος χρήστη

Σε ορισμένες περιπτώσεις, οι αλλαγές UPN (UserPrincipalName) δεν μεταδίδονται στο cloud. Ενδέχεται να λάβετε σφάλματα επικύρωσης στην πύλη του Office 365 ή να μην μπορείτε να αλλάξετε το όνομα χρήστη ή τη διεύθυνση ηλεκτρονικού ταχυδρομείου. Για να επιλύσετε αυτό το ζήτημα, ορίστε με μη αυτόματο τρόπο το UserPrincipalName χρησιμοποιώντας αυτήν την εντολή PowerShell.

**Παράδειγμα: Μετονομασία χρήστη**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Αυτή η εντολή μετονομάζει davidc@contoso.com σε davidchew@contoso.com.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).