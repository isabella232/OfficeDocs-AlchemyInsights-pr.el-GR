---
title: Η εικόνα χρήστη εξακολουθεί να εμφανίζεται στο οργανόγραμμα Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422254"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Η εικόνα χρήστη εξακολουθεί να εμφανίζεται στο οργανόγραμμα Microsoft Teams

Εάν ένα ή περισσότερα άτομα στον οργανισμό σας έχουν απενεργοποιηθεί ή καταργηθεί και η φωτογραφία προφίλ τους εξακολουθεί να εμφανίζεται στο οργανόγραμμα, είναι πιθανό η ρύθμιση **ShowInAddressLists** να έχει οριστεί στην τιμή False: 

1. Μεταβείτε στο Κέντρο διαχείρισης Microsoft 365 > [Ενεργοί χρήστες](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) και επιλέξτε το χρήστη με τη φωτογραφία που εξακολουθεί να εμφανίζεται. 
1. Επιλέξτε την καρτέλα **Αλληλογραφία** και βεβαιωθείτε ότι η επιλογή **Εμφάνιση στην καθολική λίστα διευθύνσεων** έχει οριστεί σε **Όχι.**

Εάν η ρύθμιση **ShowInAddressLists** σε **Όχι** δεν λειτουργεί, ελέγξτε τα εξής: 

- Ο χρήστης μπορεί να εμφανίζεται από τη λίστα παραληπτών στο Exchange. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση λιστών διευθύνσεων στο Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Ο χρήστης μπορεί να εμφανίζεται από τη λίστα διευθύνσεων στο Azure Active Directory. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 