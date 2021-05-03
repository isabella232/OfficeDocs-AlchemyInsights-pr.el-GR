---
title: Προβλήματα με SharePoint σε Windows 7 υπολογιστές
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125120"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Προβλήματα με SharePoint σε Windows 7 υπολογιστές

Εάν λάβετε σφάλματα σε Windows 7 υπολογιστές ενώ εργάζεστε σε SharePoint ή OneDrive, ενδέχεται να σχετίζονται με την απόσβεση του TLS 1.0/1.1. Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

- [Προετοιμασία για TLS 1.2 σε Office 365 και Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 πρέπει να έχουν ενεργοποιημένο το TLS1.2. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Σφάλματα ελέγχου ταυτότητας όταν το πρόγραμμα-πελάτης δεν έχει υποστήριξη TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Εγκαταστήστε το KB3140245 και δημιουργήστε την τιμή μητρώου. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ενημέρωση για την ενεργοποίηση [των TLS 1.1 και TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows

- Windows 7 SP1/Windows 8 πρέπει να εξασφαλίσουν ότι έχουν εγκατασταθεί οι πιο πρόσφατες οικογένειες προγραμμάτων κρυπτογράφησης TLS. Για περισσότερες πληροφορίες, ανατρέξτε στο [Συμβουλευτικό δελτίο ασφαλείας της Microsoft 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


