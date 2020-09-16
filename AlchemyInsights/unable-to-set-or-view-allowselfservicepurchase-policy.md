---
title: Δεν είναι δυνατός ο καθορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735199"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Δεν είναι δυνατός ο καθορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase

Όταν επιχειρείτε να καθορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα σφάλματος:

*HandleError: δεν ήταν δυνατή η ανάκτηση της πολιτικής προϊόντος με το PolicyId ' AllowSelfServicePurchase ', μήνυμα-η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε μη αναμενόμενο σφάλμα σε μια αποστολή.*

Αυτό μπορεί να οφείλεται σε μια παλαιότερη έκδοση της ασφάλειας επιπέδου μεταφοράς (TLS). Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε το TLS 1,2 ή νεότερη.  

Δοκιμάστε τα παρακάτω βήματα για να ενεργοποιήσετε/Ορίστε το πρωτόκολλο TLS στο 1,2, επαληθεύστε και προσπαθήστε ξανά.
 1. Στη γραμμή εντολών PowerShell (PS C: \) Πληκτρολογήστε την ακόλουθη εντολή για να καθορίσετε το πρωτόκολλο TLS στην έκδοση 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Επαναλάβετε τις εντολές λήψη ή ενημέρωση, ανάλογα με τις ανάγκες.

