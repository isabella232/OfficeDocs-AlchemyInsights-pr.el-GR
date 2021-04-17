---
title: Δεν είναι δυνατή η πρόσβαση σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819512"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Το Outlook δεν μπορεί να συνδεθεί σε δημόσιους φακέλους

Εάν η πρόσβαση σε δημόσιους φακέλους δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:

Συνδεθείτε στο EXO PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στον λογαριασμό χρήστη προβλήματος, ώστε να ταιριάζει με την παράμετρο σε ένα λογαριασμό χρήστη που εργάζεται.

Παράδειγμα:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Περιμένετε τουλάχιστον μία ώρα για να ισχύει η αλλαγή.

Εάν το πρόβλημα παραμένει, ακολουθήστε αυτή τη διαδικασία για [να αντιμετωπίσετε](https://aka.ms/pfcte) προβλήματα πρόσβασης σε δημόσιους φακέλους χρησιμοποιώντας το Outlook.
 
**Για να ελέγξετε ποιοι χρήστες μπορούν να έχουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το Outlook:**

1.  Χρήση Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ή $false  
      
    $true: Να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους στο Outlook  
      
    $false: Αποτρέψτε την πρόσβαση των χρηστών σε δημόσιους φακέλους στο Outlook. Αυτή είναι η προεπιλεγμένη τιμή.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Σημείωση** Αυτή η διαδικασία μπορεί να ελέγξει τις συνδέσεις μόνο με προγράμματα-πελάτες του Outlook για υπολογιστή με Windows. Ένας χρήστης μπορεί να συνεχίσει να έχει πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το OWA ή το Outlook για Mac.
 
Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Ανακοίνωση υποστήριξης για ελεγχόμενες συνδέσεις σε δημόσιους φακέλους" στο Outlook.](https://aka.ms/controlpf)