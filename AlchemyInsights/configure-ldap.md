---
title: Ρύθμιση παραμέτρων LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885160"
---
# <a name="configure-ldap"></a><span data-ttu-id="b6680-102">Ρύθμιση παραμέτρων LDAP</span><span class="sxs-lookup"><span data-stu-id="b6680-102">Configure LDAP</span></span>

<span data-ttu-id="b6680-103">Για να ρυθμίσετε τις παραμέτρους του LDAP, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="b6680-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="b6680-104">Επιλέξτε την εύρυθμη λειτουργία του τομέα σας στην [πύλη Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="b6680-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="b6680-105">Βεβαιωθείτε ότι είναι διαθέσιμη μια έγκυρη συνδρομή Azure AD και ότι οι υπηρεσίες τομέα AD Azure έχουν ενεργοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="b6680-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="b6680-106">Το πιστοποιητικό που απαιτείται για την ενεργοποίηση του ασφαλούς LDAP πρέπει να λαμβάνεται από μια αξιόπιστη δημόσια αρχή έκδοσης πιστοποιητικών ή να είναι ένα πιστοποιητικό αυτόματης υπογραφής.</span><span class="sxs-lookup"><span data-stu-id="b6680-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="b6680-107">Βεβαιωθείτε ότι το πιστοποιητικό ακολουθεί τις απαιτούμενες [οδηγίες](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="b6680-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="b6680-108">**Μη έγκυρο πιστοποιητικό**</span><span class="sxs-lookup"><span data-stu-id="b6680-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="b6680-109">Για να ανανεώσετε ένα πιστοποιητικό, ακολουθήστε τα βήματα για να δημιουργήσετε ένα νέο πιστοποιητικό και να κάνετε ξανά αποστολή: [Ρύθμιση παραμέτρων LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b6680-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="b6680-110">Για να επιλύσετε ένα γνωστό πρόβλημα με ασφαλείς ειδοποιήσεις LDAP στις υπηρεσίες τομέα Active Directory Azure, ανατρέξτε στο θέμα [επίλυση ΕΙΔΟΠΟΙΉΣΕΩΝ LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b6680-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
