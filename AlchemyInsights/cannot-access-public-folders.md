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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996630"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook να συνδεθείτε σε δημόσιους φακέλους

Εάν η πρόσβαση σε δημόσιους φακέλους δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:

Σύνδεση στο EXO PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στο λογαριασμό χρήστη προβλήματος, ώστε να ταιριάζει με την παράμετρο σε ένα λογαριασμό χρήστη που λειτουργεί.

Παράδειγμα:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Περιμένετε τουλάχιστον μία ώρα για να ισχύει η αλλαγή.

Εάν το πρόβλημα παραμένει, ακολουθήστε αυτή τη διαδικασία για [να αντιμετωπίσετε](https://aka.ms/pfcte) προβλήματα πρόσβασης σε δημόσιους φακέλους χρησιμοποιώντας Outlook.
 
**Για να ελέγξετε ποιοι χρήστες μπορούν να αποκτήσουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας Outlook:**

1.  Χρήση Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ή $false  
      
    $true: Να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους Outlook  
      
    $false: Αποτρέψτε την πρόσβαση των χρηστών σε δημόσιους φακέλους Outlook. Αυτή είναι η προεπιλεγμένη τιμή.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Σημείωση** Αυτή η διαδικασία μπορεί να ελέγξει τις συνδέσεις μόνο με Outlook υπολογιστή για Windows υπολογιστές-πελάτες. Ένας χρήστης μπορεί να συνεχίσει να έχει πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το OWA ή Outlook για Mac.
 
Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Ανακοίνωση υποστήριξης για ελεγχόμενες συνδέσεις σε δημόσιους φακέλους" Outlook.](https://aka.ms/controlpf)