---
title: Η εικόνα χρήστη δεν εμφανίζεται σε Microsoft Teams οργανόγραμμα
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792754"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Η εικόνα χρήστη δεν εμφανίζεται σε Microsoft Teams οργανόγραμμα

Εάν ένα ή περισσότερα άτομα στον οργανισμό σας δεν έχουν τη φωτογραφία προφίλ τους στο οργανόγραμμα, είναι πιθανό η ρύθμιση **ShowInAddressLists** να έχει οριστεί σε **Ψευδές:**

1. Μεταβείτε Κέντρο διαχείρισης Microsoft 365 > την επιλογή [**Ενεργοί χρήστες**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)και επιλέξτε το χρήστη με τη φωτογραφία που λείπει. 
1. Επιλέξτε την καρτέλα **Αλληλογραφία** και βεβαιωθείτε ότι η επιλογή **Εμφάνιση στην καθολική λίστα διευθύνσεων** έχει οριστεί σε **Ναι.** 

Εάν η ρύθμιση **ShowInAddressLists** σε **Yes** δεν λειτουργεί, ελέγξτε τα εξής:

- Ο χρήστης μπορεί να είναι κρυφός από τη λίστα παραληπτών στο Exchange. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση λιστών διευθύνσεων στο Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Ο χρήστης μπορεί να είναι κρυφός από τη λίστα διευθύνσεων στο Azure Active Directory. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
