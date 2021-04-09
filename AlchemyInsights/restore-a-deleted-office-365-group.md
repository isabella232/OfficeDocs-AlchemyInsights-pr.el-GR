---
title: Επαναφορά διαγραμμένης ομάδας Του Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645131"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="51db9-102">Επαναφορά διαγραμμένης ομάδας Του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="51db9-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="51db9-103">Μπορείτε να επαναφέρετε μια διαγραμμένη ομάδα του Microsoft 365 ή το Microsoft Teams εντός 30 ημερών από τη διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="51db9-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="51db9-104">Μεταβείτε στο [κέντρο διαχείρισης του Microsoft 365](https://aka.ms/RestoreDeletedGroup) για να συνδεθείτε σε μια λίστα με τις ομάδες και τις ομάδες που έχετε διαγράψει.</span><span class="sxs-lookup"><span data-stu-id="51db9-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="51db9-105">**Σημείωση:** Συνδεθείτε χρησιμοποιώντας το λογαριασμό που έχει εκχωρηθεί στο διαχειριστή του μισθωτή ή στο ρόλο διαχειριστή ομάδων.</span><span class="sxs-lookup"><span data-stu-id="51db9-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="51db9-106">Επιλέξτε τη διαγραμμένη ομάδα του Microsoft 365/Teams για επαναφορά και κάντε κλικ στην επιλογή **"Επαναφορά ομάδας".**</span><span class="sxs-lookup"><span data-stu-id="51db9-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="51db9-107">Εάν δεν είναι δυνατή η επαναφορά της ομάδας λόγω μιας διεύθυνσης SMTP σε διένεξη, χρησιμοποιήστε την ακόλουθη εντολή για να βρείτε το αντικείμενο που προκαλεί διένεξη και να καταργήσετε τη διεύθυνση SMTP:</span><span class="sxs-lookup"><span data-stu-id="51db9-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="51db9-108">**Σημείωση:** Σε ορισμένες περιπτώσεις, μπορεί να διαρκέσει έως και 24 ώρες για την επαναφορά της ομάδας και όλων των δεδομένων της.</span><span class="sxs-lookup"><span data-stu-id="51db9-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="51db9-109">Για περισσότερες πληροφορίες ή για να μάθετε πώς μπορείτε να επαναφέρετε ομάδες χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα [Επαναφορά διαγραμμένης ομάδας του Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="51db9-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>