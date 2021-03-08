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
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="ce119-102">Εκχώρηση ρόλου αρχείου καταγραφής ελέγχου στο Κέντρο συμμόρφωσης ασφαλείας του Office 365 & Συμμόρφωσης</span><span class="sxs-lookup"><span data-stu-id="ce119-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="ce119-103">Για να κάνετε αναζήτηση στο αρχείο καταγραφής ελέγχου του  Office 365,  πρέπει να έχει εκχωρηθεί ο ρόλος "Αρχεία καταγραφής ελέγχου μόνο για προβολή" ή ο ρόλος "Αρχεία καταγραφής ελέγχου" στο Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ce119-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="ce119-104">Αυτοί οι ρόλοι εκχωρούνται από προεπιλογή στις ομάδες ρόλων "Διαχείριση συμμόρφωσης" και "Διαχείριση οργανισμού".</span><span class="sxs-lookup"><span data-stu-id="ce119-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="ce119-105">Οι καθολικοί διαχειριστές του Office 365 και του Microsoft 365 προστίθενται αυτόματα ως μέλη της ομάδας ρόλων "Διαχείριση οργανισμού".</span><span class="sxs-lookup"><span data-stu-id="ce119-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="ce119-106">Για να επιτρέψετε σε ένα χρήστη να κάνει αναζήτηση με το ελάχιστο  επίπεδο δικαιωμάτων, δημιουργήστε  μια προσαρμοσμένη ομάδα ρόλων στο Exchange Online, προσθέστε το ρόλο "Αρχεία καταγραφής ελέγχου μόνο για προβολή" ή το ρόλο "Αρχεία καταγραφής ελέγχου" και, στη συνέχεια, προσθέστε το χρήστη ως μέλος της νέας ομάδας ρόλων.</span><span class="sxs-lookup"><span data-stu-id="ce119-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="ce119-107">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Διαχείριση ομάδων ρόλων](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) στο Exchange Online" και "Αναζήτηση στο αρχείο [καταγραφής ελέγχου" στο Κέντρο & συμμόρφωσης.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="ce119-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>