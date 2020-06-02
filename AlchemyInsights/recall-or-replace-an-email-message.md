---
title: Ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509456"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="bc867-102">Ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου στο Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bc867-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="bc867-103">Μπορείτε να **ανακαλέσετε μόνο μηνύματα που αποστέλλονται σε άτομα στον οργανισμό σας**.</span><span class="sxs-lookup"><span data-stu-id="bc867-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="bc867-104">Εάν το μήνυμα στάλθηκε σε μια διεύθυνση Gmail, για παράδειγμα, δεν μπορείτε να το θυμηθείτε.</span><span class="sxs-lookup"><span data-stu-id="bc867-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="bc867-105">Μπορείτε να **ανακαλέσετε μόνο μηνύματα που αποστέλλονται από το Outlook 2016 για τον υπολογιστή**.</span><span class="sxs-lookup"><span data-stu-id="bc867-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="bc867-106">Εάν ένας χρήστης στείλει ένα μήνυμα χρησιμοποιώντας το Outlook για Mac ή το Outlook στο web, δεν μπορείτε να το θυμηθείτε.</span><span class="sxs-lookup"><span data-stu-id="bc867-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="bc867-107">Εάν είστε διαχειριστής, μπορείτε να **ανακαλέσετε μηνύματα εκ μέρους των χρηστών χρησιμοποιώντας το PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="bc867-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="bc867-108">Δεν μπορείτε να ανακαλέσετε μηνύματα από το κέντρο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="bc867-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="bc867-109">Κάντε κύλιση προς τα κάτω στην επιλογή "Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας" για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="bc867-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="bc867-110">**Ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου που στείλατε**</span><span class="sxs-lookup"><span data-stu-id="bc867-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="bc867-111">Στο παράθυρο φακέλων στα αριστερά του παραθύρου του Outlook, επιλέξτε το φάκελο "Απεσταλμένα".</span><span class="sxs-lookup"><span data-stu-id="bc867-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="bc867-112">Ανοίξτε το μήνυμα που θέλετε να ανακαλέσετε.</span><span class="sxs-lookup"><span data-stu-id="bc867-112">Open the message that you want to recall.</span></span> <span data-ttu-id="bc867-113">Πρέπει να κάνετε διπλό κλικ για να ανοίξετε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="bc867-113">You must double-click to open the message.</span></span> <span data-ttu-id="bc867-114">Η επιλογή του μηνύματος ώστε να εμφανίζεται στο παράθυρο ανάγνωσης δεν θα σας επιτρέψει να ανακαλέσετε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="bc867-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="bc867-115">Από την καρτέλα Μήνυμα, επιλέξτε **Ενέργειες**  >  **ανάκλησης αυτού του μηνύματος**.</span><span class="sxs-lookup"><span data-stu-id="bc867-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="bc867-116">Επιλέξτε **Διαγραφή μη αναγνωσμένων αντιγράφων αυτού του μηνύματος** ή Διαγραφή μη **αναγνωσμένων αντιγράφων και αντικατάσταση με νέο μήνυμα**και, στη συνέχεια, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="bc867-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="bc867-117">Εάν στέλνετε ένα μήνυμα αντικατάστασης, συνθέστε το μήνυμα και, στη συνέχεια, επιλέξτε **Αποστολή**.</span><span class="sxs-lookup"><span data-stu-id="bc867-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="bc867-118">Η επιτυχία ή αποτυχία μιας ανάκλησης μηνύματος εξαρτάται από τις ρυθμίσεις των παραληπτών στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="bc867-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="bc867-119">Για περισσότερες πληροφορίες, συμπεριλαμβανομένου του τρόπου ελέγχου της ανάκλησης, ανατρέξτε στο θέμα [Ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου που στείλατε](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="bc867-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="bc867-120">***Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας*** Για να αναζητήσετε και να διαγράψετε μηνύματα ηλεκτρονικού ταχυδρομείου στον οργανισμό σας, είναι πιο εύκολο αν είστε καθολικός διαχειριστής. Εάν δεν είστε καθολικός διαχειριστής, ο λογαριασμός σας πρέπει να προστεθεί στην ομάδα ρόλων του EDiscovery Manager ή στο ρόλο διαχείρισης αναζήτησης συμμόρφωσης.</span><span class="sxs-lookup"><span data-stu-id="bc867-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="bc867-121">Για να διαγράψετε μηνύματα, θα πρέπει να συμμετάσχετε στην ομάδα ρόλων "Διαχείριση οργανισμού" ή στο ρόλο διαχείρισης αναζήτησης και εκκαθάρισης.</span><span class="sxs-lookup"><span data-stu-id="bc867-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="bc867-122">Τα δικαιώματα για αυτούς τους ρόλους εκχωρούνται στο [κέντρο συμμόρφωσης & ασφαλείας](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="bc867-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="bc867-123">[Δημιουργήστε μια αναζήτηση περιεχομένου](https://docs.microsoft.com/microsoft-365/compliance/content-search) για να βρείτε το μήνυμα προς διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="bc867-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="bc867-124">[Σύνδεση στο PowerShell του Κέντρου συμμόρφωσης & ασφάλειας](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="bc867-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="bc867-125">Εάν χρησιμοποιείτε ΣΠΙ, ανατρέξτε στο θέμα [Σύνδεση με ασφάλεια microsoft 365 & PowerShell του Κέντρου συμμόρφωσης που χρησιμοποιεί έλεγχο ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="bc867-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
