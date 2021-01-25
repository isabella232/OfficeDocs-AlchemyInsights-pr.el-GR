---
title: Προβλήματα με την ανάπτυξη εφαρμογών
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974476"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="1ff5b-102">Προβλήματα με την ανάπτυξη εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="1ff5b-102">Issues developing applications</span></span>

<span data-ttu-id="1ff5b-103">Για να αντιμετωπίσετε τα πιο συνηθισμένα προβλήματα κατά τη δημιουργία εφαρμογών Azure Active Directory (AD), ανατρέξτε στα ακόλουθα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="1ff5b-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="1ff5b-104">Αντιμετωπίζω προβλήματα κατά την είσοδο σε εφαρμογές χρησιμοποιώντας μόνο το πρόγραμμα περιήγησης Chrome</span><span class="sxs-lookup"><span data-stu-id="1ff5b-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="1ff5b-105">Δεν γνωρίζω πώς να αλλάξω τις προεπιλογές διάρκειας ζωής διακριτικού για την εφαρμογή μου</span><span class="sxs-lookup"><span data-stu-id="1ff5b-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="1ff5b-106">Είμαι σε σύγχυση σχετικά με τον τρόπο λειτουργίας της συγκατάθεσης εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="1ff5b-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="1ff5b-107">Δεν γνωρίζω πώς να εκχωρήσω δικαιώματα στην εφαρμογή μου</span><span class="sxs-lookup"><span data-stu-id="1ff5b-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="1ff5b-108">Δεν κατανοώ τη διαφορά μεταξύ των δικαιωμάτων ανάθεσης και εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="1ff5b-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="1ff5b-109">\***Λήξη υποστήριξης για τη βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και το API του Azure AD Graph (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="1ff5b-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="1ff5b-110">Ξεκινώντας στις 30 Ιουνίου, 2020, δεν θα προσθέτουμε πλέον νέες δυνατότητες στη βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και στο Azure AD Graph API (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="1ff5b-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="1ff5b-111">Θα συνεχίσουμε να παρέχουμε τεχνική υποστήριξη και ενημερώσεις ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="1ff5b-112">Ξεκινώντας στις 30 Ιουνίου 2022, θα τερματίσουμε την υποστήριξη για το ADAL και το AAD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="1ff5b-113">Ως αποτέλεσμα αυτής της Συνθήκης, οι συνέπειες είναι οι εξής:</span><span class="sxs-lookup"><span data-stu-id="1ff5b-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="1ff5b-114">Οι εφαρμογές που χρησιμοποιούν το ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα έχουν οποιαδήποτε τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="1ff5b-115">Οι εφαρμογές που χρησιμοποιούν το AAD Graph μετά από αυτό το χρονικό διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό σημείο του AAD Graph</span><span class="sxs-lookup"><span data-stu-id="1ff5b-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="1ff5b-116">_ *ADAL μετεγκατάστασης*\*</span><span class="sxs-lookup"><span data-stu-id="1ff5b-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="1ff5b-117">Εάν χρησιμοποιείτε τις εφαρμογές Microsoft, συνιστούμε να κάνετε ενημέρωση στη βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL), η οποία έχει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="1ff5b-118">Αυτή η σύσταση βρίσκεται στο πλαίσιο της Microsoft για την έναρξη της διαδικασίας μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι την λήξη της προθεσμίας υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="1ff5b-119">Η μετεγκατάσταση από τη Microsoft των εφαρμογών της στο MSAL διασφαλίζει ότι οι εφαρμογές επωφελούνται από τη συνεχιζόμενη βελτίωση της ασφάλειας και των δυνατοτήτων του MSAL.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="1ff5b-120">Διαβάστε τις συνήθεις ερωτήσεις για το ADAL</span><span class="sxs-lookup"><span data-stu-id="1ff5b-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="1ff5b-121">Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές σε βάση ανά πλατφόρμα</span><span class="sxs-lookup"><span data-stu-id="1ff5b-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="1ff5b-122">Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιουσδήποτε ανεξάρτητους προμηθευτές λογισμικού (ISV) ή υπηρεσίες παροχής εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="1ff5b-123">Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα με όλες τις εφαρμογές που δεν ανήκουν στη Microsoft ADAL στον μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="1ff5b-124">**Μετεγκατάσταση γραφήματος AAD**</span><span class="sxs-lookup"><span data-stu-id="1ff5b-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="1ff5b-125">Για εφαρμογές που χρησιμοποιούν το AAD Graph, ακολουθήστε τις οδηγίες μας για να μετεγκαταστήσετε τις εφαρμογές Graph του AAD στο Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="1ff5b-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="1ff5b-126">[Ο πίνακας ελέγχου μετεγκατάστασης παρέχει ένα χρονικό ξεκίνημα](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="1ff5b-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="1ff5b-127">Η πύλη δήλωσης της εφαρμογής Azure εμφανίζει ποιες εφαρμογές χρησιμοποιούν το AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="1ff5b-128">Σας συνιστούμε να εξετάσετε όλο τον πηγαίο κώδικα των εφαρμογών σας και, εάν υπάρχει, να επικοινωνήσετε με οποιουσδήποτε ανεξάρτητους προμηθευτές λογισμικού (ISV) ή υπηρεσίες παροχής εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="1ff5b-129">Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει πληροφορίες σχετικά με τη χρήση του AAD Graph στον μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="1ff5b-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







