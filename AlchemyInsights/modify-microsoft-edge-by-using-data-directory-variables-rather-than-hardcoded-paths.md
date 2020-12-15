---
title: Τροποποιήστε το Microsoft Edge χρησιμοποιώντας μεταβλητές καταλόγου δεδομένων αντί για διαδρομές που είναι κωδικοποιημένη
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677989"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Τροποποιήστε το Microsoft Edge χρησιμοποιώντας μεταβλητές καταλόγου δεδομένων αντί για διαδρομές που είναι κωδικοποιημένη

Για παράδειγμα, στα Windows, για να αποθηκεύσετε τα δεδομένα προφίλ στα τοπικά δεδομένα εφαρμογής ενός χρήστη και όχι στην προεπιλεγμένη θέση, ορίστε την πολιτική **UserDataDir** σε **$ {local_app_data} \Edge\Profile**. 

Για να μάθετε περισσότερα, ανατρέξτε στο θέμα [Δημιουργία μεταβλητών καταλόγου δεδομένων χρήστη του Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).