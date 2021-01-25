---
title: Προβλήματα με την ανάπτυξη εφαρμογών με API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974617"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="4ba2e-102">Προβλήματα με την ανάπτυξη εφαρμογών με API</span><span class="sxs-lookup"><span data-stu-id="4ba2e-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="4ba2e-103">Για να ξεκινήσετε να χρησιμοποιείτε το API γραφήματος Azure Active Directory, ανατρέξτε στο θέμα [Οδηγός γρήγορης εκκίνησης του Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ή προβολή της [τεκμηρίωσης της αλληλεπιδραστικής αναφοράς αναφοράς API του Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="4ba2e-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="4ba2e-104">**Λήξη υποστήριξης για τη βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και το API του Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="4ba2e-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="4ba2e-105">**Ξεκινώντας στις 30 Ιουνίου, 2020**, δεν θα προσθέτουμε πλέον νέες ΔΥΝΑΤΌΤΗΤΕς στο ADAL και το Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="4ba2e-106">Θα συνεχίσουμε να παρέχουμε τεχνική υποστήριξη και ενημερώσεις ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="4ba2e-107">**Ξεκινώντας στις 30 Ιουνίου, 2022**, θα τερματίσουμε την υποστήριξη για το ADAL και το Azure AD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="4ba2e-108">Οι εφαρμογές που χρησιμοποιούν το ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα έχουν οποιαδήποτε τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="4ba2e-109">Οι εφαρμογές που χρησιμοποιούν το Azure AD Graph μετά από αυτό το διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό σημείο του Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="4ba2e-110">**Μετεγκατάσταση ADAL**</span><span class="sxs-lookup"><span data-stu-id="4ba2e-110">**ADAL Migration**</span></span>

<span data-ttu-id="4ba2e-111">Συνιστούμε να κάνετε ενημέρωση στη [βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), η οποία έχει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="4ba2e-112">Εάν χρησιμοποιείτε τις εφαρμογές της Microsoft, να γνωρίζετε ότι η Microsoft βρίσκεται στη διαδικασία μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι την λήξη της προθεσμίας υποστήριξης, εξασφαλίζοντας ότι θα επωφεληθούν από τις συνεχιζόμενες βελτιώσεις ασφαλείας και δυνατοτήτων του MSAL.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="4ba2e-113">[Διαβάστε τις συνήθεις ερωτήσεις για το ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="4ba2e-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="4ba2e-114">[Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές σε βάση ανά πλατφόρμα](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="4ba2e-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="4ba2e-115">Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιαδήποτε ISV ή υπηρεσίες παροχής εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="4ba2e-116">Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα με όλες τις εφαρμογές που δεν ανήκουν στη Microsoft ADAL στον μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="4ba2e-117">**Μετεγκατάσταση γραφήματος AAD**</span><span class="sxs-lookup"><span data-stu-id="4ba2e-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="4ba2e-118">Για τις εφαρμογές που χρησιμοποιούν το Azure AD Graph, ακολουθήστε τις οδηγίες για τη μετεγκατάσταση [εφαρμογών Azure AD Graph στο Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="4ba2e-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="4ba2e-119">[Ο πίνακας ελέγχου μετεγκατάστασης παρέχει ένα χρονικό ξεκίνημα](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="4ba2e-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="4ba2e-120">Η πύλη δήλωσης της εφαρμογής Azure εμφανίζει ποιες εφαρμογές χρησιμοποιούν το AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="4ba2e-121">Σας συνιστούμε να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιαδήποτε ISV ή υπηρεσίες παροχής εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="4ba2e-122">Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα με όλες AAD τη χρήση γραφημάτων στο μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="4ba2e-123">Για την εφαρμογή σας για την πρόσβαση σε δεδομένα στο Microsoft Graph, ο χρήστης ή ο διαχειριστής πρέπει να του εκχωρήσει τα κατάλληλα δικαιώματα μέσω μιας διαδικασίας συγκατάθεσης.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="4ba2e-124">Η [αναφορά δικαιωμάτων του Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) παραθέτει τα δικαιώματα που σχετίζονται με κάθε κύριο πρόγραμμα API του Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="4ba2e-125">Παρέχει επίσης οδηγίες σχετικά με τον τρόπο χρήσης των δικαιωμάτων.</span><span class="sxs-lookup"><span data-stu-id="4ba2e-125">It also provides guidance about how to use the permissions.</span></span>
