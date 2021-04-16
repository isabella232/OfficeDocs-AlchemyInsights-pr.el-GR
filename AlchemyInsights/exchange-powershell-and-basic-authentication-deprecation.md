---
title: Exchange PowerShell και απόσυρση βασικού ελέγχου ταυτότητας
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813472"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="b6f06-102">Exchange PowerShell και απόσυρση βασικού ελέγχου ταυτότητας</span><span class="sxs-lookup"><span data-stu-id="b6f06-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="b6f06-103">Για τις πιο πρόσφατες πληροφορίες σχετικά με το πώς μπορείτε να συνδεθείτε στο Exchange Online PowerShell χωρίς τη χρήση Βασικού ελέγχου ταυτότητας, [μεταβείτε εδώ](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="b6f06-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="b6f06-104">Η λειτουργική μονάδα v2 PowerShell δεν κάνει χρήση βασικού ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="b6f06-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="b6f06-105">Σημειώστε ότι ο βασικός έλεγχος ταυτότητας εξακολουθεί να πρέπει να είναι ενεργοποιημένος στον υπολογιστή-πελάτη σας.</span><span class="sxs-lookup"><span data-stu-id="b6f06-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="b6f06-106">Η νέα λειτουργική μονάδα v2 PowerShell χρησιμοποιεί τον σύγχρονο έλεγχο ταυτότητας για να δημιουργήσει σύνδεση για την ενεργοποίηση όλων των cmdlet v2 που βασίζονται στο REST.</span><span class="sxs-lookup"><span data-stu-id="b6f06-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="b6f06-107">Επιπλέον των cmdlets v2, σάς επιτρέπει να έχετε πρόσβαση σε παλαιότερες cmdlet απομακρυσμένης σύνδεσης PowerShell (RPS) για τα οποία απαιτείται η δημιουργία απομακρυσμένης περιόδου λειτουργίας PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b6f06-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="b6f06-108">Η δημιουργία μιας περιόδου λειτουργίας RPS στον υπολογιστή με Windows απαιτεί την ενεργοποίηση του WinRM BasicAuth στον υπολογιστή-πελάτη, παρόλο που η λειτουργική μονάδα χρησιμοποιεί τον σύγχρονο μηχανισμό ελέγχου ταυτότητας για τον έλεγχο ταυτότητας στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="b6f06-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="b6f06-109">Η διοχέτευση βασικού ελέγχου ταυτότητας WinRM χρησιμοποιείται για τη μεταφορά διακριτικών σύγχρονου ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="b6f06-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="b6f06-110">Εάν ο βασικός έλεγχος ταυτότητας WinRM έχει απενεργοποιηθεί στον υπολογιστή-πελάτη, τα νέα cmdlets v2 θα συνεχίσουν να λειτουργούν (αλλά οι παλαιότερες cmdlet RPS δεν θα λειτουργούν).</span><span class="sxs-lookup"><span data-stu-id="b6f06-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
