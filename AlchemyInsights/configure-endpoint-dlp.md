---
title: Ρύθμιση παραμέτρων DLP τελικών σημείων
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402423"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="4ea88-102">Ρύθμιση παραμέτρων DLP τελικών σημείων</span><span class="sxs-lookup"><span data-stu-id="4ea88-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="4ea88-103">Τα DLP τελικών σημείων της Microsoft σάς επιτρέπουν να επεκτείνετε τη δυνατότητα προστασίας και παρακολούθησης DLP στις ευαίσθητες πληροφορίες σε συσκευές Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4ea88-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="4ea88-104">Αφού οι συσκευές εγγραφούν στη διαχείριση συσκευών, μπορείτε να δημιουργήσετε πολιτικές DLP για την επιβολή ασφαλιστικών ενεργειών σε στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="4ea88-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="4ea88-105">Η "Εξερεύνηση δραστηριότητας" μπορεί να χρησιμοποιηθεί για την παρακολούθηση της δραστηριότητας για ευαίσθητα στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="4ea88-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="4ea88-106">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών στη διαχείριση συσκευών](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="4ea88-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="4ea88-107">Για να ξεκινήσετε με τα DLP τελικών σημείων:</span><span class="sxs-lookup"><span data-stu-id="4ea88-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="4ea88-108">Βεβαιωθείτε ότι έχετε τις κατάλληλες άδειες χρήσης για το SKU/συνδρομές.</span><span class="sxs-lookup"><span data-stu-id="4ea88-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="4ea88-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [άδειες χρήσης SKU/συνδρομές](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="4ea88-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="4ea88-110">Ελέγξτε τα δικαιώματα που απαιτούνται για να ενεργοποιήσετε τη διαχείριση συσκευών, να αποκτήσετε πρόσβαση στη σελίδα εγγραφής ή να ενεργοποιήσετε/απενεργοποιήσετε την παρακολούθηση συσκευών.</span><span class="sxs-lookup"><span data-stu-id="4ea88-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="4ea88-111">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δικαιώματα](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="4ea88-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="4ea88-112">Εγγράψτε συσκευές στη Διαχείριση συσκευών, ακολουθώντας τη διαδικασία εγγραφής συσκευών.</span><span class="sxs-lookup"><span data-stu-id="4ea88-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="4ea88-113">Εάν δεν έχετε την επιλογή "Εγγραφή συσκευών" (προεπισκόπηση) στην περιοχή **Ρυθμίσεις** συμμόρφωσης M365, βεβαιωθείτε ότι έχετε την κατάλληλη άδεια χρήσης και τα δικαιώματα που αναφέρονται παραπάνω.</span><span class="sxs-lookup"><span data-stu-id="4ea88-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="4ea88-114">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="4ea88-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="4ea88-115">Δημιουργήστε πολιτικές DLP για την προστασία των ευαίσθητων στοιχείων σας.</span><span class="sxs-lookup"><span data-stu-id="4ea88-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="4ea88-116">Για πληροφορίες, ανατρέξτε στο θέμα [Σενάρια πολιτικής DLP τελικών σημείων](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="4ea88-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="4ea88-117">Για περισσότερες πληροφορίες σχετικά με τα DLP τελικών σημείων της Microsoft, ανατρέξτε στο θέμα [Μάθετε περισσότερα σχετικά με την αποτροπή απώλειας δεδομένων τελικών σημείων του Microsoft 365 (προεπισκόπηση)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="4ea88-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="4ea88-118">**Σημαντικά βήματα συλλογής δεδομένων, εάν απαιτείται υποστήριξη:**</span><span class="sxs-lookup"><span data-stu-id="4ea88-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="4ea88-119">Κατέβασμα της Προεπισκόπησης ανάλυσης προγράμματος-πελάτη MDATP από το [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="4ea88-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="4ea88-120">Εκτελέστε το εργαλείο ως διαχειριστής από το παράθυρο cmd:</span><span class="sxs-lookup"><span data-stu-id="4ea88-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="4ea88-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="4ea88-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="4ea88-122">Όταν σας ζητηθεί η ερώτηση "Εισαγάγετε τον αριθμό των λεπτών για τη συλλογή ανιχνεύσεων:", εισαγάγετε τον αριθμό των λεπτών που απαιτούνται για την εκτέλεση του σεναρίου</span><span class="sxs-lookup"><span data-stu-id="4ea88-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="4ea88-123">Εκτέλεση του σεναρίου</span><span class="sxs-lookup"><span data-stu-id="4ea88-123">Run the scenario</span></span>

<span data-ttu-id="4ea88-124">Συλλέξτε την έξοδο του αρχείου zip που θα δοθεί στον συνεργάτη υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="4ea88-124">Collect the Zip file output to be given to the Support agent.</span></span>
