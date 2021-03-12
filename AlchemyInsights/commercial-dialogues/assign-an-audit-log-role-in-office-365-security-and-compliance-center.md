---
title: Εκχώρηση ρόλου "Αρχείο καταγραφής ελέγχου" στο Κέντρο ασφάλειας του Office 365 & Συμμόρφωσης
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746167"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Εκχώρηση ρόλου "Αρχείο καταγραφής ελέγχου" στο Κέντρο ασφάλειας του Office 365 & Συμμόρφωσης

Για να κάνετε αναζήτηση στο αρχείο καταγραφής ελέγχου του Office 365, πρέπει να εκχωρηθεί σε ένα διαχειριστή ο ρόλος "Αρχεία **καταγραφής** ελέγχου μόνο για προβολή" ή ο ρόλος "Αρχεία **καταγραφής** ελέγχου" στο Exchange Online. Αυτοί οι ρόλοι εκχωρούνται στις ομάδες ρόλων "Διαχείριση συμμόρφωσης" και "Διαχείριση οργανισμού" από προεπιλογή. Οι καθολικοί διαχειριστές στο Office 365 και το Microsoft 365 προστίθενται αυτόματα ως μέλη της ομάδας ρόλων διαχείρισης οργανισμού.

Για να επιτρέψετε σε ένα χρήστη να πραγματοποιεί αναζήτηση με το ελάχιστο επίπεδο δικαιωμάτων, δημιουργήστε  μια προσαρμοσμένη ομάδα ρόλων στο Exchange Online, προσθέστε το ρόλο "Αρχεία **καταγραφής** ελέγχου μόνο για προβολή" ή το ρόλο "Αρχεία καταγραφής ελέγχου" και, στη συνέχεια, προσθέστε το χρήστη ως μέλος της νέας ομάδας ρόλων.

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Διαχείριση ομάδων](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) ρόλων στο Exchange Online και αναζήτηση στο αρχείο [καταγραφής ελέγχου στο Κέντρο & ασφάλειας.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)