---
title: Κολλήσει στα εξερχόμενα λόγω μεγάλων συνημμένων
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241252"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="aa0d4-102">Επιδιόρθωση μηνυμάτων που έχουν κολλήσει στα εξερχόμενα</span><span class="sxs-lookup"><span data-stu-id="aa0d4-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="aa0d4-103">Συνιστάται να ξεκινήσετε εκτελώντας το σενάριο ["Αντιμετωπίζετε προβλήματα κατά την αποστολή, λήψη ή εύρεση μηνυμάτων ηλεκτρονικού ταχυδρομείου"](https://aka.ms/SaRA-OutlookSendReceive) από το εργαλείο [υποστήριξης και αποκατάστασης της Microsoft.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="aa0d4-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="aa0d4-104">Όταν ένα μήνυμα κολλήσει στα Εξερχόμενα, η πιο πιθανή αιτία είναι ένα μεγάλο συνημμένο ή η επιλογή "Άμεση αποστολή όταν είναι συνδεδεμένο".</span><span class="sxs-lookup"><span data-stu-id="aa0d4-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="aa0d4-105">**Κατάργηση του μεγάλου συνημμένου**</span><span class="sxs-lookup"><span data-stu-id="aa0d4-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="aa0d4-106">Στο Outlook, επιλέξτε **Αποστολή / Λήψη** > **εργασίας χωρίς σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="aa0d4-107">Στο παράθυρο περιήγησης, επιλέξτε **Εξερχόμενα**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="aa0d4-108">Από εδώ, μπορείτε να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="aa0d4-108">From here, you can:</span></span> 
    - <span data-ttu-id="aa0d4-109">Διαγράψτε το μήνυμα (επιλέξτε το και, στη συνέχεια, **επιλέξτε Διαγραφή**).</span><span class="sxs-lookup"><span data-stu-id="aa0d4-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="aa0d4-110">Σύρετε το μήνυμα στο φάκελο "Πρόχειρα", κάντε διπλό κλικ για να το ανοίξετε και καταργήστε το συνημμένο επιλέξτε το και, στη συνέχεια, επιλέξτε **Διαγραφή**).</span><span class="sxs-lookup"><span data-stu-id="aa0d4-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="aa0d4-111">Εάν λάβετε ένα σφάλμα που αναφέρει ότι το Outlook προσπαθεί να μεταδώσει το μήνυμα, κλείστε το Outlook.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="aa0d4-112">Μπορεί να πάρει μερικά λεπτά για να βγείτε.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-112">It may take a few moments to exit.</span></span> <span data-ttu-id="aa0d4-113">Εάν το Outlook δεν κλείσει, πατήστε το συνδυασμό πλήκτρων Ctrl+Alt+Delete και επιλέξτε **Έναρξη Διαχείρισης Εργασιών**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="aa0d4-114">Στη Διαχείριση Εργασιών, επιλέξτε την καρτέλα **Διεργασίες,** κάντε κύλιση προς τα κάτω στο outlook.exe και επιλέξτε **Τερματισμός διεργασίας**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="aa0d4-115">Αφού κλείσει το Outlook, επανεκκινήστε το και επαναλάβετε τα βήματα 2 και 3.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="aa0d4-116">Αφού καταργήσετε το συνημμένο, κάντε κλικ στην επιλογή **Αποστολή / Λήψη** > **εργασίας χωρίς σύνδεση** για να συνεχίσετε να εργάζεστε online.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="aa0d4-117">Τα μηνύματα κολλάνε επίσης στα εξερχόμενα όταν κάνετε κλικ στην επιλογή **Αποστολή**, αλλά δεν είστε συνδεδεμένοι.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="aa0d4-118">Κάντε κλικ στην **επιλογή Αποστολή / Παραλαβή** και κοιτάξτε το κουμπί Εργασία χωρίς **σύνδεση.**</span><span class="sxs-lookup"><span data-stu-id="aa0d4-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="aa0d4-119">Αν είναι μπλε, είσαι αποσυνδεδεμένος.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="aa0d4-120">Κάντε κλικ σε αυτό για να συνδεθείτε (το κουμπί γίνεται λευκό) και κάντε κλικ στην επιλογή **Αποστολή όλων**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="aa0d4-121">**Ενεργοποίηση άμεσης αποστολής όταν είστε συνδεδεμένοι**</span><span class="sxs-lookup"><span data-stu-id="aa0d4-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="aa0d4-122">Στην καρτέλα Αρχείο, κάντε κλικ στην επιλογή **Επιλογές**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="aa0d4-123">Στο παράθυρο διαλόγου Επιλογές του Outlook, κάντε κλικ στην επιλογή **Για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="aa0d4-124">Στην ενότητα Αποστολή και λήψη, κάντε κλικ για να **ενεργοποιήσετε την επιλογή Αποστολή αμέσως όταν είστε συνδεδεμένοι**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="aa0d4-125">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa0d4-125">Click **OK**.</span></span>
 
<span data-ttu-id="aa0d4-126">Για περισσότερες λεπτομέρειες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="aa0d4-126">For full details, see:</span></span>
- [<span data-ttu-id="aa0d4-127">Βίντεο: Αποστολή ή διαγραφή μηνύματος ηλεκτρονικού ταχυδρομείου που έχει κολλήσει</span><span class="sxs-lookup"><span data-stu-id="aa0d4-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="aa0d4-128">Το μήνυμα ηλεκτρονικού ταχυδρομείου παραμένει στο φάκελο "Εξερχόμενα" μέχρι να ξεκινήσετε με μη αυτόματο τρόπο μια λειτουργία αποστολής/παραλαβής στο Outlook</span><span class="sxs-lookup"><span data-stu-id="aa0d4-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
