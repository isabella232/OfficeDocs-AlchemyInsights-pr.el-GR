---
title: Εισαγωγή και εξαγωγή από Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036126"
---
# <a name="import-and-export-from-yammer"></a>Εισαγωγή και εξαγωγή από Yammer

**Εισαγωγή**

Οι επιλογές εισαγωγής χρήστη διαφέρουν ανάλογα με το εάν το Yammer σας βρίσκεται σε [εγγενή λειτουργία για το Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ή όχι.

- **Μη εγγενής λειτουργία:** Οι χρήστες μπορούν να εισαχθούν σε ομάδες χρησιμοποιώντας την επιλογή ["Προσθήκη](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) από βιβλίο διευθύνσεων" (όριο σε 100 χρήστες) στις ρυθμίσεις ομάδας ή στο δίκτυο χρησιμοποιώντας [τη Μαζική ενημέρωση](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) μέσα από το διαχειριστή δικτύου.
- **Εγγενής λειτουργία:** Οι λειτουργίες ιδιότητας μέλους ομάδας και μέλους δικτύου θα πρέπει να εκτελούνται από την πύλη διαχείρισης [Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users)την πύλη [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ή χρησιμοποιώντας μια άλλη επιλογή Azure AD. Τα δίκτυα στην εγγενή λειτουργία δεν έχουν πλέον πρόσβαση στη Μαζική ενημέρωση και σε άλλες δυνατότητες παλαιού τύπου.

> [!IMPORTANT]
> Yammer υποστηρίζεται η εισαγωγή περιεχομένου από το διαχειριστή δικτύου, ακόμα και όταν η δυνατότητα εξαγωγής δεδομένων χρησιμοποιήθηκε σε άλλο δίκτυο. Το περιεχόμενο μπορεί να δημοσιευτεί εκ Yammer λύσεων συνεργατών.

**Εξαγωγή**

[Η εξαγωγή δεδομένων δικτύου μέσα από το διαχειριστή](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) δικτύου επιτρέπει την εξαγωγή περιεχομένου από Yammer δίκτυα, συμπεριλαμβανομένων των μηνυμάτων και των αρχείων. Τα συνημμένα μπορεί να είναι εξαιρετικά μεγάλα και θα προκαλέσουν την ολοκλήρωση των εξαγωγών. Συνιστάται η εξαγωγή ενεργών δικτύων με χρήση του [API εξαγωγής δεδομένων](https://developer.yammer.com/docs/data-export-api) σε μπλοκ ανά ημέρα ή εβδομάδα. Η Υποστήριξη της Microsoft δεν παρέχει προσαρμοσμένες δέσμες ενεργειών για το σκοπό αυτό.

Μια ξεχωριστή [εξαγωγή ΓΚΠΔ](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) υπάρχει για την εξαγωγή περιεχομένου για έναν μεμονωμένο χρήστη.