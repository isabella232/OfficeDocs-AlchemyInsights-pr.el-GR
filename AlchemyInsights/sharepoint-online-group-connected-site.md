---
title: Προσθήκη ομάδας σε μια SharePoint τοποθεσίας
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897716"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Συνήθη προβλήματα κατά τη δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας σε SharePoint

1. Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.

   - Λήψη [κελύφους διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Για περισσότερες πληροφορίες σχετικά με τα γρήγορα αποτελέσματα με το Powershell, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με SharePoint Κέλυφος ηλεκτρονικής διαχείρισης.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Καταργήστε την τοποθεσία από διαγραμμένες τοποθεσίες [χρησιμοποιώντας το cmdlet Powershell Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Το Powershell απαιτείται για την οριστική διαγραφή τοποθεσιών ομάδας.

1. Εάν δημιουργείτε μια συνδεδεμένη τοποθεσία ομάδας και λαμβάνετε μια **προειδοποίηση:** Μια άλλη ομάδα με το ίδιο ψευδώνυμο υπάρχει ήδη, ελέγξτε τις υπάρχουσες ομάδες από [το Κέντρο διαχείρισης Microsoft 365.](https://admin.microsoft.com/AdminPortal/Home#/groups) Για να επιλύσετε το πρόβλημα, διαγράψτε την υπάρχουσα ομάδα εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με διαφορετικό ψευδώνυμο.

1. Υπάρχουν διαφορετικοί τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε σύγχρονες ομάδες με SharePoint.

   - Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια Microsoft 365 ομάδας. Για περισσότερες πληροφορίες, [ανατρέξτε Σύνδεση μια Microsoft 365 χρησιμοποιώντας το SharePoint χρήστη.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Για να δημιουργήσετε μια Microsoft 365 συνδεδεμένη τοποθεσία ομάδας, θα πρέπει να δημιουργήσετε μια [τοποθεσία ομάδας.](https://admin.microsoft.com/sharepoint)
