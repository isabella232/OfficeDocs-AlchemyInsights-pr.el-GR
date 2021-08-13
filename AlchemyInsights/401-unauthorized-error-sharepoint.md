---
title: 401 Μη εξουσιοδοτημένο σφάλμα στο SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919027"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Μη εξουσιοδοτημένο σφάλμα στο SharePoint

Εάν εμφανιστεί το σφάλμα "(401) Μη εξουσιοδοτημένη" στο SharePoint μπορεί να σχετίζεται με την κατάργηση του TLS 1.0/1.1. Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα:

- [Προετοιμασία για TLS 1.2 σε Office 365 και Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Σφάλματα ελέγχου ταυτότητας προκύπτουν εάν το πρόγραμμα-πελάτης δεν έχει υποστήριξη TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Ενημέρωση για την ενεργοποίηση των TLS 1.1 και TLS 1.2 ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Εάν οι χρήστες βρίσκονται στο Windows 7, βεβαιωθείτε ότι ελέγχουν τις οικογένειες προγραμμάτων [κρυπτογράφησης TLS στο Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)