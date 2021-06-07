---
title: Προβλήματα επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793757"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Προβλήματα επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux

Αυτό το άρθρο σάς καθοδηγεί στα βήματα για τον προσδιορισμό ζητημάτων επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux.

Είναι σημαντικό να επαληθεύσετε πρώτα ότι το πρόβλημα που αντιμετωπίζετε έχει επιλυθεί με την [πιο πρόσφατη έκδοση.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Για να ξεκινήσετε την έρευνα, ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Εξαιρέσεις

Οι εξαιρέσεις μπορούν να σας βοηθήσουν να μετριάσουν τα προβλήματα επιδόσεων. Ελέγξτε τις εξαιρέσεις σας πριν ξεκινήσετε, ώστε να είναι γνωστός και τεκμηριωμένος οποιοσδήποτε πρόσθετος κίνδυνος.

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για το Microsoft Defender για τελικό σημείο σε Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Όταν έχετε πολλά αρχεία που & να εξαιρέσετε και βρίσκονται όλα στο ίδιο σημείο τοποθέτησης, ίσως είναι ευκολότερο να εξαιρέσετε το σημείο τοποθέτησης. Ξεκινώντας από την έκδοση 101.22.80 του Φεβρουαρίου, μπορείτε να εξαιρέσετε ένα ολόκληρο σημείο τοποθέτησης.

Για παράδειγμα, εάν το /mnt/backup είναι ένα σημείο τοποθέτησης, μπορείτε να προσθέσετε /mnt/backup στη λίστα εξαιρέσεων εκτελώντας αυτή την εντολή:

`$ mdatp exclusion folder add –path /mnt/backup`

**Σημείωση:** Η προσθήκη εξαιρέσεων αυξάνει τον κίνδυνο να μην εντοπιστεί λογισμικό κακόβουλης λειτουργίας και θα πρέπει να γίνεται χειρισμός και να εφαρμόζεται με προσοχή.

## <a name="need-help"></a>Χρειάζεστε βοήθεια;

Για να σας βοηθήσει με τον πιο αποτελεσματικό τρόπο, συλλέξτε τα διαγνωστικά δεδομένα πριν ανοίξετε μια υπόθεση υποστήριξης.
