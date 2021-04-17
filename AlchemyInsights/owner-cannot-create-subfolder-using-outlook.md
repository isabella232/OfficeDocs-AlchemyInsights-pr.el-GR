---
title: Ο κάτοχος δεν μπορεί να δημιουργήσει υποφάκελο χρησιμοποιώντας το Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836135"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="e10bd-102">Ο κάτοχος δεν μπορεί να δημιουργήσει υποφάκελο χρησιμοποιώντας το Outlook</span><span class="sxs-lookup"><span data-stu-id="e10bd-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="e10bd-103">**Υπάρχει ένα συνεχιζόμενο πρόβλημα με τους κατόχους δημόσιων φακέλων που δημιουργούν υποφακέλους χρησιμοποιώντας το Outlook. Το πρόβλημα θα διορθωθεί σύντομα.**</span><span class="sxs-lookup"><span data-stu-id="e10bd-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="e10bd-104">Στο μεταξύ, χρησιμοποιήστε μία από τις παρακάτω λύσεις:</span><span class="sxs-lookup"><span data-stu-id="e10bd-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="e10bd-105">Χρησιμοποιήστε το Outlook για MAC για να δημιουργήσετε τον υποφάκελο, καθώς το πρόβλημα επηρεάζει μόνο το Outlook για windows για υπολογιστή (όλες οι εκδόσεις)</span><span class="sxs-lookup"><span data-stu-id="e10bd-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="e10bd-106">Να έχει ο διαχειριστής τη δημιουργία του υποφακέλου χρησιμοποιώντας το κέλυφος EXO ή το EAC</span><span class="sxs-lookup"><span data-stu-id="e10bd-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="e10bd-107">Αλλαγή του DefaultPublicFolderMailbox/EffectivePublicFolderMailbox στο χρήστη σε άλλο γραμματοκιβώτιο εκτός από το γραμματοκιβώτιο περιεχομένου για το φάκελο που προκαλεί το πρόβλημα</span><span class="sxs-lookup"><span data-stu-id="e10bd-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="e10bd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="e10bd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="e10bd-109">Περιμένετε μία ώρα, επανεκκινήστε το πρόγραμμα-πελάτη του Outlook</span><span class="sxs-lookup"><span data-stu-id="e10bd-109">Wait for an hour, restart outlook client</span></span>