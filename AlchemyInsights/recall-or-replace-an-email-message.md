---
title: Ανάκληση ή αντικατάσταση ενός μηνύματος ηλεκτρονικού ταχυδρομείου
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 170fbd632f0289a45d9497ac26fbe7f90cf88318
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356597"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="11148-102">Ανάκληση ή αντικατάσταση ενός μηνύματος ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="11148-102">Recall or replace an email message</span></span>

- <span data-ttu-id="11148-103">Μπορείτε να κάνετε **μόνο ανάκληση μηνύματα, που αποστέλλονται σε άτομα στον οργανισμό σας**.</span><span class="sxs-lookup"><span data-stu-id="11148-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="11148-104">Αν το μήνυμα έχει σταλεί σε μια διεύθυνση Gmail, για παράδειγμα, δεν μπορείτε να θυμηθείτε το.</span><span class="sxs-lookup"><span data-stu-id="11148-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="11148-105">Μπορείτε να κάνετε **μόνο μήνυμα ανάκλησης που αποστέλλονται από το Outlook 2016 για PC**.</span><span class="sxs-lookup"><span data-stu-id="11148-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="11148-106">Εάν ένας χρήστης στέλνει ένα μήνυμα χρησιμοποιώντας το Outlook για Mac ή του Outlook στο web, δεν μπορείτε να την θυμηθείτε.</span><span class="sxs-lookup"><span data-stu-id="11148-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="11148-107">Εάν είστε ένας admin, μπορείτε να κάνετε **ανάκληση μηνυμάτων εκ μέρους των χρηστών, χρησιμοποιώντας PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="11148-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="11148-108">Δεν μπορείτε να θυμηθείτε τα μηνύματα από το Κέντρο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="11148-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="11148-109">Κάντε κύλιση προς τα κάτω "Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας" για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="11148-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="11148-110">***Ανάκληση ή αντικατάσταση ενός μηνύματος ηλεκτρονικού ταχυδρομείου που στείλατε***</span><span class="sxs-lookup"><span data-stu-id="11148-110">***Recall or replace an email message that you sent***</span></span>

1. <span data-ttu-id="11148-111">Στο παράθυρο φακέλων στην αριστερή πλευρά του παραθύρου του Outlook, επιλέξτε το φάκελο "Απεσταλμένα".</span><span class="sxs-lookup"><span data-stu-id="11148-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="11148-112">Ανοίξτε το μήνυμα που θέλετε να ανακαλέσετε.</span><span class="sxs-lookup"><span data-stu-id="11148-112">Open the message that you want to recall.</span></span> <span data-ttu-id="11148-113">Θα πρέπει να κάντε διπλό κλικ για να ανοίξετε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="11148-113">You must double-click to open the message.</span></span> <span data-ttu-id="11148-114">Επιλέγοντας το μήνυμα, έτσι ώστε να εμφανίζεται στο παράθυρο ανάγνωσης δεν θα επιτρέψουν να ανακαλέσετε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="11148-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="11148-115">Από την καρτέλα "μήνυμα", επιλέξτε **Ενέργειες** > **Ανάκληση του μηνύματος**.</span><span class="sxs-lookup"><span data-stu-id="11148-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="11148-116">Επιλέξτε **Διαγραφή μη αναγνωσμένων αντιγράφων του μηνύματος** "ή" **Διαγραφή μη αναγνωσμένων αντιγράφων και αντικατάστασή τους με νέο μήνυμα**και, στη συνέχεια, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="11148-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="11148-117">Εάν στέλνετε ένα μήνυμα αντικατάστασης, συντάξτε το μήνυμα και, στη συνέχεια, επιλέξτε **Αποστολή**.</span><span class="sxs-lookup"><span data-stu-id="11148-117">If you’re sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="11148-118">Η επιτυχία ή αποτυχία της ανάκληση μηνύματος εξαρτάται από τους παραλήπτες ρυθμίσεις στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="11148-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="11148-119">Για περισσότερες πληροφορίες, συμπεριλαμβανομένου του τρόπου ελέγχου ανάκλησης, ανατρέξτε στο θέμα [ανάκλησης ή αντικατάστασης ενός μηνύματος ηλεκτρονικού ταχυδρομείου που στείλατε](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="11148-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="11148-120">***Αναζήτηση και διαγραφή μηνυμάτων ηλεκτρονικού ταχυδρομείου στον οργανισμό σας*** Για να αναζητήσετε και να διαγράφετε μηνύματα ηλεκτρονικού ταχυδρομείου στην εταιρεία σας, είναι ευκολότερος Εάν είστε ένα καθολικό διαχειριστή. Εάν δεν είστε διαχειριστής της κύριας, ο λογαριασμός σας πρέπει να προστεθεί στην ομάδα ρόλου διαχείρισης ανακάλυψης ή ο ρόλος διαχείρισης αναζήτησης συμμόρφωσης.</span><span class="sxs-lookup"><span data-stu-id="11148-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="11148-121">Για να διαγράψετε μηνύματα, θα χρειαστεί να συμμετάσχετε στην ομάδα ρόλου διαχείρισης εταιρείας ή ο ρόλος διαχείρισης αναζήτησης και εκκαθάριση.</span><span class="sxs-lookup"><span data-stu-id="11148-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="11148-122">Αντιστοιχίζονται δικαιώματα για αυτούς τους ρόλους στο [Κέντρο συμμόρφωσης ασφαλείας &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="11148-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="11148-123">[Δημιουργία ενός περιεχομένου αναζήτησης](https://docs.microsoft.com/office365/securitycompliance/content-search) για να βρείτε το μήνυμα για να διαγράψετε.</span><span class="sxs-lookup"><span data-stu-id="11148-123">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="11148-124">[Συνδεθείτε με PowerShell συμμόρφωση παραγωγής & ασφαλείας](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="11148-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="11148-125">Εάν χρησιμοποιείτε ΣΠΙ, ανατρέξτε στο θέμα [σύνδεση σε & ασφαλείας για το Office 365 συμμόρφωση παραγωγής PowerShell χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="11148-125">If you're using MFA, see [Connect to Office 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
