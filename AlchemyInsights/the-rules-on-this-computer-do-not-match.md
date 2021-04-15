---
title: 'Σφάλμα: Οι κανόνες σε αυτόν τον υπολογιστή δεν συμφωνούν'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782952"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="6e243-102">Σφάλμα: Οι κανόνες σε αυτόν τον υπολογιστή δεν συμφωνούν</span><span class="sxs-lookup"><span data-stu-id="6e243-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="6e243-103">Για να δείτε την ενημερωμένη κατάσταση αυτού του γνωστού προβλήματος, ανατρέξτε στο θέμα Οι κανόνες σε αυτόν τον υπολογιστή [δεν συμφωνούν με τους κανόνες στο Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="6e243-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="6e243-104">Η ομάδα του Outlook έχει εφαρμόσει μια επιδιόρθωση στη Δόμηση 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="6e243-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="6e243-105">Η επιδιόρθωση βρίσκεται ήδη στο Insider Fast και θα μεταβεί στο Μηνιαίο κανάλι στα τέλη Ιουνίου 2020.</span><span class="sxs-lookup"><span data-stu-id="6e243-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="6e243-106">Αφού έχετε τη διορθώθηκε η έκδοση, μπορεί να εμφανιστεί το μήνυμα "Ποιοι κανόνες θέλετε να διατηρήσετε" για τελευταία φορά.</span><span class="sxs-lookup"><span data-stu-id="6e243-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="6e243-107">Επιλέξτε "Διακομιστής" όταν σας ζητηθεί και, στη συνέχεια, μεταβείτε ξανά στο Outlook και ενεργοποιήστε ξανά τυχόν κανόνες που ήταν απενεργοποιημένες.</span><span class="sxs-lookup"><span data-stu-id="6e243-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="6e243-108">Μέχρι να γίνει διαθέσιμη η επιδιόρθωση, χρησιμοποιήστε την παρακάτω λύση:</span><span class="sxs-lookup"><span data-stu-id="6e243-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="6e243-109">**Λύση:** Στις πρόσφατες αναφορές, το πρόβλημα παρουσιάστηκε για εκείνους που έχουν δημιουργήσει μόνο κανόνες προγράμματος-πελάτη στο Outlook για υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="6e243-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="6e243-110">Εάν συνεχίσετε να παρουσιάζεται το πρόβλημα, εξετάστε το ενδεχόμενο να διαγράψετε τους κανόνες και, στη συνέχεια, να δημιουργήσετε και να επεξεργαστείτε κανόνες μόνο στο OWA (Outlook Web App) μέχρι να επιλυθεί το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="6e243-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="6e243-111">Εάν δεν μπορείτε να διαγράψετε τους κανόνες με μη αυτόματο τρόπο, μπορείτε να εκτελέσετε μια εντολή του Outlook κατά την εκκίνηση του Outlook εκτελώντας Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="6e243-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="6e243-112">Αυτό θα διαγράψει τόσο τους κανόνες προγράμματος-πελάτη όσο και τους κανόνες διακομιστή.</span><span class="sxs-lookup"><span data-stu-id="6e243-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="6e243-113">Θα διαγράψει όλους τους κανόνες για όλους τους λογαριασμούς στο προφίλ του Outlook.</span><span class="sxs-lookup"><span data-stu-id="6e243-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="6e243-114">Αυτή η εντολή τεκμηριωθεί περαιτέρω στο άρθρο "Διακόπτες γραμμής εντολών".</span><span class="sxs-lookup"><span data-stu-id="6e243-114">This command is further documented in the Command-line switches article.</span></span>

