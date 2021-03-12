---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708890"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="81906-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="81906-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="81906-103">Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="81906-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="81906-104">Ορισμένα συνήθη μηνύματα σφάλματος και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="81906-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="81906-105">**Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει.</span><span class="sxs-lookup"><span data-stu-id="81906-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="81906-106">Κάντε εκ ξανά λήψη του πακέτου λογισμικού προγράμματος-πελάτη υπολογιστή στην κονσόλα διαχείρισης Intune.</span><span class="sxs-lookup"><span data-stu-id="81906-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="81906-107">Ανατρέξτε σε αυτή την τεκμηρίωση για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="81906-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="81906-108">**Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να προκύψει στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="81906-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="81906-109">Ο χρήστης έχει εγγράψει περισσότερες συσκευές σε σχέση με το όριο συσκευών.</span><span class="sxs-lookup"><span data-stu-id="81906-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="81906-110">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο συσκευών.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="81906-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="81906-111">Η ρύθμιση "Οι χρήστες μπορούν να συμμετάσχουν σε συσκευές στο Azure AD" ορίζεται σε "καμία".</span><span class="sxs-lookup"><span data-stu-id="81906-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="81906-112">Ρυθμίστε το σε όλους ή επιλέξτε χρήστες.</span><span class="sxs-lookup"><span data-stu-id="81906-112">Set it to all or select users.</span></span> <span data-ttu-id="81906-113">Ανατρέξτε [σε αυτή την](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) τεκμηρίωση για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="81906-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="81906-114">Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="81906-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="81906-115">Σε αυτή την περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε τη μισθοδοσία της συσκευής με μη αυτόματο τρόπο πριν να δοκιμάσετε ξανά.</span><span class="sxs-lookup"><span data-stu-id="81906-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="81906-116">Η συσκευή είναι Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="81906-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="81906-117">Μόνο οι SKUs των Windows 10 Pro, Education και Enterprise μπορούν να συμμετάσχουν στο Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81906-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="81906-118">Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="81906-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="81906-119">Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων του Intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) τη διάγνωση και την επίλυση συνηθισμένων αποτυχιών εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="81906-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="81906-120">Ελέγξτε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="81906-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="81906-121">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και την επίλυση του [καθένα:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Οδηγός αντιμετώπισης προβλημάτων και [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="81906-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="81906-122">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Windows στο Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="81906-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
