---
title: Exchange PowerShell και απόσυρση βασικού ελέγχου ταυτότητας
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015689"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="8758d-102">Exchange PowerShell και απόσυρση βασικού ελέγχου ταυτότητας</span><span class="sxs-lookup"><span data-stu-id="8758d-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="8758d-103">Για τις πιο πρόσφατες πληροφορίες σχετικά με το πώς μπορείτε να συνδεθείτε στο Exchange Online PowerShell χωρίς τη χρήση Βασικού ελέγχου ταυτότητας, [μεταβείτε εδώ](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="8758d-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="8758d-104">Σημειώστε ότι ο βασικός έλεγχος ταυτότητας εξακολουθεί να πρέπει να είναι ενεργοποιημένος στον υπολογιστή-πελάτη σας.</span><span class="sxs-lookup"><span data-stu-id="8758d-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="8758d-105">Η νέα λειτουργική μονάδα v2 PowerShell χρησιμοποιεί τον σύγχρονο έλεγχο ταυτότητας για να δημιουργήσει σύνδεση για την ενεργοποίηση όλων των cmdlet v2 που βασίζονται στο REST.</span><span class="sxs-lookup"><span data-stu-id="8758d-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="8758d-106">Επιπλέον των cmdlets v2, σάς επιτρέπει να έχετε πρόσβαση σε παλαιότερες cmdlet απομακρυσμένης σύνδεσης PowerShell (RPS) για τα οποία απαιτείται η δημιουργία απομακρυσμένης περιόδου λειτουργίας PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8758d-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="8758d-107">Η δημιουργία μιας περιόδου λειτουργίας RPS στον υπολογιστή με Windows απαιτεί την ενεργοποίηση του WinRM BasicAuth στον υπολογιστή-πελάτη, παρόλο που η λειτουργική μονάδα χρησιμοποιεί τον σύγχρονο μηχανισμό ελέγχου ταυτότητας για τον έλεγχο ταυτότητας στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="8758d-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="8758d-108">Η διοχέτευση βασικού ελέγχου ταυτότητας WinRM χρησιμοποιείται για τη μεταφορά διακριτικών σύγχρονου ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="8758d-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="8758d-109">Εάν ο βασικός έλεγχος ταυτότητας WinRM έχει απενεργοποιηθεί στον υπολογιστή-πελάτη, τα νέα cmdlets v2 θα συνεχίσουν να λειτουργούν (αλλά οι παλαιότερες cmdlet RPS δεν θα λειτουργούν).</span><span class="sxs-lookup"><span data-stu-id="8758d-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
