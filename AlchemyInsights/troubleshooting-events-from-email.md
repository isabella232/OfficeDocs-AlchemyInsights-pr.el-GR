---
title: Αντιμετώπιση προβλημάτων συμβάντων από ηλεκτρονικό ταχυδρομείο
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569142"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="72e99-102">Αντιμετώπιση προβλημάτων συμβάντων από ηλεκτρονικό ταχυδρομείο</span><span class="sxs-lookup"><span data-stu-id="72e99-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="72e99-103">Επαλήθευση της δυνατότητας είναι ενεργοποιημένη για το γραμματοκιβώτιο: \*\*Get-EventsFromEmailConfiguration -Ταυτότητα <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="72e99-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="72e99-104">Στη συνέχεια, κοιτάξτε τα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο" **"Εξαγωγή-ΓραμματοκιβώτιοΔιαγνωστικά <mailbox> Logs-Προφίλ χρόνου στοιχείου"**</span><span class="sxs-lookup"><span data-stu-id="72e99-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="72e99-105">Στα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο", βρείτε το InternetMessageId που ταιριάζει με το στοιχείο στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="72e99-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="72e99-106">Το TrustScore καθορίζει εάν το στοιχείο έχει προστεθεί ή όχι.</span><span class="sxs-lookup"><span data-stu-id="72e99-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="72e99-107">Τα συμβάντα θα προστεθούν μόνο αν το TrustScore = "Αξιόπιστο".</span><span class="sxs-lookup"><span data-stu-id="72e99-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="72e99-108">Το TrustScore καθορίζεται από τις ιδιότητες SPF, Dkim ή Dmarc, οι οποίες βρίσκονται στην κεφαλίδα μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="72e99-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="72e99-109">Για να προβάλετε αυτές τις ιδιότητες:</span><span class="sxs-lookup"><span data-stu-id="72e99-109">To view these properties:</span></span>

<span data-ttu-id="72e99-110">**Επιφάνεια εργασίας outlook**</span><span class="sxs-lookup"><span data-stu-id="72e99-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="72e99-111">Άνοιγμα του στοιχείου</span><span class="sxs-lookup"><span data-stu-id="72e99-111">Open the item</span></span>
- <span data-ttu-id="72e99-112">Αρχείο -ιδιότητες > -> κεφαλίδες Internet</span><span class="sxs-lookup"><span data-stu-id="72e99-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="72e99-113">Ή</span><span class="sxs-lookup"><span data-stu-id="72e99-113">or</span></span>

<span data-ttu-id="72e99-114">**Mfcmapi**</span><span class="sxs-lookup"><span data-stu-id="72e99-114">**MFCMapi**</span></span>

- <span data-ttu-id="72e99-115">Μετάβαση στο στοιχείο στα εισερχόμενα</span><span class="sxs-lookup"><span data-stu-id="72e99-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="72e99-116">Ψάξτε για PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="72e99-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="72e99-117">Αυτές οι ιδιότητες προσδιορίζονται και καταγράφονται κατά τη μεταφορά και τη δρομολόγηση.</span><span class="sxs-lookup"><span data-stu-id="72e99-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="72e99-118">Για περαιτέρω αντιμετώπιση προβλημάτων, ίσως χρειαστεί να παρακολουθήσετε με την Υποστήριξη μεταφορών σχετικά με τις αποτυχίες σε SPF, DKIM και.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="72e99-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>