---
title: Ο μεμονωμένος χρήστης δεν βλέπει πρόσθετα στο Outlook
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
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197959"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Ο μεμονωμένος χρήστης δεν βλέπει πρόσθετα στο Outlook

Ο χρήστης μπορεί να είναι μέρος ενός ρόλου που δεν έχει τη σωστή παράμετρο AppsForOfficeEnabled. Εκτελέστε αυτό το cmdlet για να μάθετε αν ο σωστός ρόλος σχετίζεται με το χρήστη:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Ανάθεση $false | Μορφοποίηση-Πίνακας -Αυτόματος ρόλος,Όνομα ΡόλουAssignee,Τύπος RoleAssignee

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Καθορισμός των διαχειριστών και των χρηστών που μπορούν να εγκαταστήσουν και να διαχειριστούν πρόσθετα για το Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
