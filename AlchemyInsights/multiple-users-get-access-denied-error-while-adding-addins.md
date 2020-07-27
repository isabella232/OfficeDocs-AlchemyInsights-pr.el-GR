---
title: Πολλοί χρήστες λαμβάνουν σφάλμα άρνησης πρόσβασης κατά την προσθήκη πρόσθετων στο Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423713"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Πολλοί χρήστες λαμβάνουν σφάλμα άρνησης πρόσβασης κατά την προσθήκη πρόσθετων στο Outlook

Μπορείτε να καθορίσετε ποιοι διαχειριστές στην εταιρεία σας έχουν δικαιώματα εγκατάστασης και διαχείρισης πρόσθετων για το Outlook. Μπορείτε επίσης να καθορίσετε ποιοι χρήστες στην εταιρεία σας έχουν δικαίωμα εγκατάστασης και διαχείρισης πρόσθετων για δική τους χρήση.

Για λεπτομέρειες, ανατρέξτε στο θέμα [Καθορισμός των διαχειριστών και των χρηστών που μπορούν να εγκαταστήσουν και να διαχειριστούν πρόσθετα για το Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Για να επαληθεύσετε ότι έχετε εκχωρήσει με επιτυχία δικαιώματα για ένα χρήστη, αντικαταστήστε <Role Name> με το όνομα του ρόλου που θέλετε να επαληθεύσετε και εκτελέστε την ακόλουθη εντολή στο Exchange Online PowerShell:

Get-ManagementRoleAssignment -Ρόλος " <Role Name> " -GetEffectiveUsers

Αυτό το παράδειγμα σάς δείχνει πώς μπορείτε να επαληθεύσετε σε ποιον έχετε εκχωρήσει δικαιώματα για την εγκατάσταση πρόσθετων από το Office Store για τον οργανισμό.

Powershell

-Ρόλος "Org Marketplace Apps" -GetEffectiveUsers

Στα αποτελέσματα, Get-ManagementRoleAssignment, εξετάστε τις καταχωρήσεις στη στήλη Αποτελεσματικοί χρήστες.

Για λεπτομερείς πληροφορίες σύνταξης και παραμέτρων, ανατρέξτε στο θέμα [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 