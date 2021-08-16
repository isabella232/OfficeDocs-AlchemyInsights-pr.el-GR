---
title: Επιδιόρθωση κανόνων μεταφοράς
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034754"
---
# <a name="fix-transport-rules"></a>Επιδιόρθωση κανόνων μεταφοράς

Ένας προσαρμοσμένος κανόνας ροής αλληλογραφίας επηρέασε αυτό το μήνυμα. Για να ελέγξετε τον ακριβή κανόνα, κάντε τα εξής:

1. Στα αποτελέσματα υποβολής, στην περιοχή **Πρόσθετες πληροφορίες,** σημειώστε το **GUID** ή **το όνομα πολιτικής.**
2. Εκκίνηση Exchange κελύφους διαχείρισης. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Άνοιγμα Exchange κελύφους διαχείρισης".](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Εκτελέστε αυτή την εντολή (χρησιμοποιώντας το GUID από την υποβολή σας):  **Get-TransportRule -identity "GUID" | fl * Περιγραφή***
4. Εξετάστε την περιγραφή για να δείτε τις ρυθμισμένες συνθήκες που επηρέασαν το μήνυμα.

Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
