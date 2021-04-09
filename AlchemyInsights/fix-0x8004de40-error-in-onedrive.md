---
title: Επιδιόρθωση 0x8004de40 σφάλματος στο OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649748"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Επιδιόρθωση 0x8004de40 σφάλματος στο OneDrive

Εάν χρησιμοποιείτε Windows 7 και λάβετε αυτό το σφάλμα, ενημερώστε το για να ενεργοποιήσετε τα [TLS 1.1 και TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ως προεπιλεγμένα πρωτόκολλα ασφαλείας στο WinHTTP στα Windows.

Εάν χρησιμοποιείτε Windows 10 και λάβετε ένα μήνυμα σφάλματος 0x8004de40 oneDrive:

- Επανεκκινήστε τον υπολογιστή που επηρεάζεται ενώ είστε συνδεδεμένοι στον τομέα καταλόγου Acitve.
- Εάν μια επανεκκίνηση δεν διορθώσει το πρόβλημα, αποσυνδεθείτε και επανασυνδεθείτε στη συσκευή σας από το Azure AD. 

**Σημείωση:** Θα πρέπει να είστε στο εταιρικό σας δίκτυο κατά την εκτέλεση αυτών των βημάτων. Μην εκτελείτε αυτά τα βήματα όταν δεν είστε συνδεδεμένοι στην εταιρική υποδομή σας (για παράδειγμα, ενώ ταξιδεύετε). 

1. Ανοίξτε μια αναβαθμισμένη γραμμή εντολών επιλέγοντας "Έναρξη", κάντε δεξί κλικ στη γραμμή **εντολών και,** στη συνέχεια, επιλέξτε **"Εκτέλεση ως διαχειριστής".**

1. Πληκτρολογήστε *dsregcmd /leave και πατήστε* το **πλήκτρο Enter.**

1. Όταν ολοκληρωθεί, πληκτρολογήστε *dsregcmd /join και πατήστε* το **πλήκτρο Enter.**

1. Όταν ολοκληρωθεί, κλείστε τη γραμμή εντολών.

1. Επανεκκινήστε τον υπολογιστή και συνδεθείτε στο OneDrive.