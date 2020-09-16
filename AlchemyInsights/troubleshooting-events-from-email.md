---
title: Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658734"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="a6b2c-102">Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο</span><span class="sxs-lookup"><span data-stu-id="a6b2c-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="a6b2c-103">Επαλήθευση ότι η δυνατότητα είναι ενεργοποιημένη για το γραμματοκιβώτιο: **Get-EventsFromEmailConfiguration- <mailbox> Identity**</span><span class="sxs-lookup"><span data-stu-id="a6b2c-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="a6b2c-104">Στη συνέχεια, δείτε τα "συμβάντα από το ηλεκτρονικό ταχυδρομείο" logs **export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="a6b2c-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="a6b2c-105">Στα αρχεία καταγραφής "συμβάντα από το ηλεκτρονικό ταχυδρομείο", εντοπίστε το InternetMessageId που ταιριάζει με το στοιχείο στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="a6b2c-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="a6b2c-106">Το TrustScore προσδιορίζει εάν το στοιχείο προστίθεται ή όχι.</span><span class="sxs-lookup"><span data-stu-id="a6b2c-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="a6b2c-107">Τα συμβάντα θα προστεθούν μόνο εάν το TrustScore = "αξιόπιστες".</span><span class="sxs-lookup"><span data-stu-id="a6b2c-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="a6b2c-108">Το TrustScore καθορίζεται από τις ιδιότητες SPF, DKIM ή DMARC, οι οποίες βρίσκονται στην κεφαλίδα του μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="a6b2c-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="a6b2c-109">Για να προβάλετε αυτές τις ιδιότητες:</span><span class="sxs-lookup"><span data-stu-id="a6b2c-109">To view these properties:</span></span>

<span data-ttu-id="a6b2c-110">**Outlook υπολογιστή**</span><span class="sxs-lookup"><span data-stu-id="a6b2c-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="a6b2c-111">Άνοιγμα του στοιχείου</span><span class="sxs-lookup"><span data-stu-id="a6b2c-111">Open the item</span></span>
- <span data-ttu-id="a6b2c-112">Ιδιότητες αρχείου->-> κεφαλίδες Internet</span><span class="sxs-lookup"><span data-stu-id="a6b2c-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="a6b2c-113">ή</span><span class="sxs-lookup"><span data-stu-id="a6b2c-113">or</span></span>

<span data-ttu-id="a6b2c-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="a6b2c-114">**MFCMapi**</span></span>

- <span data-ttu-id="a6b2c-115">Μετάβαση στο στοιχείο στο φάκελο "Εισερχόμενα"</span><span class="sxs-lookup"><span data-stu-id="a6b2c-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="a6b2c-116">Αναζητήστε PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="a6b2c-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="a6b2c-117">Αυτές οι ιδιότητες καθορίζονται και καταγράφονται κατά τη μεταφορά και τη δρομολόγηση.</span><span class="sxs-lookup"><span data-stu-id="a6b2c-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="a6b2c-118">Για περαιτέρω αντιμετώπιση προβλημάτων, ίσως χρειαστεί να παρακολουθήσετε με την υποστήριξη μεταφορών τις αποτυχίες στο θέμα SPF, DKIM και. ή DMARC.</span><span class="sxs-lookup"><span data-stu-id="a6b2c-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>