---
title: Δεν είναι δυνατή η πρόσβαση σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812547"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Το Outlook δεν μπορεί να συνδεθεί με δημόσιους φακέλους

Εάν η πρόσβαση στο δημόσιο φάκελο δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:

Συνδεθείτε στο έξω PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στο λογαριασμό χρήστη του προβλήματος ώστε να ταιριάζει με την παράμετρο σε έναν λογαριασμό χρήστη που λειτουργεί.

Παράδειγμα

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Ορίστε-γραμματοκιβώτιο ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Περιμένετε τουλάχιστον μία ώρα για να ισχύσει η αλλαγή.

Εάν το πρόβλημα παραμένει, ακολουθήστε [αυτή τη διαδικασία](https://aka.ms/pfcte) για την αντιμετώπιση προβλημάτων πρόσβασης δημόσιου φακέλου με χρήση του Outlook.
 
**Για να ελέγξετε ποιοι χρήστες μπορούν να έχουν πρόσβαση σε δημόσιους φακέλους με χρήση του Outlook**:

1.  Χρήση του συνόλου-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE ή $FALSE  
      
    $true: να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους στο Outlook  
      
    $false: αποτροπή πρόσβασης χρηστών σε δημόσιους φακέλους στο Outlook. Αυτή είναι η προεπιλεγμένη τιμή.  
        
2.  Ορίστε-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Σημείωση** Αυτή η διαδικασία μπορεί να ελέγχει τις συνδέσεις μόνο με το Outlook για υπολογιστές-πελάτες των Windows. Ένας χρήστης μπορεί να συνεχίσει την πρόσβαση σε δημόσιους φακέλους με χρήση του OWA ή του Outlook για Mac.
 
Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα ανακοίνωση υποστήριξης για ελεγχόμενες συνδέσεις σε δημόσιους φακέλους στο Outlook](https://aka.ms/controlpf).