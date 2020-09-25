---
title: 1490-αντιμετώπιση προβλημάτων-ηλεκτρονική ανακάλυψη-αποτυχίες
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
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277846"
---
# <a name="troubleshoot-content-search-errors"></a>Αντιμετώπιση σφαλμάτων αναζήτησης περιεχομένου

Αντιμετωπίζετε προβλήματα με την αναζήτηση περιεχομένου ή τη λήψη αποτυχιών κατά την εξαγωγή των αποτελεσμάτων αναζήτησης;

Για παράδειγμα, λαμβάνετε τα παρακάτω κατά την εκτέλεση αναζητήσεων;

- Σφάλματα CS008 ή CS012

- Σφάλματα διαθεσιμότητας/χρονικού ορίου διακομιστή

- Παρουσιάστηκε σφάλμα εφαρμογής

Ή κατά την αναζήτηση ή την εξαγωγή αποτελεσμάτων από μεγάλο αριθμό γραμματοκιβωτίων (πάνω από 100.000 γραμματοκιβώτια), λαμβάνετε σφάλματα εξαγωγής;

Για αυτούς τους τύπους σφαλμάτων, επαναλάβετε την αναζήτηση για τις θέσεις περιεχομένου που έχουν αποτύχει. Ανατρέξτε σε  [αυτό το άρθρο](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) για περισσότερες πληροφορίες.

Εάν εξάγετε περισσότερα από 100K γραμματοκιβώτια, θα πρέπει να χρησιμοποιήσετε το ακόλουθο PowerShell για να κάνετε λήψη των αποτελεσμάτων εξαγωγής:  [Εξαγωγή αποτελεσμάτων από περισσότερα από 100K γραμματοκιβώτια](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
