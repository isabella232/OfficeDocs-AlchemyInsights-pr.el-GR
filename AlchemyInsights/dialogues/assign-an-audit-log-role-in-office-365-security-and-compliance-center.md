---
title: Εκχώρηση ρόλου αρχείου καταγραφής ελέγχου στο Κέντρο συμμόρφωσης ασφαλείας του Office 365 & Συμμόρφωσης
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524792"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Εκχώρηση ρόλου αρχείου καταγραφής ελέγχου στο Κέντρο συμμόρφωσης ασφαλείας του Office 365 & Συμμόρφωσης

Για να κάνετε αναζήτηση στο αρχείο καταγραφής ελέγχου του  Office 365,  πρέπει να έχει εκχωρηθεί ο ρόλος "Αρχεία καταγραφής ελέγχου μόνο για προβολή" ή ο ρόλος "Αρχεία καταγραφής ελέγχου" στο Exchange Online. Αυτοί οι ρόλοι εκχωρούνται από προεπιλογή στις ομάδες ρόλων "Διαχείριση συμμόρφωσης" και "Διαχείριση οργανισμού". Οι καθολικοί διαχειριστές του Office 365 και του Microsoft 365 προστίθενται αυτόματα ως μέλη της ομάδας ρόλων "Διαχείριση οργανισμού".

Για να επιτρέψετε σε ένα χρήστη να κάνει αναζήτηση με το ελάχιστο  επίπεδο δικαιωμάτων, δημιουργήστε  μια προσαρμοσμένη ομάδα ρόλων στο Exchange Online, προσθέστε το ρόλο "Αρχεία καταγραφής ελέγχου μόνο για προβολή" ή το ρόλο "Αρχεία καταγραφής ελέγχου" και, στη συνέχεια, προσθέστε το χρήστη ως μέλος της νέας ομάδας ρόλων.

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Διαχείριση ομάδων ρόλων](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) στο Exchange Online" και "Αναζήτηση στο αρχείο [καταγραφής ελέγχου" στο Κέντρο & συμμόρφωσης.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)