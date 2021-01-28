---
title: Προβλήματα με τις αξιώσεις και τα χαρακτηριστικά διακριτικού
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035891"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="fbc56-102">Προβλήματα με τις αξιώσεις και τα χαρακτηριστικά διακριτικού</span><span class="sxs-lookup"><span data-stu-id="fbc56-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="fbc56-103">**Ενημέρωση, ρύθμιση παραμέτρων ή κατάργηση αξιώσεις διακριτικού**</span><span class="sxs-lookup"><span data-stu-id="fbc56-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="fbc56-104">Χρησιμοποιώντας το Azure Active Directory (Azure AD), μπορείτε να προσαρμόσετε τον τύπο αξίωσης για την αξίωση ρόλου στο διακριτικό απάντησης που λαμβάνετε μετά την εξουσιοδότηση μιας εφαρμογής. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)</span><span class="sxs-lookup"><span data-stu-id="fbc56-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="fbc56-105">Οι προγραμματιστές εφαρμογών μπορούν να χρησιμοποιήσουν προαιρετικές αξιώσεις στις εφαρμογές του Azure AD για να καθορίσουν ποιες αξιώσεις θέλουν στα διακριτικά που αποστέλλονται στην εφαρμογή τους.</span><span class="sxs-lookup"><span data-stu-id="fbc56-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="fbc56-106">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Παροχή προαιρετικών αξιώ σεων στην εφαρμογή σας".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="fbc56-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="fbc56-107">[Ρυθμίστε τις παραμέτρους αξιώσεις ομάδας για εφαρμογές με το Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="fbc56-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="fbc56-108">Εάν χρησιμοποιείτε απρόσκοπτη σύνδεση μονής πρόσβασης στην εφαρμογή σας, ανατρέξτε στις αιτήσεις προσαρμογής που εκδίδονται στο [διακριτικό SAML για τις εφαρμογές για μεγάλες επιχειρήσεις.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="fbc56-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="fbc56-109">**Αντιστοίχιση χαρακτηριστικών διεκδίκησης**</span><span class="sxs-lookup"><span data-stu-id="fbc56-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="fbc56-110">Για να ρυθμίσετε τις παραμέτρους πολιτικής αντιστοίχισης αξιώσεις χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα "Προσαρμογή αξιώσεων που μεταδίδονται σε διακριτικά για μια συγκεκριμένη εφαρμογή [σε ένα μισθωτή (Προεπισκόπηση)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="fbc56-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="fbc56-111">Τα χαρακτηριστικά επέκτασης σχήματος καταλόγου παρέχουν έναν τρόπο για την αποθήκευση πρόσθετων δεδομένων στο Azure Active Directory σε αντικείμενα χρηστών και άλλα αντικείμενα καταλόγου, όπως ομάδες, λεπτομέρειες μισθωτή, αρχές υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="fbc56-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="fbc56-112">Μόνο τα χαρακτηριστικά επέκτασης στα αντικείμενα χρήστη μπορούν να χρησιμοποιηθούν για την εμφάνιση αξιώ σε εφαρμογές.</span><span class="sxs-lookup"><span data-stu-id="fbc56-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="fbc56-113">[Η χρήση χαρακτηριστικών επέκτασης σχήματος καταλόγου σε αξιώσεις](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) περιγράφει πώς μπορείτε να χρησιμοποιήσετε χαρακτηριστικά επέκτασης σχήματος καταλόγου για την αποστολή δεδομένων χρήστη σε εφαρμογές σε αξιώσεις διακριτικού.</span><span class="sxs-lookup"><span data-stu-id="fbc56-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="fbc56-114">Για περισσότερες πληροφορίες σχετικά με τις αξιώσεις διακριτικού, ανατρέξτε στα εξής:</span><span class="sxs-lookup"><span data-stu-id="fbc56-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="fbc56-115">Αξιώσεις σε διακριτικά πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="fbc56-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="fbc56-116">Αξιώσεις σε id_token</span><span class="sxs-lookup"><span data-stu-id="fbc56-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="fbc56-117">[Αξιώσεις](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) που μπορείτε να αναμένετε από τα διακριτικά αναγνωριστικού και τα διακριτικά πρόσβασης που εκδίδονται από το Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="fbc56-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="fbc56-118">Αναφορά αξιώ σεων διακριτικού SAML</span><span class="sxs-lookup"><span data-stu-id="fbc56-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
