---
title: Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834839"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="4c5a1-102">Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο</span><span class="sxs-lookup"><span data-stu-id="4c5a1-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="4c5a1-103">Βεβαιωθείτε ότι η δυνατότητα είναι ενεργοποιημένη για το γραμματοκιβώτιο: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="4c5a1-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="4c5a1-104">Στη συνέχεια, δείτε τα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="4c5a1-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="4c5a1-105">Στα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο", βρείτε το InternetMessageId που ταιριάζει με το στοιχείο στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="4c5a1-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="4c5a1-106">Ο "TrustScore" καθορίζει εάν το στοιχείο προστίθεται ή όχι.</span><span class="sxs-lookup"><span data-stu-id="4c5a1-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="4c5a1-107">Τα συμβάντα θα προστεθούν μόνο εάν το TrustScore = "Αξιόπιστο".</span><span class="sxs-lookup"><span data-stu-id="4c5a1-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="4c5a1-108">Το TrustScore καθορίζεται από τις ιδιότητες SPF, Dkim ή Dmarc, οι οποίες βρίσκονται στην κεφαλίδα του μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="4c5a1-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="4c5a1-109">Για να προβάλετε αυτές τις ιδιότητες:</span><span class="sxs-lookup"><span data-stu-id="4c5a1-109">To view these properties:</span></span>

<span data-ttu-id="4c5a1-110">**Outlook υπολογιστή**</span><span class="sxs-lookup"><span data-stu-id="4c5a1-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="4c5a1-111">Άνοιγμα του στοιχείου</span><span class="sxs-lookup"><span data-stu-id="4c5a1-111">Open the item</span></span>
- <span data-ttu-id="4c5a1-112">Αρχείο -> Ιδιότητες -> Κεφαλίδες Internet</span><span class="sxs-lookup"><span data-stu-id="4c5a1-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="4c5a1-113">ή</span><span class="sxs-lookup"><span data-stu-id="4c5a1-113">or</span></span>

<span data-ttu-id="4c5a1-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="4c5a1-114">**MFCMapi**</span></span>

- <span data-ttu-id="4c5a1-115">Μετάβαση στο στοιχείο στα Εισερχόμενα</span><span class="sxs-lookup"><span data-stu-id="4c5a1-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="4c5a1-116">Αναζητήστε PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="4c5a1-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="4c5a1-117">Αυτές οι ιδιότητες προσδιορίζονται και καταγράφονται κατά τη μεταφορά και δρομολόγηση.</span><span class="sxs-lookup"><span data-stu-id="4c5a1-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="4c5a1-118">Για περαιτέρω αντιμετώπιση προβλημάτων, ίσως χρειαστεί να παρακολουθήσετε την υποστήριξη μεταφοράς σχετικά με τις αποτυχίες στα SPF, DKIM και.ή DMARC.</span><span class="sxs-lookup"><span data-stu-id="4c5a1-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>