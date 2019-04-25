---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών των Windows στα Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390643"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="c3f38-102">Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών των Windows στα Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c3f38-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="c3f38-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="c3f38-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c3f38-104">Ορισμένα κοινά μηνύματα λάθους και τα βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="c3f38-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="c3f38-105">**Το λογισμικό δεν είναι εγκατεστημένο, 0x80cf4017:** Έχει λήξει το πιστοποιητικό του λογαριασμού σας.</span><span class="sxs-lookup"><span data-stu-id="c3f38-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="c3f38-106">Εκ νέου λήψη του πακέτου λογισμικού PC υπολογιστή-πελάτη στην κονσόλα διαχείρισης του Intune.</span><span class="sxs-lookup"><span data-stu-id="c3f38-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="c3f38-107">Εξετάστε αυτήν την τεκμηρίωση για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="c3f38-107">Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="c3f38-108">**Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να προκύψει στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="c3f38-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="c3f38-109">Ο χρήστης έχει περισσότερες συσκευές που συμμετέχουν από το όριο συσκευής.</span><span class="sxs-lookup"><span data-stu-id="c3f38-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c3f38-110">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="c3f38-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="c3f38-111">"Οι χρήστες μπορούν να συμμετέχουν συσκευές σε Azure AD" έχει οριστεί σε "Κανένα".</span><span class="sxs-lookup"><span data-stu-id="c3f38-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="c3f38-112">Ορίστε την σε όλους ή επιλέξτε χρήστες.</span><span class="sxs-lookup"><span data-stu-id="c3f38-112">Set it to all or select users.</span></span> <span data-ttu-id="c3f38-113">Εξετάστε [αυτήν την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="c3f38-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="c3f38-114">Η συσκευή είναι ήδη συμμετέχουν από κάποιον άλλο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="c3f38-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="c3f38-115">Εάν συμβαίνει αυτό, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή unenroll με μη αυτόματο τρόπο τη συσκευή πριν να προσπαθήσετε πάλι.</span><span class="sxs-lookup"><span data-stu-id="c3f38-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="c3f38-116">Η συσκευή είναι 10 Windows Home.</span><span class="sxs-lookup"><span data-stu-id="c3f38-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="c3f38-117">Μόνο Windows 10 Pro, εκπαίδευση και Enterprise SKU να συμμετάσχετε Azure υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c3f38-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="c3f38-118">Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="c3f38-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c3f38-119">Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="c3f38-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c3f38-120">Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="c3f38-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c3f38-121">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και λύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c3f38-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="c3f38-122">[Μάθετε πώς μπορείτε να εγγραφείτε συσκευές Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="c3f38-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

