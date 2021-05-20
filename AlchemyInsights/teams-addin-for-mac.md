---
title: Teams πρόσθετο για Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582070"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="9aab5-102">Teams πρόσθετο για Mac</span><span class="sxs-lookup"><span data-stu-id="9aab5-102">Teams add-in for Mac</span></span>

<span data-ttu-id="9aab5-103">Για να αντιμετωπίσετε ένα πρόσθετο Teams που λείπει για τους χρήστες λειτουργικού συστήματος Mac, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="9aab5-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="9aab5-104">**Βήμα 1:** Εάν έχετε υβριδική έκδοση Exchange εσωτερικής εγκατάστασης (απαιτείται CU3 2016 ή νεότερη έκδοση), χρησιμοποιήστε το εργαλείο Test-HMA.ps1 για να επιβεβαιώσετε ότι οι παράμετροι του υβριδικού σύγχρονου ελέγχου ταυτότητας έχουν ρυθμιστεί σωστά.</span><span class="sxs-lookup"><span data-stu-id="9aab5-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="9aab5-105">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Επικύρωση ρύθμισης υβριδικού σύγχρονου ελέγχου ταυτότητας για Outlook για iOS και Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="9aab5-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="9aab5-106">**Σημείωση** Χρησιμοποιήστε τη μορφή διεύθυνσης UPN (για παράδειγμα, [username@contoso.com](mailto:username@contoso.com)), όχι τον τομέα\όνομα χρήστη.</span><span class="sxs-lookup"><span data-stu-id="9aab5-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="9aab5-107">Κάντε το αυτό ακόμη και για τους χρήστες με Exchange Online γραμματοκιβώτια.</span><span class="sxs-lookup"><span data-stu-id="9aab5-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="9aab5-108">**Βήμα 2:** Να μεταβεί ο χρήστης στην επιλογή **"Εργαλεία**  >  **λογαριασμών"**... στο Outlook για Mac και βρείτε και επιλέξτε το λογαριασμό.</span><span class="sxs-lookup"><span data-stu-id="9aab5-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="9aab5-109">Επιβεβαιώστε ότι το όνομα χρήστη που αναφέρεται είναι σε μορφή UPN (για παράδειγμα, [username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="9aab5-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="9aab5-110">**Βήμα 3:** Επιβεβαιώστε ότι ο χρήστης διαθέτει άδεια χρήσης Microsoft Teams χρήστη.</span><span class="sxs-lookup"><span data-stu-id="9aab5-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="9aab5-111">Ο χρήστης πρέπει να χρησιμοποιεί τη Office 365 για Mac, έκδοση προϊόντος 16.24 ή νεότερη.</span><span class="sxs-lookup"><span data-stu-id="9aab5-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>