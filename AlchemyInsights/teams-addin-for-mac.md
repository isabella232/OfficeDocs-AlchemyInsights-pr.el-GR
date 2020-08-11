---
title: Πρόσθετο "ομάδες" για Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629575"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="9d2ec-102">Πρόσθετο "ομάδες" για Mac</span><span class="sxs-lookup"><span data-stu-id="9d2ec-102">Teams add-in for Mac</span></span>

<span data-ttu-id="9d2ec-103">Για να αντιμετωπίσετε ένα πρόσθετο που λείπει από τις ομάδες για τους χρήστες του λειτουργικού συστήματος για Mac, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="9d2ec-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="9d2ec-104">**Βήμα 1:** Εάν έχετε υβριδική Exchange εσωτερικής εγκατάστασης (2016 CU3 ή νεότερη έκδοση), χρησιμοποιήστε το εργαλείο Test-HMA.ps1 για να επιβεβαιώσετε ότι έχει ρυθμιστεί σωστά ο υβριδικός σύγχρονος έλεγχος ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="9d2ec-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="9d2ec-105">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [επικύρωση υβριδικών σύγχρονων ρυθμίσεων ελέγχου ταυτότητας για το Outlook για iOS και Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="9d2ec-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="9d2ec-106">**Σημείωση** Χρήση της μορφής διεύθυνσης UPN (για παράδειγμα, [username@contoso.com](mailto:username@contoso.com)), όχι DOMAIN\username.</span><span class="sxs-lookup"><span data-stu-id="9d2ec-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="9d2ec-107">Κάντε αυτό ακόμα και για τους χρήστες με γραμματοκιβώτια του Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9d2ec-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="9d2ec-108">**Βήμα 2:** Ζητήστε από το χρήστη να **Tools**μετακινήσει σε  >  **λογαριασμούς**εργαλείων... στο Outlook για Mac και εντοπίστε και επιλέξτε το λογαριασμό.</span><span class="sxs-lookup"><span data-stu-id="9d2ec-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="9d2ec-109">Επιβεβαιώστε ότι το όνομα χρήστη που παρατίθεται είναι σε μορφή UPN (για παράδειγμα, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="9d2ec-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="9d2ec-110">**Βήμα 3:** Επιβεβαιώστε ότι ο χρήστης είναι ένας χρήστης με άδεια χρήσης του Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="9d2ec-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="9d2ec-111">Ο χρήστης πρέπει να χρησιμοποιεί τη συνδρομή του Office 365 για Mac, έκδοση προϊόντος 16,24 ή νεότερη.</span><span class="sxs-lookup"><span data-stu-id="9d2ec-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>