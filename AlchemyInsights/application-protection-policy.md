---
title: Πολιτική προστασίας εφαρμογών
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423600"
---
# <a name="application-protection-policy"></a><span data-ttu-id="1d0f0-102">Πολιτική προστασίας εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="1d0f0-102">Application protection policy</span></span>

<span data-ttu-id="1d0f0-103">Αν είστε νέος στην πολιτική προστασίας εφαρμογών (APP), ανατρέξτε στην [επισκόπηση πολιτικών προστασίας εφαρμογών](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="1d0f0-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="1d0f0-104">Για να αρχίσετε να χρησιμοποιείτε το APP, ανατρέξτε στο θέμα [Τρόπος δημιουργίας και αντιστοίχισης πολιτικών προστασίας εφαρμογών](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="1d0f0-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="1d0f0-105">Απαιτήσεις πολιτικής προστασίας εφαρμογών:</span><span class="sxs-lookup"><span data-stu-id="1d0f0-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="1d0f0-106">Ο χρήστης έχει άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="1d0f0-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="1d0f0-107">Ο χρήστης ανήκει σε μια ομάδα που στοχεύει από τις πολιτικές προστασίας εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="1d0f0-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="1d0f0-108">Μόνο ένας εταιρικός χρήστης είναι συνδεδεμένος σε προστατευμένες εφαρμογές σε μια συσκευή.</span><span class="sxs-lookup"><span data-stu-id="1d0f0-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="1d0f0-109">Η εφαρμογή έχει εφαρμόσει το [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="1d0f0-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="1d0f0-110">Για μια λίστα εφαρμογών που υποστηρίζουν το SDK, ανατρέξτε στο θέμα [Προστατευμένες εφαρμογές Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="1d0f0-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="1d0f0-111">Οι πολιτικές ισχύουν όταν ένας χρήστης που πληροί τις παραπάνω απαιτήσεις συνδεθεί σε μια εφαρμογή με δυνατότητα Intune SDK.</span><span class="sxs-lookup"><span data-stu-id="1d0f0-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="1d0f0-112">Ο ευκολότερος τρόπος για να προσδιορίσετε αν εφαρμόζεται μια πολιτική είναι να απαιτείται από το χρήστη να ορίσει μια καρφίτσα στην πολιτική.</span><span class="sxs-lookup"><span data-stu-id="1d0f0-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="1d0f0-113">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="1d0f0-113">For more information, see:</span></span>

[<span data-ttu-id="1d0f0-114">Συνήθεις ερωτήσεις για την αντιμετώπιση προβλημάτων APP/MAM</span><span class="sxs-lookup"><span data-stu-id="1d0f0-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="1d0f0-115">Τρόπος επικύρωσης της ρύθμισης της πολιτικής προστασίας εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="1d0f0-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="1d0f0-116">Κατανόηση του χρονισμού παράδοσης της Πολιτικής προστασίας εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="1d0f0-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="1d0f0-117">Τρόπος εποπτείας των πολιτικών προστασίας εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="1d0f0-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)