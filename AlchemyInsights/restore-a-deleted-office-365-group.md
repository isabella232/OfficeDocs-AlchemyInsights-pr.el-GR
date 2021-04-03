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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505686"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="68438-102">Επαναφορά διαγραμμένης ομάδας Του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="68438-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="68438-103">Μπορείτε να επαναφέρετε μια διαγραμμένη ομάδα του Microsoft 365 ή το Microsoft Teams εντός 30 ημερών από τη διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="68438-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="68438-104">Για να συνδεθείτε στο Κέντρο διαχείρισης του Microsoft 365 και να παρατίθενται οι διαγραμμένες ομάδες και ομάδες, μεταβείτε στο Κέντρο διαχείρισης Microsoft [365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="68438-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="68438-105">**Σημείωση:** Συνδεθείτε χρησιμοποιώντας το λογαριασμό που έχει εκχωρηθεί στο διαχειριστή του μισθωτή ή στο ρόλο διαχειριστή ομάδων.</span><span class="sxs-lookup"><span data-stu-id="68438-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="68438-106">Επιλέξτε τη διαγραμμένη ομάδα του Microsoft 365/Teams για επαναφορά και κάντε κλικ στην επιλογή **"Επαναφορά ομάδας".**</span><span class="sxs-lookup"><span data-stu-id="68438-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="68438-107">Εάν δεν είναι δυνατή η επαναφορά της ομάδας λόγω μιας διεύθυνσης SMTP σε διένεξη, χρησιμοποιήστε την ακόλουθη εντολή για να βρείτε το αντικείμενο που προκαλεί διένεξη και να καταργήσετε τη διεύθυνση SMTP:</span><span class="sxs-lookup"><span data-stu-id="68438-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="68438-108">**Σημείωση:** Σε ορισμένες περιπτώσεις, μπορεί να διαρκέσει έως και 24 ώρες για την επαναφορά της ομάδας και όλων των δεδομένων της.</span><span class="sxs-lookup"><span data-stu-id="68438-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="68438-109">Για περισσότερες πληροφορίες ή για να μάθετε πώς μπορείτε να επαναφέρετε ομάδες χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα [Επαναφορά διαγραμμένης ομάδας του Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="68438-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>