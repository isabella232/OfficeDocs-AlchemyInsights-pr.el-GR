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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694151"
---
# <a name="fix-transport-rules"></a>Επιδιόρθωση κανόνων μεταφοράς

Ένας προσαρμοσμένος κανόνας ροής αλληλογραφίας επηρέασε αυτό το μήνυμα. Για να εξετάσετε τον ακριβή κανόνα, κάντε τα εξής:

1. Στα αποτελέσματα υποβολής, στην περιοχή **Πρόσθετες πληροφορίες,** σημειώστε το **GUID** ή το **όνομα της πολιτικής.**
2. Εκκινεί το Κέλυφος διαχείρισης Exchange. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Άνοιγμα κελύφους διαχείρισης Exchange".](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Εκτελέστε αυτή την εντολή (χρησιμοποιώντας το GUID από την υποβολή  **σας): Get-TransportRule -identity "GUID" | fl * Περιγραφή***
4. Ελέγξτε την περιγραφή για να δείτε τις ρυθμισμένες συνθήκες που επηρέασαν το μήνυμα.

Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
