---
title: Οι πολιτικές διατήρησης Exchange κέντρο διαχείρισης δεν λειτουργούν
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074932"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Πολιτικές διατήρησης στο Exchange Διαχείρισης

Εάν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί "Πίσω" <-- στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που έχει προβλήματα με τις πολιτικές διατήρησης.

Εάν έχετε προβλήματα με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης Exchange δεν ισχύουν για γραμματοκιβώτια ή στοιχεία που δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης, ελέγξτε τα εξής:

**Ριζικές αιτίες:**

- **Ο Βοηθός διαχειριζόμενων** φακέλων δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη. Ο Βοηθός διαχειριζόμενων φακέλων προσπαθεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες.

  **Λύση:** Εκτελέστε τον Βοηθό διαχείρισης φακέλων.

- **Το RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο. Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία κατά τη διάρκεια αυτής της περιόδου.

  **Λύση:** Ελέγξτε την κατάσταση της ρύθμισης διατήρησης και της ενημέρωσης, όπως απαιτείται. Για λεπτομέρειες, ανατρέξτε στο [θέμα Διατήρηση γραμματοκιβωτίου](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο Βοηθός διαχειριζόμενων φακέλων δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.
 
Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο Exchange Διαχείρισης, ανατρέξτε στα θέμα:

- [Ετικέτες διατήρησης και πολιτικές διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια ή προσθήκη](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [ή κατάργηση ετικετών διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Τρόπος αναγνώρισης του τύπου διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
