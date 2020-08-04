---
title: Χρήση του TeamViewer για την απομακρυσμένη διαχείριση συσκευών Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554975"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="d785b-102">Χρήση του TeamViewer για την απομακρυσμένη διαχείριση συσκευών Intune</span><span class="sxs-lookup"><span data-stu-id="d785b-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="d785b-103">Οι συσκευές που διαχειρίζεται το Intune μπορούν να διαχειρίζονται απομακρυσμένα χρησιμοποιώντας [το TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="d785b-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="d785b-104">Για να διαχειριστείτε το Intune χρησιμοποιώντας το TeamViewer, χρησιμοποιήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="d785b-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="d785b-105">Ξεκινήστε αποκτώντας διαπιστευτήρια από το TeamViewer για να ρυθμίσετε τη σύνδεση TeamViewer στο Intune.</span><span class="sxs-lookup"><span data-stu-id="d785b-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="d785b-106">Αυτό επιτρέπει στο διαχειριστή να εισαγάγει διαπιστευτήρια στο περιβάλλον εργασίας χρήστη σύνδεσης TeamViewer στην περιοχή Συσκευές, μια λειτουργία μίας φοράς για τη δημιουργία της σύνδεσης μεταξύ Intune και της υπηρεσίας TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d785b-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="d785b-107">**Μέρος 1: Έναρξη περιόδου λειτουργίας με απομακρυσμένη συσκευή**</span><span class="sxs-lookup"><span data-stu-id="d785b-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="d785b-108">Στην περιοχή **Όλες οι συσκευές**, επιλέξτε τη συσκευή με την οποία θέλετε να ξεκινήσετε μια απομακρυσμένη περίοδο λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="d785b-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="d785b-109">Από **... Περισσότερα**, επιλέξτε **Νέα περίοδος λειτουργίας απομακρυσμένης βοήθειας**.</span><span class="sxs-lookup"><span data-stu-id="d785b-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="d785b-110">Επιλέξτε **Ναι** για να επιβεβαιώσετε ότι θέλετε να δημιουργήσετε μια απομακρυσμένη περίοδο λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="d785b-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="d785b-111">Αφού αναγνωριστεί η αίτηση "Έναρξη νέας απομακρυσμένης περιόδου λειτουργίας" από την υπηρεσία TeamViewer, θα δείτε μια επιλογή **εκκίνησης απομακρυσμένης βοήθειας** κάτω από τις λεπτομέρειες του παραθύρου Επισκόπηση (ή Essentials) για τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="d785b-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="d785b-112">Επιλέξτε **"Δείτε περισσότερα"** για να αναπτύξετε το παράθυρο και να εμφανίσετε την κατάσταση απομακρυσμένης βοήθειας.</span><span class="sxs-lookup"><span data-stu-id="d785b-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="d785b-113">Επιλέξτε **Έναρξη απομακρυσμένης περιόδου λειτουργίας** για να ξεκινήσετε την περίοδο λειτουργίας από την πλευρά του διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="d785b-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="d785b-114">Επιλέξτε να κάνετε λήψη του δυαδικού αρχείου TeamViewer (Windows) και επιλέξτε **Εκτέλεση**.</span><span class="sxs-lookup"><span data-stu-id="d785b-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="d785b-115">**Σημείωση** Μπορείτε να αγνοήσετε οποιαδήποτε σελίδα προγράμματος περιήγησης web που έχει ανοιχτεί στην τοποθεσία Web του TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d785b-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="d785b-116">Αναγνωρίστε την αίτηση για την εφαρμογή TeamViewer για να κάνετε αλλαγές στη συσκευή (μόνο για Windows).</span><span class="sxs-lookup"><span data-stu-id="d785b-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="d785b-117">Η εφαρμογή TeamViewer ξεκινά και περιλαμβάνει τον κωδικό περιόδου λειτουργίας για τον έλεγχο ταυτότητας της σύνδεσης με την απομακρυσμένη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="d785b-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="d785b-118">**Μέρος 2: Στη συσκευή που προορίζεται για απομακρυσμένη περίοδο λειτουργίας**</span><span class="sxs-lookup"><span data-stu-id="d785b-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="d785b-119">Ανοίξτε την πύλη της εταιρείας Intune.</span><span class="sxs-lookup"><span data-stu-id="d785b-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="d785b-120">Αναζητήστε μια σημαία ειδοποιήσεων: "Ο διαχειριστής it ζητά τον έλεγχο αυτής της συσκευής για μια περίοδο λειτουργίας απομακρυσμένης βοήθειας" και επιλέξτε την ειδοποίηση.</span><span class="sxs-lookup"><span data-stu-id="d785b-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="d785b-121">Επιλέξτε να κάνετε λήψη της εφαρμογής TeamViewer ή να αναγνωρίσετε τη λήψη της εφαρμογής TeamViewer από το app store και επιλέξτε **Εκτέλεση**.</span><span class="sxs-lookup"><span data-stu-id="d785b-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="d785b-122">**Σημείωση** Μπορείτε να αγνοήσετε οποιαδήποτε σελίδα προγράμματος περιήγησης web που έχει ανοιχτεί στην τοποθεσία Web του TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d785b-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="d785b-123">Αναγνωρίστε την αίτηση για την εφαρμογή TeamViewer για να κάνετε αλλαγές στη συσκευή (μόνο για Windows).</span><span class="sxs-lookup"><span data-stu-id="d785b-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="d785b-124">Η εφαρμογή TeamViewer ξεκινά και περιλαμβάνει τον κωδικό περιόδου λειτουργίας για τον έλεγχο ταυτότητας της σύνδεσης με την απομακρυσμένη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="d785b-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="d785b-125">Ένα αναδυόμενο παράθυρο ρωτά αν θέλετε να επιτρέψετε την έναρξη της περιόδου λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="d785b-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="d785b-126">**Σημείωση** Οι κωδικοί περιόδου λειτουργίας που δημιουργούνται από την υπηρεσία TeamViewer είναι μόνο μία φορά.</span><span class="sxs-lookup"><span data-stu-id="d785b-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="d785b-127">Εάν χάσετε τη σύνδεση, πρέπει:</span><span class="sxs-lookup"><span data-stu-id="d785b-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="d785b-128">Κλείστε την παρουσία της εφαρμογής TeamViewer στην απομακρυσμένη συσκευή και στο σταθμό εργασίας διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="d785b-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="d785b-129">Κλείστε την εταιρική πύλη στην απομακρυσμένη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="d785b-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="d785b-130">Ξεκινήστε μια νέα "Νέα περίοδο λειτουργίας απομακρυσμένης Βοήθειας" από την πύλη διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="d785b-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="d785b-131">Ανοίξτε εκ νέου την εταιρική πύλη στην απομακρυσμένη συσκευή για να λάβετε τη νέα ειδοποίηση.</span><span class="sxs-lookup"><span data-stu-id="d785b-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="d785b-132">Κάντε λήψη και ανοίξτε την εφαρμογή TeamViewer τόσο στην απομακρυσμένη συσκευή όσο και στο σταθμό εργασίας διαχειριστή, όπως και πριν.</span><span class="sxs-lookup"><span data-stu-id="d785b-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>