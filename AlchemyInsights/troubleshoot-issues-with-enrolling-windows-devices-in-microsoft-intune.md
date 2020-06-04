---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Των Windows στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665832"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="f1ff2-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Των Windows στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f1ff2-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="f1ff2-103">Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f1ff2-104">Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="f1ff2-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="f1ff2-105">**Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="f1ff2-106">Κάντε ξανά λήψη του πακέτου λογισμικού υπολογιστή-πελάτη στην κονσόλα διαχείρισης Intune.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="f1ff2-107">Εξετάστε αυτήν την τεκμηρίωση για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="f1ff2-108">**Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να παρουσιαστεί στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="f1ff2-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="f1ff2-109">Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f1ff2-110">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή [να αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f1ff2-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="f1ff2-111">"Οι χρήστες μπορούν να ενώσουν συσκευές σε Azure AD" έχει οριστεί σε "καμία".</span><span class="sxs-lookup"><span data-stu-id="f1ff2-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="f1ff2-112">Ορίστε το σε όλους ή επιλέξτε χρήστες.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-112">Set it to all or select users.</span></span> <span data-ttu-id="f1ff2-113">Εξετάστε [αυτήν την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="f1ff2-114">Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="f1ff2-115">Σε αυτήν την περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε την εγγραφή της συσκευής με μη αυτόματο τρόπο πριν προσπαθήσετε ξανά.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="f1ff2-116">Η συσκευή είναι Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="f1ff2-117">Μόνο τα Windows 10 Pro, εκπαιδευτικά και εταιρικά SKU μπορούν να συμμετάσχουν στην υπηρεσία καταλόγου Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="f1ff2-118">Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το ζήτημά σας:</span><span class="sxs-lookup"><span data-stu-id="f1ff2-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="f1ff2-119">Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνήθεις αποτυχίες εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f1ff2-120">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="f1ff2-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="f1ff2-121">Εξετάστε αυτά τα έγγραφα για μια λίστα συνηθισμένων σφαλμάτων που εμποδίζουν την εγγραφή και τις λύσεις σε κάθε ένα: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) και [Αντιμετώπιση προβλημάτων εγγράφου](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f1ff2-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="f1ff2-122">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Windows στο Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="f1ff2-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
