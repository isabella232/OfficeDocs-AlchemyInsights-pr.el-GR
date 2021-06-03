---
title: Το τελικό σημείο DLP δεν έχει αναπτυχθεί στη συσκευή του χρήστη
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731584"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Το τελικό σημείο DLP δεν έχει αναπτυχθεί στη συσκευή του χρήστη

Εάν η ρύθμιση αποτροπής απώλειας δεδομένων τελικού σημείου (DLP) δεν έχει εφαρμοστεί στη συσκευή ενός χρήστη, επιβεβαιώστε ότι πληροίτε αυτές τις απαιτήσεις:

- Windows 10 έκδοση x64 1809 ή νεότερη έκδοση είναι εγκατεστημένη στη συσκευή.
- Έχει εγκατασταθεί η έκδοση 4.18.2009.7 ή νεότερη έκδοση προγράμματος-πελάτη προστασίας από λογισμικό κακόβουλης λειτουργίας.
- Η συσκευή είναι **μία από** τις εξής:
    
    - Azure Active Directory (Azure AD) συνδεδεμένος
    - Υβριδική σύνδεση azure AD
    - Καταχωρημένο AAD

- Για να επιβάλετε ενέργειες πολιτικής, βεβαιωθείτε ότι το πρόγραμμα Chromium Microsoft Edge είναι εγκατεστημένο στη συσκευή τελικού σημείου.

Για πρόσθετες απαιτήσεις για την ανάπτυξη του DLP τελικού σημείου, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με την αποτροπή απώλειας δεδομένων τελικού σημείου.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)