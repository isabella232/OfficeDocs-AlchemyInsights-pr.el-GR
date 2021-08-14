---
title: Εικονίδιο ημερολογίου που δεν εμφανίζεται στο πρόγραμμα-πελάτη του Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989591"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Εικονίδιο ημερολογίου που δεν εμφανίζεται στο πρόγραμμα-πελάτη του Teams

Η καρτέλα ημερολογίου στο Teams απαιτεί πρόσβαση σε ένα γραμματοκιβώτιο του Exchange μέσω των υπηρεσιών Web του Exchange. Το γραμματοκιβώτιο του Exchange μπορεί να είναι online ή εσωτερικής εγκατάστασης. Για τους online χρήστες που δεν μπορούν να δουν την καρτέλα ημερολογίου, βεβαιωθείτε ότι [έχουν άδεια χρήσης για ένα γραμματοκιβώτιο του Exchange Online και ότι το γραμματοκιβώτιο έχει ενεργοποιηθεί](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Εάν ο χρήστης έχει ένα έγκυρο γραμματοκιβώτιο στο Exchange Online, αλλά εξακολουθεί να μην μπορεί να δει την καρτέλα ημερολογίου, ενδέχεται να αντιμετωπίζετε κάποιο πρόβλημα με το δίκτυο. Χρησιμοποιήστε το [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) και εκτελέστε τους **Ελέγχους συνδεσιμότητας των Υπηρεσιών Web του Microsoft Exchange** για τον επηρεαζόμενο χρήστη.

Τέλος, ελέγξτε το θέμα [Εφαρμογές του Teams – Πολιτικές εγκατάστασης εφαρμογών](https://admin.teams.microsoft.com/policies/app-setup) για να εξασφαλίσετε ότι η εφαρμογή "Ημερολόγιο" δεν έχει καταργηθεί από την πολιτική που εφαρμόζεται για τον χρήστη (πιθανότατα η **Καθολική (προεπιλογή σε επίπεδο οργανισμού)**).

Εάν οι χρήστες σας φιλοξενούνται στην εσωτερική εγκατάσταση, πρέπει να επιβεβαιώσετε ότι η υβριδική ρύθμιση παραμέτρων λειτουργεί κανονικά. Χρησιμοποιήστε τον [Οδηγό υβριδικής ρύθμισης παραμέτρων](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) για να αντιμετωπίσετε το πρόβλημα..

Λάβετε υπόψη ότι το [Teams απαιτεί το Exchange 2016 CU3 ή νεότερη έκδοση](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
