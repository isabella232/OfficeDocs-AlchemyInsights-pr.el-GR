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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657929"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="183e3-102">Ρύθμιση παραμέτρων DLP τελικών σημείων</span><span class="sxs-lookup"><span data-stu-id="183e3-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="183e3-103">Τα DLP τελικών σημείων της Microsoft σάς επιτρέπουν να επεκτείνετε τη δυνατότητα προστασίας και παρακολούθησης DLP στις ευαίσθητες πληροφορίες σε συσκευές Windows 10.</span><span class="sxs-lookup"><span data-stu-id="183e3-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="183e3-104">Αφού οι συσκευές εγγραφούν στη διαχείριση συσκευών, μπορείτε να δημιουργήσετε πολιτικές DLP για την επιβολή ασφαλιστικών ενεργειών σε στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="183e3-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="183e3-105">Η "Εξερεύνηση δραστηριότητας" μπορεί να χρησιμοποιηθεί για την παρακολούθηση της δραστηριότητας για ευαίσθητα στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="183e3-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="183e3-106">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών στη διαχείριση συσκευών](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="183e3-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="183e3-107">Για να ξεκινήσετε με τα DLP τελικών σημείων:</span><span class="sxs-lookup"><span data-stu-id="183e3-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="183e3-108">Βεβαιωθείτε ότι έχετε τις κατάλληλες άδειες χρήσης για το SKU/συνδρομές.</span><span class="sxs-lookup"><span data-stu-id="183e3-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="183e3-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [άδειες χρήσης SKU/συνδρομές](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="183e3-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="183e3-110">Ελέγξτε τα δικαιώματα που απαιτούνται για να ενεργοποιήσετε τη διαχείριση συσκευών, να αποκτήσετε πρόσβαση στη σελίδα εγγραφής ή να ενεργοποιήσετε/απενεργοποιήσετε την παρακολούθηση συσκευών.</span><span class="sxs-lookup"><span data-stu-id="183e3-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="183e3-111">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δικαιώματα](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="183e3-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="183e3-112">Εγγράψτε συσκευές στη Διαχείριση συσκευών, ακολουθώντας τη διαδικασία εγγραφής συσκευών.</span><span class="sxs-lookup"><span data-stu-id="183e3-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="183e3-113">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="183e3-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="183e3-114">Δημιουργήστε πολιτικές DLP για την προστασία των ευαίσθητων στοιχείων σας.</span><span class="sxs-lookup"><span data-stu-id="183e3-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="183e3-115">Για πληροφορίες, ανατρέξτε στο θέμα [Σενάρια πολιτικής DLP τελικών σημείων](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="183e3-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="183e3-116">Για περισσότερες πληροφορίες σχετικά με τα DLP τελικών σημείων της Microsoft, ανατρέξτε στο θέμα [Μάθετε περισσότερα σχετικά με την αποτροπή απώλειας δεδομένων τελικών σημείων του Microsoft 365 (προεπισκόπηση)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="183e3-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="183e3-117">**Σημαντικά βήματα συλλογής δεδομένων, εάν απαιτείται υποστήριξη:**</span><span class="sxs-lookup"><span data-stu-id="183e3-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="183e3-118">Λήψη [MDATP Προγράμματος-πελάτη Analyzer Preview.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="183e3-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="183e3-119">Εκτελέστε το εργαλείο ως διαχειριστής από το παράθυρο cmd:</span><span class="sxs-lookup"><span data-stu-id="183e3-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="183e3-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="183e3-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="183e3-121">Όταν σας ζητηθεί με το enter ο αριθμός των λεπτών για τη συλλογή **ανιχνεύει:**, πληκτρολογήστε τον αριθμό των λεπτών που απαιτούνται για την εκτέλεση του σεναρίου.</span><span class="sxs-lookup"><span data-stu-id="183e3-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="183e3-122">Εκτελέστε το σενάριο.</span><span class="sxs-lookup"><span data-stu-id="183e3-122">Run the scenario.</span></span>

<span data-ttu-id="183e3-123">Συλλέξτε το αποτέλεσμα του αρχείου Zip για να το δώσετε στον εκπρόσωπο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="183e3-123">Collect the Zip file output to give to the Support agent.</span></span>
