---
title: Δεν είναι δυνατή η πρόσβαση σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891749"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Το Outlook δεν είναι δυνατό να συνδεθεί με δημόσιους φακέλους

Εάν η πρόσβαση σε δημόσιους φακέλους δεν λειτουργεί για ορισμένους χρήστες, δοκιμάστε τα εξής:

Συνδεθείτε με το EXO PowerShell και ρυθμίστε τις παραμέτρους της παραμέτρου DefaultPublicFolderMailbox στο λογαριασμό χρήστη προβλήματος, ώστε να ταιριάζει με την παράμετρο σε ένα λογαριασμό χρήστη που λειτουργεί.

Παράδειγμα:

Λειτουργικός χρήστης του γραμματοκιβωτίου get | ft προεπιλεγμένοδημόσιο φάκελογραμματοκιβώτιο, αποτελεσματικόδημόσιο φάκελογραμματοκιβώτιο

Set-Γραμματοκιβώτιο ProblemUser -Προεπιλεγμένη τιμήδημόσιου φακέλουΓραμματοκιβώτιο \<από την προηγούμενη εντολή>

Περιμένετε τουλάχιστον μία ώρα για να εφαρμοστεί η αλλαγή.

Εάν το ζήτημα παραμένει, ακολουθήστε [αυτήν τη διαδικασία](https://aka.ms/pfcte) για να αντιμετωπίσετε ζητήματα πρόσβασης σε δημόσιους φακέλους χρησιμοποιώντας το Outlook.