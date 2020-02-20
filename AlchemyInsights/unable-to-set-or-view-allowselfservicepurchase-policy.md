---
title: Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158561"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase

Όταν επιχειρείτε να ορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα λάθους:

*HandleError: απέτυχε η ανάκτηση της πολιτικής προϊόντος με PolicyId ' AllowSelfServicePurchase ', μήνυμα-η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε ένα μη αναμενόμενο σφάλμα σε μια αποστολή.*

Αυτό μπορεί να οφείλεται σε παλαιότερη έκδοση της ασφάλειας επιπέδου μεταφοράς (TLS). Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε το TLS 1,2 ή μεγαλύτερο.  

Δοκιμάστε τα ακόλουθα βήματα για να ενεργοποιήσετε/ορίσετε το πρωτόκολλο TLS σε 1,2, επιβεβαιώστε και προσπαθήστε ξανά.
 1. Στη γραμμή εντολών PowerShell (PS C:\) πληκτρολογήστε την ακόλουθη εντολή για να ορίσετε το πρωτόκολλο TLS στην έκδοση 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Επαναλάβετε τις εντολές "λάβετε" ή "ενημέρωση", όπως απαιτείται.

