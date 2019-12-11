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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959495"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Δεν είναι δυνατή η σύνδεση του Outlook με δημόσιους φακέλους

Εάν η πρόσβαση σε δημόσιους φακέλους δεν λειτουργεί για λίγους χρήστες, δοκιμάστε τα εξής:

Σύνδεση με εξω PowerShell και ρυθμίστε τις παραμέτρους του γραμματοκιβωτίου Προεπιλεγήςφάκελος στο λογαριασμό χρήστη του προβλήματος για να ταιριάζει με μία σε ένα λογαριασμό χρήστη που λειτουργεί.

Παράδειγμα:

Λήψη-γραμματοκιβώτιο WorkingUser | Γραμματοκιβωτίου EffectivePublicFolderMailbox

Set-γραμματοκιβώτιο Πρόβλήσενος χρήστη προεπιλεγμένη τιμή γραμματοκιβωτίου \<από την προηγούμενη εντολή>

Περιμένετε τουλάχιστον μία ώρα για να τεθεί σε ισχύ η αλλαγή.