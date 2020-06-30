---
title: Πρόσβαση υπό όρους με το Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931430"
---
# <a name="conditional-access-with-intune"></a>Πρόσβαση υπό όρους με το Intune

Η χρήση **της πρόσβασης υπό όρους** με το Intune απαιτεί 3 βήματα:

- Δημιουργήστε μια **πολιτική συμμόρφωσης** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) για να ορίσετε τις ρυθμίσεις που πρέπει να πληρούνται πριν η συσκευή θεωρείται συμβατή. Για παράδειγμα, μια συσκευή πρέπει να έχει μια ακίδα τουλάχιστον 6 ψηφίων πριν θεωρηθεί συμβατή.
- Δημιουργήστε μια **πολιτική πρόσβασης υπό όρους** που καθορίζει τους πόρους που προστατεύονται και ποιες προϋποθέσεις πρέπει να πληρούνται για την πρόσβαση σε αυτούς τους πόρους.  [Για παράδειγμα,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) μια συσκευή πρέπει να είναι συμβατή πριν από την πρόσβαση σε εταιρικό ηλεκτρονικό ταχυδρομείο.
- Βεβαιωθείτε ότι τόσο οι **πολιτικές συμμόρφωσης** όσο και οι **πολιτικές πρόσβασης υπό όρους** στοχεύουν στις επιθυμητές ομάδες χρηστών. Αυτό μπορεί να απαιτεί τη δημιουργία συγκεκριμένων ομάδων χρηστών στην υπηρεσία καταλόγου Azure Active Directory.

**Χρήσιμες συνδέσεις:**

[Επισκόπηση συμμόρφωσης συσκευής](https://docs.microsoft.com/intune/device-compliance-get-started)

[Αντιμετώπιση προβλημάτων αρχής έκδοσης πιστοποιητικών](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Πολιτική αντιμετώπισης προβλημάτων](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Για να προστατεύσετε το ηλεκτρονικό ταχυδρομείο (Exchange online) από την πρόσβαση από μη συμβατές συσκευές, πρέπει να ακολουθούνται και τα δύο έγγραφα:

1. [Προστασία πρόσβασης ηλεκτρονικού ταχυδρομείου από συσκευές που χρησιμοποιούν EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Προστασία πρόσβασης ηλεκτρονικού ταχυδρομείου από συσκευές που χρησιμοποιούν σύγχρονα προγράμματα-πελάτες ελέγχου ταυτότητας, όπως το Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)