---
title: Κολλημένος στα εξερχόμενα εξαιτίας μεγάλων συνημμένων
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441306"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="4d6ab-102">Επιδιόρθωση μηνυμάτων που έχουν κολλήσει στο φάκελο "Εξερχόμενα"</span><span class="sxs-lookup"><span data-stu-id="4d6ab-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="4d6ab-103">Συνιστούμε να ξεκινήσετε εκτελώντας το σενάριο ["έχω προβλήματα με την αποστολή, τη λήψη ή την εύρεση μηνυμάτων ηλεκτρονικού ταχυδρομείου"](https://aka.ms/SaRA-OutlookSendReceive) από το εργαλείο [υποστήριξης της Microsoft και του βοηθού αποκατάστασης](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="4d6ab-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="4d6ab-104">Όταν ένα μήνυμα κολλάει στο φάκελο "Εξερχόμενα", οι πιο πιθανές αιτίες είναι οι εξής:</span><span class="sxs-lookup"><span data-stu-id="4d6ab-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="4d6ab-105">Μεγάλα συνημμένα.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-105">Large attachments.</span></span>
- <span data-ttu-id="4d6ab-106">Η επιλογή **Αποστολή αμέσως όταν είναι συνδεδεμένη** δεν είναι ενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="4d6ab-107">Για να καταργήσετε μεγάλα συνημμένα:</span><span class="sxs-lookup"><span data-stu-id="4d6ab-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="4d6ab-108">Στο Outlook, επιλέξτε **Αποστολή/παραλαβή** > **εργασίας χωρίς σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="4d6ab-109">Στο παράθυρο περιήγησης, επιλέξτε **Εξερχόμενα**.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="4d6ab-110">Από εδώ, μπορείτε να:</span><span class="sxs-lookup"><span data-stu-id="4d6ab-110">From here, you can:</span></span> 
    - <span data-ttu-id="4d6ab-111">Διαγράψτε το μήνυμα (επιλέξτε το και, στη συνέχεια, επιλέξτε **Διαγραφή**).</span><span class="sxs-lookup"><span data-stu-id="4d6ab-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="4d6ab-112">Σύρετε το μήνυμα στο φάκελο "Πρόχειρα", κάντε διπλό κλικ για να το ανοίξετε και καταργήστε το συνημμένο, επιλέξτε το και, στη συνέχεια, επιλέξτε **Διαγραφή**).</span><span class="sxs-lookup"><span data-stu-id="4d6ab-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="4d6ab-113">Εάν εμφανιστεί ένα σφάλμα που λέει ότι το Outlook προσπαθεί να μεταδώσει το μήνυμα, κλείστε το Outlook.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="4d6ab-114">Μπορεί να χρειαστούν λίγα λεπτά για να βγείτε.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-114">It may take a few moments to exit.</span></span> <span data-ttu-id="4d6ab-115">Εάν το Outlook δεν κλείσει, πιέστε το συνδυασμό πλήκτρων CTRL + ALT + DELETE και επιλέξτε **Έναρξη διαχείρισης εργασιών**.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="4d6ab-116">Στη διαχείριση εργασιών, επιλέξτε την καρτέλα **διεργασίες** , μετακινηθείτε προς τα κάτω στο Outlook. exe και επιλέξτε **Τέλος διεργασίας**.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="4d6ab-117">Μετά το κλείσιμο του Outlook, επανεκκινήστε το και επαναλάβετε τα βήματα 2 και 3.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="4d6ab-118">Αφού καταργήσετε το συνημμένο, κάντε κλικ στην επιλογή **Αποστολή/παραλαβή** > **εργασίας χωρίς σύνδεση** για να συνεχίσετε την εργασία σε σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="4d6ab-119">Τα μηνύματα έχουν επίσης κολλήσει στο φάκελο "Εξερχόμενα" όταν κάνετε κλικ στο κουμπί " **Αποστολή**", αλλά δεν είστε συνδεδεμένοι.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="4d6ab-120">Κάντε κλικ στην επιλογή **Αποστολή/παραλαβή** και δείτε το κουμπί **εργασίας χωρίς σύνδεση** .</span><span class="sxs-lookup"><span data-stu-id="4d6ab-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="4d6ab-121">Αν είναι μπλε, είσαι αποσυνδεδεμένος.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="4d6ab-122">Επιλέξτε το για να συνδεθείτε (το κουμπί γίνεται λευκό) και κάντε κλικ στο κουμπί **Αποστολή όλων**.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="4d6ab-123">Για να ενεργοποιήσετε την **Αποστολή αμέσως όταν συνδέεστε**:</span><span class="sxs-lookup"><span data-stu-id="4d6ab-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="4d6ab-124">Επιλέξτε \*\*\*\* > \*\*\*\* επιλογές >  αρχείου**για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="4d6ab-125">Στην ενότητα **Αποστολή και παραλαβή** , επιλέξτε **Αποστολή αμέσως όταν είστε συνδεδεμένοι**και, στη συνέχεια, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="4d6ab-126">Για πλήρεις λεπτομέρειες βλέπε:</span><span class="sxs-lookup"><span data-stu-id="4d6ab-126">For full details see:</span></span>
- [<span data-ttu-id="4d6ab-127">Βίντεο: αποστολή ή διαγραφή ενός κολλήτου ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="4d6ab-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="4d6ab-128">Το μήνυμα ηλεκτρονικού ταχυδρομείου παραμένει στο φάκελο "Εξερχόμενα" μέχρι να ξεκινήσετε με μη αυτόματο τρόπο μια λειτουργία αποστολής/παραλαβής στο Outlook</span><span class="sxs-lookup"><span data-stu-id="4d6ab-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
