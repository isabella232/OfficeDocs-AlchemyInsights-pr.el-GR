---
title: 1490-troubleshooting-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105568"
---
# <a name="troubleshoot-content-search-errors"></a>Αντιμετώπιση σφαλμάτων αναζήτησης περιεχομένου

Αντιμετωπίζετε προβλήματα με την Αναζήτηση περιεχομένου ή αντιμετωπίζετε αποτυχίες κατά την εξαγωγή αποτελεσμάτων αναζήτησης;

Για παράδειγμα, λαμβάνετε τα εξής κατά την εκτέλεση αναζητήσεων;

- Σφάλματα CS008 ή CS012

- Σφάλματα διαθεσιμότητας διακομιστή/χρονικού ορίου

- Παρουσιάστηκε σφάλμα εφαρμογής

Ή κατά την αναζήτηση ή εξαγωγή αποτελεσμάτων από μεγάλο αριθμό γραμματοκιβωτίων (πάνω από 100.000 γραμματοκιβώτια), εμφανίζεται σφάλμα εξαγωγής;

Για αυτούς τους τύπους σφαλμάτων, επαναλάβετε την αναζήτηση για τις θέσεις περιεχομένου που έχουν αποτύχει. Ανατρέξτε  [σε αυτό το](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) άρθρο για περισσότερες πληροφορίες.

Εάν εξάγετε περισσότερα από 100K γραμματοκιβώτια, θα πρέπει να χρησιμοποιήσετε το ακόλουθο Powershell για να κάνετε λήψη των αποτελεσμάτων εξαγωγής: Εξαγωγή αποτελεσμάτων από περισσότερα από [100K γραμματοκιβώτια.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
