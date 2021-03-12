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
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="3062f-102">Εκχώρηση ρόλου "Αρχείο καταγραφής ελέγχου" στο Κέντρο ασφάλειας του Office 365 & Συμμόρφωσης</span><span class="sxs-lookup"><span data-stu-id="3062f-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="3062f-103">Για να κάνετε αναζήτηση στο αρχείο καταγραφής ελέγχου του Office 365, πρέπει να εκχωρηθεί σε ένα διαχειριστή ο ρόλος "Αρχεία **καταγραφής** ελέγχου μόνο για προβολή" ή ο ρόλος "Αρχεία **καταγραφής** ελέγχου" στο Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3062f-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="3062f-104">Αυτοί οι ρόλοι εκχωρούνται στις ομάδες ρόλων "Διαχείριση συμμόρφωσης" και "Διαχείριση οργανισμού" από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="3062f-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="3062f-105">Οι καθολικοί διαχειριστές στο Office 365 και το Microsoft 365 προστίθενται αυτόματα ως μέλη της ομάδας ρόλων διαχείρισης οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="3062f-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="3062f-106">Για να επιτρέψετε σε ένα χρήστη να πραγματοποιεί αναζήτηση με το ελάχιστο επίπεδο δικαιωμάτων, δημιουργήστε  μια προσαρμοσμένη ομάδα ρόλων στο Exchange Online, προσθέστε το ρόλο "Αρχεία **καταγραφής** ελέγχου μόνο για προβολή" ή το ρόλο "Αρχεία καταγραφής ελέγχου" και, στη συνέχεια, προσθέστε το χρήστη ως μέλος της νέας ομάδας ρόλων.</span><span class="sxs-lookup"><span data-stu-id="3062f-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="3062f-107">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Διαχείριση ομάδων](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) ρόλων στο Exchange Online και αναζήτηση στο αρχείο [καταγραφής ελέγχου στο Κέντρο & ασφάλειας.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="3062f-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>