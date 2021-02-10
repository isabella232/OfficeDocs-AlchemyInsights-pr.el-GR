---
title: Πρόβλημα με τις ομάδες ασφαλείας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177494"
---
# <a name="issue-with-security-groups"></a>Πρόβλημα με τις ομάδες ασφαλείας

**Εάν εμφανίζεται το σφάλμα δικτύου AADDS104**

Οι μη έγκυροι κανόνες ομάδας ασφαλείας δικτύου είναι η πιο συνηθισμένη αιτία σφαλμάτων δικτύου για τις υπηρεσίες τομέα Azure Active Directory (AD DS). Η ομάδα ασφαλείας δικτύου για το εικονικό δίκτυο πρέπει να επιτρέπει την πρόσβαση σε συγκεκριμένες θύρες και πρωτόκολλα. Εάν αυτές οι θύρες έχουν αποκλειστεί, η πλατφόρμα Azure δεν μπορεί να παρακολουθεί ή να ενημερώνει τον διαχειριζόμενο τομέα. Ο συγχρονισμός μεταξύ του Azure AD και του Azure AD DS επίσης επηρεάζει. Βεβαιωθείτε ότι έχετε ανοιχτές τις προεπιλεγμένες θύρες για να αποφύγετε τη διακοπή της υπηρεσίας.

Για να κατανοήσετε και να επιλύσετε συνήθεις ειδοποιήσεις για ζητήματα ρύθμισης παραμέτρων ομάδας ασφαλείας δικτύου, ανατρέξτε στο θέμα ["Προσθήκη και επαλήθευση ομάδων ασφαλείας".](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
