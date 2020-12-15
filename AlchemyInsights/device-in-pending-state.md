---
title: Συσκευή σε κατάσταση εκκρεμούς
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678479"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="a91c0-102">Συσκευή σε κατάσταση εκκρεμούς</span><span class="sxs-lookup"><span data-stu-id="a91c0-102">Device in pending state</span></span>

<span data-ttu-id="a91c0-103">**Τις προϋποθέσεις**</span><span class="sxs-lookup"><span data-stu-id="a91c0-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="a91c0-104">Εάν ρυθμίζετε εγγραφές συσκευών για πρώτη φορά, βεβαιωθείτε ότι έχετε αναθεωρηθεί [Εισαγωγή στη διαχείριση συσκευών στο Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) που θα σας καθοδηγήσει στον τρόπο με τον οποίο μπορείτε να λάβετε συσκευές υπό τον έλεγχο του Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a91c0-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="a91c0-105">Εάν καταχωρείτε συσκευές στο Azure AD απευθείας και τις εγγράφετε σε Intune, θα πρέπει να εξασφαλίσετε ότι έχετε ρυθμίσει τις [παραμέτρους του Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) και ότι θα έχετε την [άδεια χρήσης](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) στη θέση της πρώτα.</span><span class="sxs-lookup"><span data-stu-id="a91c0-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="a91c0-106">Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Azure AD και τη διαφήμιση εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="a91c0-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="a91c0-107">Μόνο ένας καθολικός διαχειριστής στο Azure AD μπορεί να διαχειριστεί ρυθμίσεις για τις καταχωρήσεις συσκευών.</span><span class="sxs-lookup"><span data-stu-id="a91c0-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="a91c0-108">Επιπλέον, εάν ρυθμίζετε αυτόματες εγγραφές στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, θα πρέπει να είστε διαχειριστής της υπηρεσίας καταλόγου Active Directory και του AD FS (εάν υπάρχει).</span><span class="sxs-lookup"><span data-stu-id="a91c0-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="a91c0-109">Η διαδικασία δήλωσης σύνδεσης του υβριδικού Azure AD απαιτεί συσκευές για να είναι σε εταιρικό δίκτυο.</span><span class="sxs-lookup"><span data-stu-id="a91c0-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="a91c0-110">Λειτουργεί επίσης μέσω VPN, αλλά υπάρχουν ορισμένες προειδοποιήσεις για αυτό.</span><span class="sxs-lookup"><span data-stu-id="a91c0-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="a91c0-111">Ακούσαμε ότι οι πελάτες χρειάζονται βοήθεια για την αντιμετώπιση της διαδικασίας δήλωσης συμμετοχής στο υβριδικό Azure AD, στην περιοχή απομακρυσμένες συνθήκες εργασίας.</span><span class="sxs-lookup"><span data-stu-id="a91c0-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="a91c0-112">**Περιβάλλον ελέγχου ταυτότητας cloud (χρησιμοποιώντας τον συγχρονισμό κατακερματισμού κωδικού πρόσβασης AD Azure ή τον έλεγχο ταυτότητας διαβίβασης)**</span><span class="sxs-lookup"><span data-stu-id="a91c0-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="a91c0-113">Αυτή η ροή δήλωσης είναι επίσης γνωστή ως "Συγχρονισμός συνδέσμου".</span><span class="sxs-lookup"><span data-stu-id="a91c0-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="a91c0-114">Ακολουθεί μια ανάλυση για το τι συμβαίνει κατά τη διαδικασία εγγραφής:</span><span class="sxs-lookup"><span data-stu-id="a91c0-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="a91c0-115">Τα Windows 10 ανακαλύπτουν την εγγραφή του σημείο σύνδεσης υπηρεσίας (SCP) όταν ο χρήστης συνδέεται στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="a91c0-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="a91c0-116">Η συσκευή επιχειρεί πρώτα να ανακτήσει πληροφορίες μισθωτών από το SCP του προγράμματος-πελάτη στο μητρώο [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="a91c0-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="a91c0-117">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [έγγραφο](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="a91c0-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="a91c0-118">Εάν αποτύχει, η συσκευή επικοινωνεί με την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης για να λάβετε πληροφορίες μισθωτών από την SCP.</span><span class="sxs-lookup"><span data-stu-id="a91c0-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="a91c0-119">Για να επαληθεύσετε το SCP, ανατρέξτε σε αυτό το [έγγραφο](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="a91c0-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="a91c0-120">Συνιστούμε να ενεργοποιήσετε την SCP στην υπηρεσία καταλόγου Active Directory και να χρησιμοποιείτε μόνο το SCP προγράμματος-πελάτη για την αρχική επικύρωση.</span><span class="sxs-lookup"><span data-stu-id="a91c0-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="a91c0-121">Τα Windows 10 προσπαθούν να επικοινωνούν με το Azure AD κάτω από το περιβάλλον συστήματος για τον έλεγχο ταυτότητας από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a91c0-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="a91c0-122">Μπορείτε να επαληθεύσετε εάν η συσκευή μπορεί να αποκτήσει πρόσβαση σε πόρους της Microsoft κάτω από το λογαριασμό συστήματος, χρησιμοποιώντας τη [δέσμη ενεργειών συνδεσιμότητας δήλωσης δοκιμής συσκευής](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="a91c0-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="a91c0-123">Τα Windows 10 παράγουν αυτο-υπογεγραμμένο πιστοποιητικό και το αποθηκεύουν κάτω από το αντικείμενο υπολογιστή στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="a91c0-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="a91c0-124">Αυτό απαιτεί οπτική επαφή με τον ελεγκτή τομέα.</span><span class="sxs-lookup"><span data-stu-id="a91c0-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="a91c0-125">Αντικείμενο συσκευής που έχει το πιστοποιητικό συγχρονίζεται με το Azure AD μέσω σύνδεσης Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a91c0-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="a91c0-126">Ο κύκλος συγχρονισμού είναι κάθε 30 λεπτά από προεπιλογή, αλλά εξαρτάται από τη ρύθμιση παραμέτρων του Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a91c0-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="a91c0-127">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό το [έγγραφο](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="a91c0-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="a91c0-128">Σε αυτό το στάδιο, θα πρέπει να μπορείτε να δείτε τη συσκευή θέματος σε κατάσταση "σε **εκκρεμότητα**" στην περιοχή "λεπίδα συσκευής" του Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="a91c0-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="a91c0-129">Στην επόμενη σύνδεση χρήστη στα Windows 10, η καταχώρηση θα ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="a91c0-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a91c0-130">Εάν βρίσκεστε σε VPN και η αποσύνδεση/σύνδεση τερματίζει τη συνδεσιμότητα τομέα, μπορείτε να ενεργοποιήσετε την καταχώρηση με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="a91c0-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="a91c0-131">Για να το κάνετε αυτό:</span><span class="sxs-lookup"><span data-stu-id="a91c0-131">To do that:</span></span>
    >
    > <span data-ttu-id="a91c0-132">Εκδώσετε ένα `dsregcmd /join` τοπικό μήνυμα στο διαχειριστή ή απομακρυσμένα μέσω του PSExec στον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="a91c0-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="a91c0-133">Για παράδειγμα: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="a91c0-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="a91c0-134">Για συνηθισμένα προβλήματα με την καταχώρηση συσκευής του Azure Active Directory, ανατρέξτε στο θέμα [Συνήθεις ερωτήσεις](https://docs.microsoft.com/azure/active-directory/devices/faq)για τις συσκευές.</span><span class="sxs-lookup"><span data-stu-id="a91c0-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
