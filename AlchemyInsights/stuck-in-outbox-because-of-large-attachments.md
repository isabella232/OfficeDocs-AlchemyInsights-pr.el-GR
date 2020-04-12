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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232630"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="60420-102">Επιδιόρθωση μηνυμάτων που έχουν κολλήσει στα εξερχόμενα</span><span class="sxs-lookup"><span data-stu-id="60420-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="60420-103">Συνιστάται να ξεκινήσετε εκτελώντας το σενάριο ["Αντιμετωπίζετε προβλήματα κατά την αποστολή, λήψη ή εύρεση μηνυμάτων ηλεκτρονικού ταχυδρομείου"](https://aka.ms/SaRA-OutlookSendReceive) από το εργαλείο [υποστήριξης και αποκατάστασης της Microsoft](https://diagnostics.office.com/#/) στον υπολογιστή που επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="60420-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="60420-104">Όταν ένα μήνυμα κολλήσει στα Εξερχόμενα, η πιο πιθανή αιτία είναι ένα μεγάλο συνημμένο ή η επιλογή "Άμεση αποστολή όταν είναι συνδεδεμένο".</span><span class="sxs-lookup"><span data-stu-id="60420-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="60420-105">**Κατάργηση του μεγάλου συνημμένου**</span><span class="sxs-lookup"><span data-stu-id="60420-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="60420-106">Κάντε κλικ στην επιλογή **Αποστολή / Λήψη** > **εργασίας χωρίς σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="60420-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="60420-107">Στο παράθυρο περιήγησης, κάντε κλικ στην επιλογή **Εξερχόμενα**.</span><span class="sxs-lookup"><span data-stu-id="60420-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="60420-108">Από εδώ, μπορείτε να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="60420-108">From here, you can:</span></span> 
    - <span data-ttu-id="60420-109">Διαγράψτε το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="60420-109">Delete the message.</span></span> <span data-ttu-id="60420-110">Απλά επιλέξτε το και κάντε κλικ στο **κουμπί Διαγραφή**.</span><span class="sxs-lookup"><span data-stu-id="60420-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="60420-111">Σύρετε το μήνυμα στο **φάκελο "Πρόχειρα",** κάντε διπλό κλικ για να ανοίξετε το μήνυμα και διαγράψτε το συνημμένο (κάντε κλικ σε αυτό και κάντε κλικ στην επιλογή **Διαγραφή**).</span><span class="sxs-lookup"><span data-stu-id="60420-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="60420-112">Εάν ένα σφάλμα σας ενημερώνει ότι το Outlook προσπαθεί να μεταδώσει το μήνυμα, κλείστε το Outlook.</span><span class="sxs-lookup"><span data-stu-id="60420-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="60420-113">Μπορεί να πάρει μερικά λεπτά για να βγείτε.</span><span class="sxs-lookup"><span data-stu-id="60420-113">It may take a few moments to exit.</span></span> <span data-ttu-id="60420-114">Εάν το Outlook δεν κλείσει, **πατήστε το συνδυασμό πλήκτρων Ctrl+Alt+Delete** και κάντε κλικ στην επιλογή **Έναρξη Διαχείρισης Εργασιών**.</span><span class="sxs-lookup"><span data-stu-id="60420-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="60420-115">Στη Διαχείριση Εργασιών, επιλέξτε την καρτέλα **Διεργασίες,** κάντε κύλιση προς τα κάτω στο outlook.exe και κάντε κλικ στο **κουμπί Τερματισμός διεργασίας**.</span><span class="sxs-lookup"><span data-stu-id="60420-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="60420-116">Μετά το κλείσιμο του Outlook, επανεκκινήστε το Outlook και επαναλάβετε τα βήματα 2-3.</span><span class="sxs-lookup"><span data-stu-id="60420-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="60420-117">Αφού καταργήσετε το συνημμένο, κάντε κλικ στην επιλογή **Αποστολή / Λήψη** > **εργασίας χωρίς σύνδεση** για να καταργήσετε την επιλογή του κουμπιού και να συνεχίσετε να εργάζεστε online.</span><span class="sxs-lookup"><span data-stu-id="60420-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="60420-118">Τα μηνύματα κολλάνε επίσης στα εξερχόμενα όταν κάνετε κλικ στην επιλογή **Αποστολή**, αλλά δεν είστε συνδεδεμένοι.</span><span class="sxs-lookup"><span data-stu-id="60420-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="60420-119">Κάντε κλικ στην **επιλογή Αποστολή / Παραλαβή** και κοιτάξτε το κουμπί Εργασία χωρίς **σύνδεση.**</span><span class="sxs-lookup"><span data-stu-id="60420-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="60420-120">Αν είναι μπλε, είσαι αποσυνδεδεμένος.</span><span class="sxs-lookup"><span data-stu-id="60420-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="60420-121">Κάντε κλικ σε αυτό για να συνδεθείτε (το κουμπί γίνεται λευκό) και κάντε κλικ στην επιλογή **Αποστολή όλων**.</span><span class="sxs-lookup"><span data-stu-id="60420-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="60420-122">**Ενεργοποίηση άμεσης αποστολής όταν είστε συνδεδεμένοι**</span><span class="sxs-lookup"><span data-stu-id="60420-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="60420-123">Στην καρτέλα Αρχείο, κάντε κλικ στην επιλογή **Επιλογές**.</span><span class="sxs-lookup"><span data-stu-id="60420-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="60420-124">Στο παράθυρο διαλόγου Επιλογές του Outlook, κάντε κλικ στην επιλογή **Για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="60420-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="60420-125">Στην ενότητα Αποστολή και λήψη, κάντε κλικ για να **ενεργοποιήσετε την επιλογή Αποστολή αμέσως όταν είστε συνδεδεμένοι**.</span><span class="sxs-lookup"><span data-stu-id="60420-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="60420-126">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="60420-126">Click **OK**.</span></span>
 
<span data-ttu-id="60420-127">Για περισσότερες λεπτομέρειες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="60420-127">For full details, see:</span></span>
- [<span data-ttu-id="60420-128">Βίντεο: Αποστολή ή διαγραφή μηνύματος ηλεκτρονικού ταχυδρομείου που έχει κολλήσει</span><span class="sxs-lookup"><span data-stu-id="60420-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="60420-129">Το μήνυμα ηλεκτρονικού ταχυδρομείου παραμένει στο φάκελο "Εξερχόμενα" μέχρι να ξεκινήσετε με μη αυτόματο τρόπο μια λειτουργία αποστολής/παραλαβής στο Outlook</span><span class="sxs-lookup"><span data-stu-id="60420-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
