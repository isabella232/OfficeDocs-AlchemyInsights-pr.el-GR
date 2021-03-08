---
title: Ορισμός του ClientAccessServerEnabled σε True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524557"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="7f8fc-102">Ορισμός του ClientAccessServerEnabled σε True</span><span class="sxs-lookup"><span data-stu-id="7f8fc-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="7f8fc-103">Εάν δεν μπορείτε να ανοίξετε ένα κρυπτογραφημένο μήνυμα ηλεκτρονικού ταχυδρομείου και αντί για αυτό δείτε ένα **συνημμένο rpmsg,** εκτελέστε τα ακόλουθα βήματα:</span><span class="sxs-lookup"><span data-stu-id="7f8fc-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="7f8fc-104">Συνδεθείτε στο Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="7f8fc-105">Για να συνδεθείτε στο Exchange Online PowerShell, πρέπει να εισέλθετε χρησιμοποιώντας έναν καθολικό διαχειριστή ή ένα λογαριασμό διαχειριστή του Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="7f8fc-106">a.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-106">a.</span></span> <span data-ttu-id="7f8fc-107">Ανοίξτε το Windows PowerShell και, στη συνέχεια, εκτελέστε την ακόλουθη εντολή: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="7f8fc-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="7f8fc-108">b.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-108">b.</span></span> <span data-ttu-id="7f8fc-109">Στο παράθυρο διαλόγου **"Αίτηση διαπιστευτηρίων" του Windows PowerShell,** εισαγάγετε τον λογαριασμό εργασίας ή το σχολείο σας και τον κωδικό πρόσβασης, γ.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="7f8fc-110">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-110">Click **OK**.</span></span> 

2. <span data-ttu-id="7f8fc-111">Εκτελέστε την ακόλουθη εντολή για να δημιουργήσετε μια νέα περίοδο λειτουργίας:</span><span class="sxs-lookup"><span data-stu-id="7f8fc-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="7f8fc-112">a.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-112">a.</span></span> <span data-ttu-id="7f8fc-113">Εκτελέστε την παρακάτω εντολή:</span><span class="sxs-lookup"><span data-stu-id="7f8fc-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="7f8fc-114">Εντολή `Get-IRMConfiguration` "Εκτέλεση".</span><span class="sxs-lookup"><span data-stu-id="7f8fc-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="7f8fc-115">Ελέγξτε τη **ρύθμιση ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="7f8fc-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="7f8fc-116">a.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-116">a.</span></span> <span data-ttu-id="7f8fc-117">Εάν **η ρύθμιση ClientAccessServerEnabled** έχει οριστεί σε **False,** εκτελέστε το ακόλουθο cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="7f8fc-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="7f8fc-118">Κλείνετε πάντα την περίοδο λειτουργίας του PowerShell με την ακόλουθη εντολή: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="7f8fc-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="7f8fc-119">Για περισσότερες πληροφορίες, ανατρέξτε [στο Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="7f8fc-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

