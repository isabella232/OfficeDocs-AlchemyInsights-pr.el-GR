---
title: Ο κάτοχος δεν είναι δυνατό να δημιουργήσει δευτερεύοντα φάκελο χρησιμοποιώντας το Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748907"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="6d71c-102">Ο κάτοχος δεν είναι δυνατό να δημιουργήσει δευτερεύοντα φάκελο χρησιμοποιώντας το Outlook</span><span class="sxs-lookup"><span data-stu-id="6d71c-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="6d71c-103">**Υπάρχει ένα συνεχιζόμενο ζήτημα με τους κατόχους δημόσιων φακέλων που δημιουργούν υποφακέλους χρησιμοποιώντας το Outlook. Το ζήτημα θα διορθωθεί σύντομα.**</span><span class="sxs-lookup"><span data-stu-id="6d71c-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="6d71c-104">Εν τω μεταξύ, χρησιμοποιήστε μία από τις ακόλουθες λύσεις:</span><span class="sxs-lookup"><span data-stu-id="6d71c-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="6d71c-105">Χρήση του Outlook για MAC για τη δημιουργία του υποφακέλου, καθώς το ζήτημα επηρεάζει μόνο το Outlook για παράθυρα επιφάνειας εργασίας (όλες οι εκδόσεις)</span><span class="sxs-lookup"><span data-stu-id="6d71c-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="6d71c-106">Να δημιουργήσει ο διαχειριστής τον υποφάκελο χρησιμοποιώντας το κέλυφος EXO ή την ΑΗΚ</span><span class="sxs-lookup"><span data-stu-id="6d71c-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="6d71c-107">Αλλαγή του πλαισίου DefaultPublicFolderMailbox/EffectivePublicFolderMailbox στο χρήστη σε άλλο γραμματοκιβώτιο από το γραμματοκιβώτιο περιεχομένου για το φάκελο που προκαλεί ζήτημα</span><span class="sxs-lookup"><span data-stu-id="6d71c-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="6d71c-108">*Set-Γραμματοκιβώτιο User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="6d71c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="6d71c-109">Περιμένετε για μια ώρα, κάντε επανεκκίνηση του προγράμματος-πελάτη του Outlook</span><span class="sxs-lookup"><span data-stu-id="6d71c-109">Wait for an hour, restart outlook client</span></span>