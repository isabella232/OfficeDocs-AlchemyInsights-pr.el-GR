---
title: Αντιμετώπιση προβλημάτων με το θέμα PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573496"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="42400-102">Αντιμετώπιση προβλημάτων με το θέμα PRT</span><span class="sxs-lookup"><span data-stu-id="42400-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="42400-103">Για να ολοκληρωθεί η επικύρωση οποιασδήποτε συσκευής, πρέπει να είναι πλήρως καταχωρημένη και να είναι σε καλή κατάσταση και να είναι σε θέση να αποκτήσει έναν κύριο κωδικό ανανέωσης (PRT).</span><span class="sxs-lookup"><span data-stu-id="42400-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="42400-104">Η διαδικασία εγγραφής του υβριδικού συνδέσμου Azure AD απαιτεί οι συσκευές να βρίσκονται σε εταιρικό δίκτυο.</span><span class="sxs-lookup"><span data-stu-id="42400-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="42400-105">Λειτουργεί επίσης μέσω VPN, αλλά υπάρχουν ορισμένες προειδοποιήσεις για αυτό.</span><span class="sxs-lookup"><span data-stu-id="42400-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="42400-106">Ακούσαμε ότι οι πελάτες χρειάζονται βοήθεια για την αντιμετώπιση της διαδικασίας εγγραφής του υβριδικού Azure AD Join σε συνθήκες απομακρυσμένων εργασιών.</span><span class="sxs-lookup"><span data-stu-id="42400-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="42400-107">Ακολουθεί μια ανάλυση των όσων συμβαίνουν "κάτω από το καπό" κατά τη διαδικασία εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="42400-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="42400-108">**Περιβάλλον ελέγχου ταυτότητας cloud (χρησιμοποιώντας τον συγχρονισμό κατακερματισμού κωδικού πρόσβασης AD Azure ή τον έλεγχο ταυτότητας διαβίβασης)**</span><span class="sxs-lookup"><span data-stu-id="42400-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="42400-109">Αυτή η ροή δήλωσης είναι επίσης γνωστή ως "Συγχρονισμός συνδέσμου".</span><span class="sxs-lookup"><span data-stu-id="42400-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="42400-110">Τα Windows 10 ανακαλύπτουν μια εγγραφή SCP κατά τη σύνδεση του χρήστη στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="42400-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="42400-111">Η συσκευή επιχειρεί πρώτα να ανακτήσει πληροφορίες μισθωτών από το SCP του προγράμματος-πελάτη στο μητρώο [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="42400-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="42400-112">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό το [έγγραφο](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="42400-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="42400-113">Εάν αποτύχει, η συσκευή επικοινωνεί με την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης (AD) για να λάβει πληροφορίες μισθωτών από το σημείο σύνδεσης υπηρεσίας (SCP).</span><span class="sxs-lookup"><span data-stu-id="42400-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="42400-114">Για να επαληθεύσετε το SCP, ανατρέξτε σε αυτό το [έγγραφο](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="42400-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="42400-115">Συνιστούμε να ενεργοποιήσετε την SCP στη διαφήμιση και να χρησιμοποιείτε μόνο το SCP προγράμματος-πελάτη για την αρχική επικύρωση.</span><span class="sxs-lookup"><span data-stu-id="42400-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="42400-116">Τα Windows 10 προσπαθούν να επικοινωνούν με το Azure AD κάτω από το περιβάλλον συστήματος για τον έλεγχο ταυτότητας από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="42400-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="42400-117">Μπορείτε να επαληθεύσετε εάν η συσκευή μπορεί να αποκτήσει πρόσβαση σε πόρους της Microsoft κάτω από το λογαριασμό συστήματος, χρησιμοποιώντας τη δέσμη ενεργειών συνδεσιμότητας δήλωσης δοκιμής συσκευής.</span><span class="sxs-lookup"><span data-stu-id="42400-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="42400-118">Τα Windows 10 δημιουργούν ένα πιστοποιητικό αυτόματης υπογραφής και το αποθηκεύουν κάτω από το αντικείμενο υπολογιστή στη διαφήμιση εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="42400-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="42400-119">Αυτό απαιτεί οπτική επαφή με τον ελεγκτή τομέα.</span><span class="sxs-lookup"><span data-stu-id="42400-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="42400-120">Ένα αντικείμενο συσκευής που έχει ένα πιστοποιητικό συγχρονίζεται με το Azure AD μέσω σύνδεσης Azure AD.</span><span class="sxs-lookup"><span data-stu-id="42400-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="42400-121">Ο κύκλος συγχρονισμού είναι κάθε 30 λεπτά από προεπιλογή, αλλά εξαρτάται από τη ρύθμιση παραμέτρων του Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="42400-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="42400-122">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό το [έγγραφο](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="42400-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="42400-123">Σε αυτό το στάδιο, θα πρέπει να μπορείτε να δείτε τη συσκευή θέματος σε κατάσταση "σε εκκρεμότητα" στην περιοχή "λεπίδα συσκευής" του Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="42400-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="42400-124">Στην επόμενη σύνδεση χρήστη στα Windows 10, η καταχώρηση θα ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="42400-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="42400-125">Εάν είστε σε VPN και μια διαδικασία σύνδεσης αποσύνδεσης τερματίζει τη συνδεσιμότητα τομέα, μπορείτε να ενεργοποιήσετε την καταχώρηση με μη αυτόματο τρόπο:</span><span class="sxs-lookup"><span data-stu-id="42400-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="42400-126">Εκδώσετε ένα dsregcmd/Join τοπικά στην προτροπή διαχειριστή ή απομακρυσμένα μέσω του PSExec στον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="42400-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="42400-127">Για παράδειγμα, PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="42400-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="42400-128">Για περισσότερες λεπτομέρειες σχετικά με τα υβριδικά θέματα συνδέσμου, ανατρέξτε στο [θέμα Αντιμετώπιση προβλημάτων συσκευών](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="42400-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
