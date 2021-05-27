---
title: Κανόνες μείωσης επιφάνειας επίθεσης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676231"
---
# <a name="attack-surface-reduction-rules"></a>Κανόνες μείωσης επιφάνειας επίθεσης

Η εξαίρεση αρχείων ή φακέλων μπορεί να μειώσει σημαντικά την προστασία που παρέχεται από τους κανόνες μείωσης επιφάνειας επίθεσης. Τα αρχεία που θα είχαν αποκλειστεί από έναν κανόνα επιτρέπεται να εκτελούνται και δεν καταγράφεται αναφορά ή συμβάν. Μια εξαίρεση ισχύει για όλους τους κανόνες που επιτρέπουν εξαιρέσεις.

Οι εξαιρέσεις ASR χρησιμοποιούν την ίδια σύνταξη με Προστασία του Microsoft Defender από ιούς εξαιρέσεων. Για λεπτομέρειες, ανατρέξτε [στο θέμα Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για Προστασία του Microsoft Defender από ιούς σαρώσεις.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Για να αποφύγετε προβλήματα, εξετάστε [τα κοινά λάθη για να αποφύγετε κατά τον ορισμό εξαιρέσεων.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Δεν υποστηρίζουν όλοι οι κανόνες ASR τις εξαιρέσεις. Για να επαληθεύσετε εάν ο κανόνας σας υποστηρίζει εξαιρέσεις, ανατρέξτε στον πίνακα [Κανόνες μείωσης επιφάνειας επίθεσης.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Κανόνες μείωσης επιφάνειας επίθεσης

Η επιφάνεια επίθεσης του οργανισμού σας περιλαμβάνει όλα τα σημεία όπου ένας εισβολέας θα μπορούσε να θέσει σε κίνδυνο τις συσκευές ή τα δίκτυα του οργανισμού. Η μείωση της επιφάνειας της επίθεσης σημαίνει ότι προστατεύετε τις συσκευές και το δίκτυο της εταιρείας, γεγονός που αφήνει τους επιτιθέμενους με λιγότερους τρόπους για να εκτελέσουν επιθέσεις. Η ρύθμιση παραμέτρων των κανόνων μείωσης επιφάνειας επίθεσης στο Microsoft Defender για το τελικό σημείο μπορεί να σας βοηθήσει.

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

- [Αντιστοίχιση GUID κανόνα ASR με όνομα](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Απαιτήσεις κανόνων ASR:
    - [Windows 10 Pro, έκδοση 1709 ή νεότερη](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, έκδοση 1709 ή νεότερη](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Διακομιστής, έκδοση 1803 (Εξαμηνιό κανάλι) ή νεότερη](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Προσδιορισμός της σωστής εξαίρεσης που θα εφαρμοστεί

1. Αναζητήστε το eventID 1121 ή 1122 στο αρχείο καταγραφής microsoft-Windows-Windows Defender/Λειτουργικό αρχείο καταγραφής.

1. Αξιολογήστε το σενάριο αποκλεισμού και το περιβάλλον και επιβεβαιώστε ότι αυτό το σενάριο πρέπει να ξεμπλοκάρει.

1. Διαβάστε την τιμή "Διαδρομή" στις λεπτομέρειες του συμβάντος, η οποία είναι η τιμή που καθορίζει την εξαίρεση.
    - Κάντε την εξαίρεση όσο το δυνατόν πιο αυστηρή.
    - Εφαρμόστε έναν χαρακτήρες μπαλαντέρ όπου χρειάζεται (για παράδειγμα, αντικατάσταση μεταβλητής χρήστη).

1. Εφαρμόστε την εξαίρεση σύμφωνα με τις ανάγκες ανάπτυξης. Για λεπτομέρειες, ανατρέξτε στο θέμα [Προσαρμογή κανόνων μείωσης επιφάνειας επίθεσης.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Ο αποκλεισμός δεν τιμάται

1. Προσδιορίστε εάν ο κανόνας υποστηρίζει εξαιρέσεις. Για λεπτομέρειες, ανατρέξτε στο [θέμα Κανόνες μείωσης επιφάνειας επίθεσης.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Εξετάστε τις εξαιρέσεις που εφαρμόστηκαν και επαληθεύστε με τα δεδομένα συμβάντος για λάθη ή εσφαλμένους χαρακτήρες μπαλαντέρ. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Υποστηριζόμενοι τύποι αποκλεισμού](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Εάν η επίδραση του κανόνα είναι πολύ υψηλή, εξετάστε το ενδεχόμενο να μετακινήσετε τον κανόνα (πίσω) σε λειτουργία ελέγχου για να εκτελέσετε περαιτέρω επικύρωση. Για λεπτομέρειες, ανατρέξτε [στο θέμα Έλεγχος του τρόπου λειτουργίας των δυνατοτήτων του Microsoft Defender για τελικά σημεία σε λειτουργία ελέγχου.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Συλλέξτε δεδομένα υποστήριξης για να ανοίξετε μια υπόθεση υποστήριξης χρησιμοποιώντας αυτή την εντολή:
    
   ** MDEClientAnalyzer.cmd -v**

    Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Θέματα σχετικά με τους υπολογιστές με [πίνακες στο Microsoft Defender για τελικά σημεία.](issues-with-onboarding-machines.md)
