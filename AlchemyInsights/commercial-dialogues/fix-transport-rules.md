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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746738"
---
# <a name="fix-transport-rules"></a>Επιδιόρθωση κανόνων μεταφοράς

Ένας προσαρμοσμένος κανόνας ροής αλληλογραφίας επηρέασε αυτό το μήνυμα. Για να ελέγξετε τον ακριβή κανόνα, κάντε τα εξής:

1. Στα αποτελέσματα υποβολής, στην περιοχή **Πρόσθετες πληροφορίες,** σημειώστε το **GUID** ή **το όνομα πολιτικής.**
2. Εκκινεί το κέλυφος διαχείρισης του Exchange. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Άνοιγμα του κελύφους διαχείρισης του Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Εκτελέστε αυτή την εντολή (χρησιμοποιώντας το GUID από την υποβολή σας):  **Get-TransportRule -identity "GUID" | fl * Περιγραφή***
4. Εξετάστε την περιγραφή για να δείτε τις ρυθμισμένες συνθήκες που επηρέασαν το μήνυμα.

Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
