---
title: Ρύθμιση παραμέτρων και επέκταση διάρκειας ζωής διακριτικού
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916826"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="8cc6f-102">Ρύθμιση παραμέτρων και επέκταση διάρκειας ζωής διακριτικού</span><span class="sxs-lookup"><span data-stu-id="8cc6f-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="8cc6f-103">Μπορείτε να καθορίσετε τη διάρκεια ζωής ενός διακριτικού Access, SAML ή ΑΝΑΓΝΩΡΙΣΤΙΚού που έχει εκδοθεί από την πλατφόρμα ταυτοτήτων της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="8cc6f-104">Μπορείτε να καθορίσετε τη διάρκεια ζωής διακριτικού για όλες τις εφαρμογές στον οργανισμό σας, για μια εφαρμογή πολλαπλών μισθωτών (πολλών οργανισμών) ή για μια συγκεκριμένη κύρια υπηρεσία στην εταιρεία σας.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="8cc6f-105">Για περισσότερες πληροφορίες, Διαβάστε τη [διάρκεια ζωής διακριτικού](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)με δυνατότητα ρύθμισης.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="8cc6f-106">Για παραδείγματα, διαβάστε [παραδείγματα για το πώς μπορείτε να ρυθμίσετε τις παραμέτρους των διακριτικών ζωών](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="8cc6f-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="8cc6f-107">Για να μάθετε πώς μπορείτε να ρυθμίσετε τη διάρκεια ζωής και τη συμβατότητα ενός διακριτικού στο Azure Active Directory B2C (Azure AD B2C), ανατρέξτε [στο θέμα Ρύθμιση παραμέτρων διακριτικού στο Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="8cc6f-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="8cc6f-108">Το άρθρο [Ρύθμιση παραμέτρων της συμπεριφοράς περιόδου λειτουργίας στο Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) περιγράφει τις μεθόδους καθολικής ΣΎΝΔΕΣΗς (SSO) που χρησιμοποιούνται στο Azure AD B2C και σας βοηθά να επιλέξετε την καταλληλότερη μέθοδο SSO κατά τη ρύθμιση των παραμέτρων της πολιτικής σας.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="8cc6f-109">**Πόσο διαρκούν τα κουπόνια; Για πόσο χρόνο ισχύουν;**</span><span class="sxs-lookup"><span data-stu-id="8cc6f-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="8cc6f-110">Η διάρκεια ζωής διακριτικού είναι 1 ώρα και η διάρκεια ζωής της περιόδου λειτουργίας είναι 24 ώρες.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="8cc6f-111">Αυτό σημαίνει ότι εάν δεν έχουν γίνει αιτήσεις σε 24 ώρες, θα πρέπει να συνδεθείτε ξανά πριν να ζητήσετε ένα νέο διακριτικό.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="8cc6f-112">Μετά τις 30 Μαΐου, 2020, κανένας νέος μισθωτής δεν θα μπορεί να χρησιμοποιήσει την πολιτική διακριτικού διάρκειας ζωής διακριτικού για να ρυθμίσει τις παραμέτρους των διακριτικών περιόδου λειτουργίας και ανανέωσης.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="8cc6f-113">Η αποδοκιμασία θα συμβεί εντός αρκετών μηνών μετά από αυτό, γεγονός που σημαίνει ότι θα πάψουμε να τιμούμε τις υπάρχουσες περιόδους λειτουργίας και να ανανεώνουμε τις πολιτικές tokens.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="8cc6f-114">Εξακολουθείτε να μπορείτε να ρυθμίσετε τις παραμέτρους της διάρκειας ζωής διακριτικού πρόσβασης μετά την αποδοκιμασία.</span><span class="sxs-lookup"><span data-stu-id="8cc6f-114">You can still configure access token lifetimes after the deprecation.</span></span>






