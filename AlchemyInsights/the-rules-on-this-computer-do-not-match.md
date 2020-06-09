---
title: 'Σφάλμα: Οι κανόνες σε αυτόν τον υπολογιστή δεν ταιριάζουν'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618007"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="d48b2-102">Σφάλμα: Οι κανόνες σε αυτόν τον υπολογιστή δεν ταιριάζουν</span><span class="sxs-lookup"><span data-stu-id="d48b2-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="d48b2-103">Για να δείτε την ενημερωμένη κατάσταση αυτού του γνωστού ζητήματος, ανατρέξτε στο θέμα [Οι κανόνες σε αυτόν τον υπολογιστή δεν ταιριάζουν με τους κανόνες στο Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="d48b2-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="d48b2-104">Η ομάδα του Outlook έχει εφαρμόσει μια ενημέρωση κώδικα στο Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="d48b2-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="d48b2-105">Η ενημέρωση κώδικα είναι ήδη στο Insider Fast και θα πάει στο Μηνιαίο Κανάλι στα τέλη Ιουνίου 2020.</span><span class="sxs-lookup"><span data-stu-id="d48b2-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="d48b2-106">Μόλις έχετε τη σταθερή κατασκευή μπορείτε να πάρετε την προτροπή "Ποιους κανόνες θέλετε να κρατήσετε" για τελευταία φορά.</span><span class="sxs-lookup"><span data-stu-id="d48b2-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="d48b2-107">Επιλέξτε Server όταν σας ζητηθεί και, στη συνέχεια, επιστρέψτε στο Outlook και ενεργοποιήστε ξανά τους κανόνες που ήταν απενεργοποιημένοι.</span><span class="sxs-lookup"><span data-stu-id="d48b2-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="d48b2-108">Μέχρι να είναι διαθέσιμη η ενημέρωση κώδικα, χρησιμοποιήστε τον ακόλουθο εναλλακτικό τρόπο:</span><span class="sxs-lookup"><span data-stu-id="d48b2-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="d48b2-109">**Λύση:** Σε πρόσφατες αναφορές, το ζήτημα παρουσιάστηκε για εκείνους που έχουν δημιουργήσει μόνο κανόνες προγράμματος-πελάτη στην επιφάνεια εργασίας του Outlook.</span><span class="sxs-lookup"><span data-stu-id="d48b2-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="d48b2-110">Εάν συνεχίσετε να αντιμετωπίσετε το πρόβλημα, εξετάστε το ενδεχόμενο να διαγραφούν οι κανόνες και, στη συνέχεια, να δημιουργήσετε και να επεξεργαστείτε κανόνες μόνο στο OWA (Outlook Web App) μέχρι να επιλυθεί το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="d48b2-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="d48b2-111">Εάν δεν μπορείτε να διαγράψετε τους κανόνες με μη αυτόματο τρόπο, μπορείτε να εκτελέσετε μια εντολή του Outlook κατά την εκκίνηση του Outlook εκτελώντας κανόνες /cleanrules του Outlook.exe.</span><span class="sxs-lookup"><span data-stu-id="d48b2-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="d48b2-112">Αυτό θα διαγράψει τόσο τους κανόνες του υπολογιστή-πελάτη όσο και του διακομιστή.</span><span class="sxs-lookup"><span data-stu-id="d48b2-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="d48b2-113">Θα διαγράψει όλους τους κανόνες για όλους τους λογαριασμούς στο προφίλ του Outlook.</span><span class="sxs-lookup"><span data-stu-id="d48b2-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="d48b2-114">Αυτή η εντολή τεκμηριώνεται περαιτέρω στο άρθρο διακόπτες γραμμής εντολών.</span><span class="sxs-lookup"><span data-stu-id="d48b2-114">This command is further documented in the Command-line switches  article.</span></span>