---
title: Το εικονίδιο ημερολογίου δεν εμφανίζεται στο Microsoft Teams πελάτη
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120004"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Το εικονίδιο ημερολογίου δεν εμφανίζεται στο Microsoft Teams πελάτη

Η **καρτέλα "Ημερολόγιο"** Teams απαιτεί πρόσβαση σε ένα γραμματοκιβώτιο Exchange μέσω Exchange Web Services. Το Exchange μπορεί να είναι online ή εσωτερικής εγκατάστασης. Για τους χρήστες στο  Internet που δεν βλέπουν την καρτέλα "Ημερολόγιο", βεβαιωθείτε ότι έχουν άδεια χρήσης για [ένα γραμματοκιβώτιο Exchange Online και ότι το γραμματοκιβώτιο είναι ενεργοποιημένο.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Εάν οι χρήστες σας είναι οικιακοί χρήστες εσωτερικής εγκατάστασης, πρέπει να επιβεβαιώσετε ότι η υβριδική ρύθμιση παραμέτρων είναι σε καλή κατάσταση. Χρησιμοποιήστε τον [Οδηγό υβριδικής ρύθμισης παραμέτρων](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) για να αντιμετωπίσετε το πρόβλημα.. Λάβετε υπόψη ότι το [Teams απαιτεί το Exchange 2016 CU3 ή νεότερη έκδοση](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Για περισσότερες πληροφορίες και βήματα αντιμετώπισης προβλημάτων, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων Microsoft Teams και Exchange Server αλληλεπιδράσεων.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
