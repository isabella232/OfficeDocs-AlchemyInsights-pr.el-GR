---
title: Δικαιώματα και συγκατάθεση API
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974603"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="d37c6-102">Δικαιώματα και συγκατάθεση API</span><span class="sxs-lookup"><span data-stu-id="d37c6-102">API permissions and consent</span></span>

<span data-ttu-id="d37c6-103">Οι εφαρμογές που ενσωματώνονται με την πλατφόρμα ταυτοτήτων της Microsoft ακολουθούν ένα μοντέλο εξουσιοδότησης που παρέχει στους χρήστες και τους διαχειριστές τον έλεγχο του τρόπου με τον οποίο είναι δυνατή η πρόσβαση στα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="d37c6-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="d37c6-104">Η εφαρμογή του μοντέλου εξουσιοδότησης έχει ενημερωθεί στο τελικό σημείο της πλατφόρμας ταυτοτήτων της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d37c6-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="d37c6-105">Αλλάζει τον τρόπο με τον οποίο μια εφαρμογή πρέπει να αλληλεπιδρά με την πλατφόρμα ταυτοτήτων της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d37c6-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="d37c6-106">Τα [δικαιώματα και η συναίνεση στο τελικό σημείο της πλατφόρμας ταυτότητας της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) καλύπτουν τις βασικές έννοιες αυτού του μοντέλου εξουσιοδότησης, συμπεριλαμβανομένων των πεδίων, των δικαιωμάτων και της συγκατάθεσης.</span><span class="sxs-lookup"><span data-stu-id="d37c6-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="d37c6-107">Το [πλαίσιο συναίνεσης του Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) διευκολύνει την ανάπτυξη των εφαρμογών Web πολλών μισθωτών και των εγγενές πρόγραμμα-πελάτη.</span><span class="sxs-lookup"><span data-stu-id="d37c6-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="d37c6-108">Αυτές οι εφαρμογές επιτρέπουν την είσοδο από τους λογαριασμούς χρηστών από έναν μισθωτή AD Azure που είναι διαφορετικός από αυτόν όπου έχει καταχωρηθεί η εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="d37c6-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="d37c6-109">Ενδέχεται επίσης να χρειαστεί να αποκτήσουν πρόσβαση σε API Web, όπως το Microsoft Graph API (για να αποκτήσετε πρόσβαση στο Azure AD, το Intune και τις υπηρεσίες στο Microsoft 365) και στα API άλλων υπηρεσιών της Microsoft, εκτός από τα δικά σας API Web.</span><span class="sxs-lookup"><span data-stu-id="d37c6-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

