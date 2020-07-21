---
title: Πολλοί χρήστες δεν βλέπουν πρόσθετα στο Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197973"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Πολλοί χρήστες δεν βλέπουν πρόσθετα στο Outlook

Εάν ελέγξετε τα πρόσθετα του Outlook και κανένα δεν εμφανίζεται, ως πρώτο βήμα αντιμετώπισης προβλημάτων, χρησιμοποιήστε το cmdlet **Get-OrganizationConfig** PowerShell για να υποβάλετε ερώτημα στην παράμετρο _AppsForOfficeEnabled._ Εάν το ερώτημα επιστρέψει μια τιμή **False**, ορίστε αυτήν την παράμετρο σε **True** χρησιμοποιώντας το cmdlet **Set-OrganizationConfig,** επομένως τα πρόσθετα εμφανίζονται όπως αναμένεται.

Δεν συνιστάται η _παράμετρος AppsForOfficeEnabled_ να έχει οριστεί σε **False**. Η τιμή **false** παρακάμπτει όλες τις παραπάνω ρυθμίσεις ρόλου διαχείρισης και χρήστη και εμποδίζει την ενεργοποίηση νέων εφαρμογών από οποιονδήποτε χρήστη στον οργανισμό.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Καθορισμός των διαχειριστών και των χρηστών που μπορούν να εγκαταστήσουν και να διαχειριστούν πρόσθετα για το Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).