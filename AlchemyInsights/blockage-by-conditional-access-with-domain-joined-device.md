---
title: Έχω αποκλειστεί από την Πρόσβαση υπό όρους με μια συσκευή που είναι συνδεδεμένος με τομέα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036697"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="8655e-102">Έχω αποκλειστεί από την Πρόσβαση υπό όρους με μια συσκευή που είναι συνδεδεμένος με τομέα</span><span class="sxs-lookup"><span data-stu-id="8655e-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="8655e-103">**Εργαλεία που συνιστώνται ιδιαίτερα**</span><span class="sxs-lookup"><span data-stu-id="8655e-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="8655e-104">[Εργαλείο αντιμετώπισης προβλημάτων εγγραφής συσκευής](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - Το εργαλείο που σας βοηθά να αντιμετωπίσετε τα πιο συνηθισμένα προβλήματα εγγραφής συσκευής.</span><span class="sxs-lookup"><span data-stu-id="8655e-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="8655e-105">[Δοκιμή δέσμης ενεργειών συνδεσιμότητας εγγραφής συσκευής](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - Η δέσμη ενεργειών που σας βοηθά να εξασφαλίζετε ότι μια συσκευή μπορεί να αποκτήσει πρόσβαση στα τελικά σημεία καταχώρησης συσκευής κάτω από το λογαριασμό συστήματος.</span><span class="sxs-lookup"><span data-stu-id="8655e-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="8655e-106">[Δέσμη ενεργειών εκκαθάρισης συσκευής Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - Η δέσμη ενεργειών που σας επιτρέπει να αναζητήσετε και να διαχειριστείτε μη ορθές συσκευές στο περιβάλλον σας.</span><span class="sxs-lookup"><span data-stu-id="8655e-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="8655e-107">Ακολουθούν ορισμένοι συνηθισμένοι λόγοι για τους οποίους η πρόσβαση υπό όρους ενδέχεται να αποτυγχάνει σε μια συσκευή που έχει ενταχθεί σε έναν τομέα (Υβριδικό Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8655e-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="8655e-108">**Δεν υπάρχει Azure AD PRT** στη συσκευή - Πρέπει να βεβαιωθείτε ότι η συσκευή διαθέτει Διακριτικό κύριας ανανέωσης Azure AD (PRT).</span><span class="sxs-lookup"><span data-stu-id="8655e-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="8655e-109">Για περισσότερες πληροφορίες σχετικά με την PRT, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="8655e-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="8655e-110">Για να επαληθεύσετε εάν έχετε Azure AD PRT, μπορείτε να εκτελέσετε την εντολή στη συσκευή και να επαληθεύσετε εάν `dsregcmd/status` το "AzureAdPrt" ισούται με "ΝΑΙ".</span><span class="sxs-lookup"><span data-stu-id="8655e-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="8655e-111">Εάν το "AzureAdPrt" είναι "NO", ελέγξτε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="8655e-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="8655e-112">Εάν έχετε ένα ομόσπονδο περιβάλλον με **AD FS και** δεν είναι προσβάσιμο από τα οικιακά δίκτυα των χρηστών σας: Σε αυτή την περίπτωση, βεβαιωθείτε ότι τα τελικά σημεία "usernamemixed" είναι προσβάσιμα από το extranet.</span><span class="sxs-lookup"><span data-stu-id="8655e-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="8655e-113">Εάν το AD FS βρίσκεται πίσω από ένα VPN, βεβαιωθείτε ότι οι χρήστες συνδέονται στο VPN και επανα-συνδέονται στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="8655e-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="8655e-114">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="8655e-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="8655e-115">**Εάν το TPM** της συσκευής είναι ελαττωματικό και, επομένως, δεν είναι δυνατός ο έλεγχος ταυτότητας της συσκευής: Ελέγξτε "tpm.msc" για να δείτε εάν η κατάσταση της TPM είναι "Ready".</span><span class="sxs-lookup"><span data-stu-id="8655e-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="8655e-116">Εάν όχι, `dsregcmd/leave` εκτελέστε και αφήστε τη συσκευή να επανα-συμμετάσχει στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8655e-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="8655e-117">Στη συνέχεια, δοκιμάστε ξανά.</span><span class="sxs-lookup"><span data-stu-id="8655e-117">Then, try again.</span></span> <span data-ttu-id="8655e-118">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="8655e-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="8655e-119">**Χρησιμοποιείτε μια υπηρεσία παροχής ταυτότητας τρίτου κατασκευαστή, η οποία δεν υποστηρίζει WS-Trust πρωτοκόλλου.**</span><span class="sxs-lookup"><span data-stu-id="8655e-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="8655e-120">Όπως περιγράφεται στα έγγραφά μας, οι υβριδικές συσκευές που είναι συνδεδεμένες με το Azure AD δεν μπορούν να λειτουργούν σε αυτή την περίπτωση.</span><span class="sxs-lookup"><span data-stu-id="8655e-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="8655e-121">Συνεργαστείτε με την υπηρεσία παροχής ταυτότητας για υποστήριξη.</span><span class="sxs-lookup"><span data-stu-id="8655e-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="8655e-122">Οι χρήστες χρησιμοποιούν το πρόγραμμα περιήγησης Chrome χωρίς τους λογαριασμούς **Των Windows 10** ή την επέκταση του Office Το Chrome δεν χρησιμοποιεί αυτόματα το PRT σε συσκευές που είναι συνδεδεμένες με AAD ή σε συσκευές που είναι συνδεδεμένες με **υβριδική AAD:** Αυτό οδηγεί σε αποτυχία των πολιτικών πρόσβασης υπό όρους που βασίζονται σε συσκευή, με το μήνυμα σφάλματος "Μη καταχωρημένη συσκευή" να εμφανίζεται.</span><span class="sxs-lookup"><span data-stu-id="8655e-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="8655e-123">Για να χρησιμοποιήσετε σωστά το πρόγραμμα περιήγησης Chrome, πρέπει να εγκαταστήσετε τους "Λογαριασμούς Windows 10" ή "Επέκταση του Office στο πρόγραμμα περιήγησης Chrome των χρηστών" μέσω SCCM ή Intune.</span><span class="sxs-lookup"><span data-stu-id="8655e-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="8655e-124">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="8655e-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="8655e-125">Εάν δεν είναι δυνατή η απομακρυσμένη ώθηση της επέκτασης, ειδοποιήστε τους χρήστες να εγκαταστήσουν με μη αυτόματο τρόπο μία από τις παραπάνω επεκτάσεις για να αποκτήσουν πρόσβαση σε εφαρμογές πίσω από την πρόσβαση υπό όρους που βασίζεται σε συσκευή.</span><span class="sxs-lookup"><span data-stu-id="8655e-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="8655e-126">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="8655e-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="8655e-127">Η συσκευή συνδέθηκε σωστά με υβριδικό **Azure AD,** αλλά διαγράφηκε ή απενεργοποιήθηκε κατά λάθος, είτε λόγω αλλαγών συγχρονισμού στο Azure AD Connect είτε από την πύλη Azure: Εάν συμβεί αυτό, το αντικείμενο συσκευής δεν αναγνωρίζεται πλέον ως πλήρως συνδεδεμένο συσκευή, παρόλο που η κατάσταση "AzureAdJoined" και "PRT" εμφανίζεται ως έγκυρη στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="8655e-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="8655e-128">Για να διορθώσετε αυτό το πρόβλημα, `dsregcmd/leave` εκτελέστε τις συσκευές που επηρεάζονται και επιτρέψτε τους να επανασυνδετούν στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8655e-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="8655e-129">Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="8655e-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="8655e-130">Εάν οι συσκευές σας βρίσκονται σε ενημέρωση των Windows 10, 1809, με διακομιστή μεσολάβησης VPN/cloud και δείτε προβλήματα με την κατάσταση "AzureAdPrt" ή οποιαδήποτε εφαρμογή με πρόβλημα SSO (το Outlook δεν συνδέεται στο γραμματοκιβώτιο παρόλο που είχατε PRT), βεβαιωθείτε ότι έχετε αυτή την ενημέρωση [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ή την αθροιστική ενημέρωση [Απριλίου KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) για να αποτρέψετε αποτυχίες PRT σε αυτούς τους υπολογιστές.</span><span class="sxs-lookup"><span data-stu-id="8655e-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















