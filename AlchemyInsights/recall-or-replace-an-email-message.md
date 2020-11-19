---
title: Ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353506"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="ce88f-102">Ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου στο Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ce88f-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="ce88f-103">Μπορείτε να **ανακαλέσετε μόνο τα μηνύματα που αποστέλλονται στα άτομα της εταιρείας σας**.</span><span class="sxs-lookup"><span data-stu-id="ce88f-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ce88f-104">Για παράδειγμα, εάν το μήνυμα στάλθηκε σε μια διεύθυνση Gmail, δεν μπορείτε να το ανακαλέσετε.</span><span class="sxs-lookup"><span data-stu-id="ce88f-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="ce88f-105">Μπορείτε να **ανακαλέσετε μόνο τα μηνύματα που αποστέλλονται από το Outlook για τον υπολογιστή**.</span><span class="sxs-lookup"><span data-stu-id="ce88f-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="ce88f-106">Εάν ένας χρήστης στείλει ένα μήνυμα χρησιμοποιώντας το Outlook για Mac ή το Outlook στο Web, δεν μπορείτε να το ανακαλέσετε.</span><span class="sxs-lookup"><span data-stu-id="ce88f-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="ce88f-107">Ως διαχειριστής μισθωτών, μπορείτε να **ανακαλέσετε μηνύματα εκ μέρους των χρηστών χρησιμοποιώντας το PowerShell** (για περισσότερες πληροφορίες, ανατρέξτε στο θέμα: [Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="ce88f-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="ce88f-108">Δεν μπορείτε να ανακαλέσετε μηνύματα από το κέντρο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="ce88f-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="ce88f-109">Κάντε κύλιση προς τα κάτω στην επιλογή "Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στην εταιρεία σας" για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="ce88f-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="ce88f-110">**Ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου που στείλατε**</span><span class="sxs-lookup"><span data-stu-id="ce88f-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="ce88f-111">Στο παράθυρο φακέλων στα αριστερά του παραθύρου του Outlook, επιλέξτε το φάκελο Απεσταλμένα.</span><span class="sxs-lookup"><span data-stu-id="ce88f-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="ce88f-112">Ανοίξτε το μήνυμα που θέλετε να ανακαλέσετε.</span><span class="sxs-lookup"><span data-stu-id="ce88f-112">Open the message that you want to recall.</span></span> <span data-ttu-id="ce88f-113">Πρέπει να κάνετε διπλό κλικ για να ανοίξετε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="ce88f-113">You must double-click to open the message.</span></span> <span data-ttu-id="ce88f-114">Η επιλογή του μηνύματος έτσι ώστε να εμφανίζεται στο παράθυρο ανάγνωσης δεν θα σας επιτρέψει να ανακαλέσετε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="ce88f-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="ce88f-115">Από την καρτέλα "μήνυμα", επιλέξτε " **ενέργειες**"  >  **ανάκληση αυτού του μηνύματος**.</span><span class="sxs-lookup"><span data-stu-id="ce88f-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="ce88f-116">Επιλέξτε **Διαγραφή μη αναγνωσμένων αντιγράφων αυτού του μηνύματος** ή **Διαγραφή μη αναγνωσμένων αντιγράφων και αντικατάσταση με ένα νέο μήνυμα** και, στη συνέχεια, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="ce88f-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="ce88f-117">Εάν στέλνετε ένα μήνυμα αντικατάστασης, συνθέστε το μήνυμα και, στη συνέχεια, επιλέξτε **Αποστολή**.</span><span class="sxs-lookup"><span data-stu-id="ce88f-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="ce88f-118">Η επιτυχία ή η αποτυχία μιας ανάκλησης μηνύματος εξαρτάται από τις ρυθμίσεις των παραληπτών στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="ce88f-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="ce88f-119">Για περισσότερες πληροφορίες, καθώς και για τον τρόπο ελέγχου της ανάκλησης, ανατρέξτε στο θέμα [ανάκληση ή αντικατάσταση μηνύματος ηλεκτρονικού ταχυδρομείου που στείλατε](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="ce88f-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ce88f-120">**_Για να αναζητήσετε και να διαγράψετε μηνύματα ηλεκτρονικού ταχυδρομείου στην εταιρεία σας_**, είναι πιο εύκολο εάν είστε καθολικός διαχειριστής. Εάν δεν είστε καθολικός διαχειριστής, ο λογαριασμός σας πρέπει να προστεθεί στην ομάδα ρόλων της διαχείρισης ανακάλυψης ή στο ρόλο διαχείρισης αναζήτησης συμμόρφωσης.</span><span class="sxs-lookup"><span data-stu-id="ce88f-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="ce88f-121">Για να διαγράψετε μηνύματα, θα πρέπει να γίνετε μέλος της ομάδας ρόλου διαχείρισης εταιρείας ή του ρόλου διαχείρισης αναζήτησης και εκκαθάρισης.</span><span class="sxs-lookup"><span data-stu-id="ce88f-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ce88f-122">Τα δικαιώματα για αυτούς τους ρόλους εκχωρούνται στο [Κέντρο συμμόρφωσης & ασφαλείας](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ce88f-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="ce88f-123">[Δημιουργήστε μια αναζήτηση περιεχομένου](https://docs.microsoft.com/microsoft-365/compliance/content-search) για να βρείτε το μήνυμα που θα διαγραφεί.</span><span class="sxs-lookup"><span data-stu-id="ce88f-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="ce88f-124">[Σύνδεση με το κέντρο συμμόρφωσης του & ασφαλείας PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ce88f-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="ce88f-125">Εάν χρησιμοποιείτε το ΣΠΙ (έλεγχος ταυτότητας πολλών παραγόντων), ανατρέξτε [στο θέμα σύνδεση στο Microsoft 365 Security & κέντρο συμμόρφωσης PowerShell με χρήση ελέγχου ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ce88f-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
