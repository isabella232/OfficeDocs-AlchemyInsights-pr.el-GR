---
title: Ρύθμιση παραμέτρων διακομιστή μεσολάβησης εφαρμογής
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885132"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="5ab82-102">Ρύθμιση παραμέτρων διακομιστή μεσολάβησης εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="5ab82-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="5ab82-103">Για να καταλάβετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους μιας εφαρμογής διακομιστή μεσολάβησης εφαρμογής εντός του Azure AD για να εκθέσετε τις εφαρμογές εσωτερικής εγκατάστασης στο cloud, ανατρέξτε στο θέμα [Πώς μπορείτε να ρυθμίσετε τις παραμέτρους μιας εφαρμογής διακομιστή μεσολάβησης εφαρμογής](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="5ab82-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="5ab82-104">Η καθολική σύνδεση (SSO) επιτρέπει στους χρήστες σας να έχουν πρόσβαση σε μια εφαρμογή χωρίς έλεγχο ταυτότητας πολλές φορές.</span><span class="sxs-lookup"><span data-stu-id="5ab82-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="5ab82-105">Επιτρέπει την εκτέλεση του μοναδικού ελέγχου ταυτότητας στο cloud, έναντι του Azure Active Directory και επιτρέπει στην υπηρεσία ή τη γραμμή σύνδεσης να μιμηθεί το χρήστη για να ολοκληρώσει τυχόν πρόσθετες προκλήσεις ελέγχου ταυτότητας από την εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="5ab82-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="5ab82-106">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα [Πώς μπορείτε να ρυθμίσετε τις παραμέτρους καθολικής σύνδεσης σε μια εφαρμογή διακομιστή μεσολάβησης εφαρμογής](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="5ab82-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="5ab82-107">Χρησιμοποιήστε [αυτό το άρθρο](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) για να αντιμετωπίσετε συνηθισμένα προβλήματα που αντιμετωπίζουν οι χρήστες κατά τη δημιουργία μιας νέας εφαρμογής διακομιστή μεσολάβησης εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="5ab82-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="5ab82-108">Εάν αντιμετωπίζετε πρόβλημα με τη ρύθμιση του ελέγχου ταυτότητας παρασκηνίου στην εφαρμογή σας, ίσως χρειαστεί να [αντιμετωπίσετε τις ρυθμίσεις παραμέτρων αντιπροσώπευσης του Kerberos για το διακομιστή μεσολάβησης εφαρμογής](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ή να ακολουθήσετε οδηγίες σχετικά [με τη ρύθμιση παραμέτρων της εφαρμογής με το PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) για να επιλύσετε το ζήτημά σας.</span><span class="sxs-lookup"><span data-stu-id="5ab82-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
