---
title: Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826091"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase

Όταν προσπαθείτε να ορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα σφάλματος:

*HandleError : Απέτυχε η ανάκτηση πολιτικής προϊόντος με το PolicyId "AllowSelfServicePurchase", ErrorMessage - Η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε μη αναμενόμενο σφάλμα κατά την αποστολή.*

Αυτό μπορεί να οφείλεται σε μια παλαιότερη έκδοση του Transport Layer Security (TLS). Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε TLS 1.2 ή μεγαλύτερο.  

Δοκιμάστε τα παρακάτω βήματα για να ενεργοποιήσετε/ορίσετε το πρωτόκολλο TLS σε 1,2, να επαληθεύσετε και να επαναλάβετε την προσπάθεια.
 1. Στη γραμμή εντολών του PowerShell (PS C: πληκτρολογήστε την ακόλουθη εντολή για να \) ορίσετε το πρωτόκολλο TLS στην έκδοση 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Επαναλάβετε τις εντολές "Λήψη" ή "Ενημέρωση", όπως απαιτείται.

