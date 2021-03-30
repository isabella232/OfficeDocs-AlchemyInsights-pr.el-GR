---
title: Αντιμετώπιση προβλημάτων του συνδέσμου Hybrid Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401907"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="eff11-102">Αντιμετώπιση προβλημάτων του συνδέσμου Hybrid Azure AD</span><span class="sxs-lookup"><span data-stu-id="eff11-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="eff11-103">Συνιστάται ιδιαίτερα. Εξασφαλίστε ότι μια συσκευή έχει πρόσβαση στα τελικά σημεία εγγραφής συσκευής κάτω από τον λογαριασμό συστήματος, χρησιμοποιώντας τη [δέσμη ενεργειών "Δοκιμή συνδεσιμότητας εγγραφής συσκευής"](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="eff11-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="eff11-104">Εάν ρυθμίζετε εγγραφές συσκευών για πρώτη φορά, φροντίστε να εξετάσετε την ενότητα [Εισαγωγή στη διαχείριση συσκευών στο Microsoft Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) για να μάθετε πώς μπορείτε να θέσετε τις συσκευές υπό τον έλεγχο του Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eff11-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="eff11-105">Εάν καταχωρείτε συσκευές απευθείας στο Microsoft Azure Active Directory και τις έχετε εγγράψει στο Intune, βεβαιωθείτε ότι έχετε ρυθμίσει τις [παραμέτρους του Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) και έχετε στη θέση τους τις [άδειες χρήσης](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="eff11-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="eff11-106">Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Microsoft Azure Active Directory και στην υπηρεσία καταλόγου AD εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="eff11-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="eff11-107">Μόνο ένας καθολικός διαχειριστής στο Microsoft Azure Active Directory μπορεί να διαχειρίζεται τις ρυθμίσεις για εγγραφές συσκευών.</span><span class="sxs-lookup"><span data-stu-id="eff11-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="eff11-108">Επιπλέον, εάν ρυθμίζετε τις αυτόματες εγγραφές στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, θα πρέπει να είστε διαχειριστής της υπηρεσίας καταλόγου Active Directory και των υπηρεσιών AD FS (εάν υπάρχουν).</span><span class="sxs-lookup"><span data-stu-id="eff11-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="eff11-109">Για περισσότερες λεπτομέρειες σχετικά με την επίλυση πιθανών προβλημάτων με τον σύνδεσμο Hybrid, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων του συνδέσμου Hybrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Για τη ρύθμιση σύνδεσης μέσω Hybrid Azure AD και τη Διαχείριση συσκευών χρησιμοποιώντας την πύλη Azure AD, ανατρέξτε στο θέμα [Ρύθμιση συσκευών σε σύνδεση μέσω Hybrid Azure AD (με σύνδεση τομέα εσωτερικής εγκατάστασης)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) και [Διαχείριση συσκευών χρησιμοποιώντας την πύλη Microsoft Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="eff11-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="eff11-110">Για να επιλύσετε συνήθη ζητήματα σχετικά με τον σύνδεσμο Hybrid Azure Active Directory (AD), ανατρέξτε στο θέμα [Συνήθεις ερωτήσεις για τον σύνδεσμο Hybrid Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="eff11-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
