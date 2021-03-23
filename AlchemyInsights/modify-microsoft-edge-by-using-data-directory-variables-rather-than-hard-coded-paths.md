---
title: Τροποποίηση του Microsoft Edge με τη χρήση μεταβλητών καταλόγου δεδομένων και όχι διαδρομών με κώδικα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035817"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Τροποποίηση του Microsoft Edge με τη χρήση μεταβλητών καταλόγου δεδομένων και όχι διαδρομών με κώδικα

Για παράδειγμα, στα Windows, για να αποθηκεύσετε τα δεδομένα προφίλ κάτω από τα δεδομένα τοπικής εφαρμογής ενός χρήστη και όχι στην προεπιλεγμένη θέση, ορίστε την πολιτική *UserDataDir* σε **${local_app_data}\Edge\Profile.**

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Δημιουργία μεταβλητών καταλόγου δεδομένων χρήστη του Microsoft Edge.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)