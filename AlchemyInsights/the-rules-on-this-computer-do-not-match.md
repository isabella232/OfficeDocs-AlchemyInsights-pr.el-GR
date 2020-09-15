---
title: 'Σφάλμα: οι κανόνες σε αυτόν τον υπολογιστή δεν συμφωνούν'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690963"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="34bbc-102">Σφάλμα: οι κανόνες σε αυτόν τον υπολογιστή δεν συμφωνούν</span><span class="sxs-lookup"><span data-stu-id="34bbc-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="34bbc-103">Για να δείτε την ενημερωμένη κατάσταση αυτού του γνωστού ζητήματος, ανατρέξτε [στο θέμα οι κανόνες σε αυτόν τον υπολογιστή δεν συμφωνούν με τους κανόνες στο Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="34bbc-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="34bbc-104">Η ομάδα του Outlook εφάρμοσε μια επιδιόρθωση στη δομή 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="34bbc-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="34bbc-105">Η επιδιόρθωση είναι ήδη στο Insider Fast και θα μετακινήσει σε μηνιαίο κανάλι στα τέλη Ιουνίου 2020.</span><span class="sxs-lookup"><span data-stu-id="34bbc-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="34bbc-106">Αφού έχετε τη σταθερή δομή, μπορεί να εμφανιστεί το μήνυμα "ποιους κανόνες θέλετε να διατηρήσετε" για τελευταία φορά.</span><span class="sxs-lookup"><span data-stu-id="34bbc-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="34bbc-107">Επιλέξτε διακομιστής όταν σας ζητηθεί και, στη συνέχεια, επιστρέψτε στο Outlook και ενεργοποιήστε ξανά τους κανόνες που έχουν απενεργοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="34bbc-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="34bbc-108">Μέχρι να είναι διαθέσιμη η επιδιόρθωση, χρησιμοποιήστε την παρακάτω λύση:</span><span class="sxs-lookup"><span data-stu-id="34bbc-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="34bbc-109">**Λύση**: στις πρόσφατες αναφορές, το πρόβλημα έχει προκύψει για τα άτομα που έχουν δημιουργήσει μόνο κανόνες προγράμματος-πελάτη στο Outlook Desktop.</span><span class="sxs-lookup"><span data-stu-id="34bbc-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="34bbc-110">Εάν εξακολουθείτε να αντιμετωπίζετε το πρόβλημα, εξετάστε το ενδεχόμενο να διαγράψετε τους κανόνες και, στη συνέχεια, να δημιουργήσετε και να επεξεργαστείτε κανόνες μόνο στο OWA (Outlook Web App) μέχρι να επιλυθεί το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="34bbc-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="34bbc-111">Εάν δεν μπορείτε να διαγράψετε τους κανόνες με μη αυτόματο τρόπο, μπορείτε να εκτελέσετε μια εντολή του Outlook κατά την εκκίνηση του Outlook εκτελώντας Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="34bbc-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="34bbc-112">Αυτή η ενέργεια θα διαγράψει τους κανόνες του προγράμματος-πελάτη και του διακομιστή.</span><span class="sxs-lookup"><span data-stu-id="34bbc-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="34bbc-113">Θα διαγράψει όλους τους κανόνες για όλους τους λογαριασμούς στο προφίλ του Outlook.</span><span class="sxs-lookup"><span data-stu-id="34bbc-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="34bbc-114">Αυτή η εντολή τεκμηριώνεται περαιτέρω στο άρθρο των διακοπτών της γραμμής εντολών.</span><span class="sxs-lookup"><span data-stu-id="34bbc-114">This command is further documented in the Command-line switches article.</span></span>

