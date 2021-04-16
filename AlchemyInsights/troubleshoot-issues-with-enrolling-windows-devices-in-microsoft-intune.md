---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808971"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="ba928-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ba928-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="ba928-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="ba928-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ba928-104">Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="ba928-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="ba928-105">**Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει.</span><span class="sxs-lookup"><span data-stu-id="ba928-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="ba928-106">Πραγματοποιήστε ξανά λήψη του πακέτου λογισμικού υπολογιστή-πελάτη στην Κονσόλα διαχείρισης Intune.</span><span class="sxs-lookup"><span data-stu-id="ba928-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="ba928-107">Διαβάστε αυτή την τεκμηρίωση για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="ba928-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="ba928-108">**Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να παρουσιαστεί στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="ba928-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="ba928-109">Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="ba928-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="ba928-110">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο της συσκευής.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="ba928-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="ba928-111">Η ρύθμιση "Οι χρήστες μπορούν να συμμετέχουν σε συσκευές στο Azure AD" έχει οριστεί σε "καμία".</span><span class="sxs-lookup"><span data-stu-id="ba928-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="ba928-112">Ορίστε το σε όλους ή επιλέξτε χρήστες.</span><span class="sxs-lookup"><span data-stu-id="ba928-112">Set it to all or select users.</span></span> <span data-ttu-id="ba928-113">Διαβάστε [αυτή την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="ba928-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="ba928-114">Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="ba928-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="ba928-115">Σε αυτή την περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε τη επαναφορά της συσκευής με μη αυτόματο τρόπο προτού δοκιμάσετε ξανά.</span><span class="sxs-lookup"><span data-stu-id="ba928-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="ba928-116">Η συσκευή είναι Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="ba928-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="ba928-117">Μόνο οι SKUs windows 10 Pro, Education και Enterprise μπορούν να συμμετάσχουν στο Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ba928-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="ba928-118">Πρόσθετοι πόροι για την επίλυση του προβλήματος:</span><span class="sxs-lookup"><span data-stu-id="ba928-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="ba928-119">Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="ba928-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ba928-120">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="ba928-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="ba928-121">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνήθη σφάλματα που εμποδίζουν την εγγραφή και τις λύσεις σε καθένα: [Οδηγός αντιμετώπισης προβλημάτων και](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="ba928-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="ba928-122">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Windows στο Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="ba928-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
