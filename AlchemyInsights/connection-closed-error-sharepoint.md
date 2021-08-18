---
title: Το υποκείμενο σφάλμα σύνδεσης έκλεισε σε SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317696"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Σφάλμα "Η υποκείμενη σύνδεση έκλεισε" στο SharePoint

Εάν λαμβάνετε το σφάλμα "Η υποκείμενη σύνδεση έκλεισε" στο SharePoint μπορεί να σχετίζεται με την απόσβεση του TLS 1.0/1.1. Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω άρθρα:

- [Προετοιμασία για TLS 1.2 σε Office 365 και Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Σφάλματα ελέγχου ταυτότητας προκύπτουν εάν το πρόγραμμα-πελάτης δεν έχει υποστήριξη TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Ενημέρωση για την ενεργοποίηση των TLS 1.1 και TLS 1.2 ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP σε Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Εάν οι χρήστες βρίσκονται στο Windows 7, βεβαιωθείτε ότι ελέγχουν τις οικογένειες προγραμμάτων [κρυπτογράφησης TLS στο Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)