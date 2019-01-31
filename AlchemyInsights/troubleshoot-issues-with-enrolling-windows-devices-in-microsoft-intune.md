---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών των Windows στα Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661533"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="28e47-102">Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών των Windows στα Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="28e47-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="28e47-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="28e47-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="28e47-104">Ορισμένα κοινά μηνύματα λάθους και τα βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="28e47-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="28e47-p101">**Το λογισμικό δεν είναι εγκατεστημένο, 0x80cf4017:** Έχει λήξει το πιστοποιητικό του λογαριασμού σας. Εκ νέου λήψη του πακέτου λογισμικού PC υπολογιστή-πελάτη στην κονσόλα διαχείρισης του Intune. Εξετάστε αυτήν την τεκμηρίωση για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="28e47-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="28e47-108">**Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να προκύψει στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="28e47-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="28e47-p102">Ο χρήστης έχει περισσότερες συσκευές που συμμετέχουν από το όριο συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="28e47-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="28e47-p103">"Οι χρήστες μπορούν να συμμετέχουν συσκευές σε Azure AD" έχει οριστεί σε "Κανένα". Ορίστε την σε όλους ή επιλέξτε χρήστες. Εξετάστε [αυτήν την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="28e47-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="28e47-p104">Η συσκευή είναι ήδη συμμετέχουν από κάποιον άλλο χρήστη. Εάν συμβαίνει αυτό, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή unenroll με μη αυτόματο τρόπο τη συσκευή πριν να προσπαθήσετε πάλι.</span><span class="sxs-lookup"><span data-stu-id="28e47-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="28e47-p105">Η συσκευή είναι 10 Windows Home. Μόνο Windows 10 Pro, εκπαίδευση και Enterprise SKU να συμμετάσχετε Azure υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="28e47-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="28e47-118">Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="28e47-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="28e47-p106">Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="28e47-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="28e47-121">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και λύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="28e47-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="28e47-122">[Μάθετε πώς μπορείτε να εγγραφείτε συσκευές Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="28e47-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

