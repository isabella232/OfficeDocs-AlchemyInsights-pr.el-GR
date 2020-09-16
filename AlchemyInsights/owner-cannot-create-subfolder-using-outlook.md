---
title: Ο κάτοχος δεν μπορεί να δημιουργήσει δευτερεύοντα φάκελο χρησιμοποιώντας το Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665718"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="6ba0a-102">Ο κάτοχος δεν μπορεί να δημιουργήσει δευτερεύοντα φάκελο χρησιμοποιώντας το Outlook</span><span class="sxs-lookup"><span data-stu-id="6ba0a-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="6ba0a-103">**Υπάρχει ένα πρόβλημα που βρίσκεται σε εξέλιξη με τους κατόχους δημόσιων φακέλων να δημιουργούν υποφακέλους χρησιμοποιώντας το Outlook. Το πρόβλημα θα διορθωθεί σύντομα.**</span><span class="sxs-lookup"><span data-stu-id="6ba0a-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="6ba0a-104">Εν τω μεταξύ, χρησιμοποιήστε μία από τις παρακάτω λύσεις:</span><span class="sxs-lookup"><span data-stu-id="6ba0a-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="6ba0a-105">Χρήση του Outlook για MAC για τη δημιουργία του υποφακέλου, καθώς το πρόβλημα επηρεάζει μόνο το Outlook για υπολογιστή Windows (όλες οι εκδόσεις)</span><span class="sxs-lookup"><span data-stu-id="6ba0a-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="6ba0a-106">Ζητήστε από το διαχειριστή να δημιουργήσει τον υποφάκελο χρησιμοποιώντας το εξωτερικό κέλυφος ή την ΑΗΚ</span><span class="sxs-lookup"><span data-stu-id="6ba0a-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="6ba0a-107">Αλλαγή του DefaultPublicFolderMailbox/EffectivePublicFolderMailbox στο χρήστη σε άλλο γραμματοκιβώτιο από το γραμματοκιβώτιο περιεχομένου για τον φάκελο που προκαλεί το πρόβλημα</span><span class="sxs-lookup"><span data-stu-id="6ba0a-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="6ba0a-108">*User1 γραμματοκιβωτίου DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="6ba0a-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="6ba0a-109">Περιμένετε μια ώρα, επανεκκινήστε το πρόγραμμα-πελάτη του Outlook</span><span class="sxs-lookup"><span data-stu-id="6ba0a-109">Wait for an hour, restart outlook client</span></span>