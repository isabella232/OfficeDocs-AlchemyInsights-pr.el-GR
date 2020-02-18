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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091706"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase

Όταν επιχειρείτε να ορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα λάθους:

*HandleError: απέτυχε η ανάκτηση της πολιτικής προϊόντος με PolicyId ' AllowSelfServicePurchase ', μήνυμα-η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε ένα μη αναμενόμενο σφάλμα σε μια αποστολή.*

Αυτό μπορεί να οφείλεται σε παλαιότερη έκδοση της ασφάλειας επιπέδου μεταφοράς (TLS). Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε το TLS 1,2 ή μεγαλύτερο.  

Δοκιμάστε τα ακόλουθα βήματα για να ενεργοποιήσετε/ορίσετε το πρωτόκολλο TLS σε 1,2, επιβεβαιώστε και προσπαθήστε ξανά.
 1. Στη γραμμή εντολών PowerShell (PS C:\) πληκτρολογήστε την ακόλουθη εντολή για να ορίσετε το πρωτόκολλο TLS στην έκδοση 1,2:

    \[NET. ServicePointManager]:: SecurityProtocol = \[NET. SecurityProtocolType]:: Tls12

2. Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:

    \[NET. ServicePointManager]:: SecurityProtocol 

3. Επαναλάβετε τις εντολές "λάβετε" ή "ενημέρωση", όπως απαιτείται.

