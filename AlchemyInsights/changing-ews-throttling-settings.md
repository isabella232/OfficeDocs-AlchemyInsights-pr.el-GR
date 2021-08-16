---
title: Αλλαγή ρυθμίσεων ελέγχου EWS
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968377"
---
# <a name="changing-ews-throttling-settings"></a>Αλλαγή ρυθμίσεων ελέγχου EWS

Εκτελέστε τον αυτοματοποιημένο έλεγχο που θα σας επιτρέψει να τροποποιήσετε την πολιτική ελέγχου EWS κατά τη διάρκεια της μετεγκατάστασης. Σημειώστε ότι ακόμη και αφού εκτελεστεί αυτή η διαδικασία, οι εισαγωγές EWS θα εξακολουθούν να περιορίζονται στα 150mb ανά 5 λεπτά ανά γραμματοκιβώτιο. Για να επιτύχετε υψηλότερη ταχύτητα μετάδοσης μετεγκατάστασης, κάντε μετεγκατάσταση περισσότερων χρηστών ταυτόχρονα.

Έχετε υπόψη ότι οι αλλαγές της πολιτικής ελέγχου EWS δεν έχουν καμία επίδραση στους ακόλουθους τύπους μετεγκατάστασης (χρησιμοποιώντας τα εργαλεία της Microsoft): Υβριδική, Πλήρης μεταφορά/Σταδιακή (RPC/HTTP), IMAP, G Suite, Δημόσιος φάκελος ή Υπηρεσία εισαγωγής PST.