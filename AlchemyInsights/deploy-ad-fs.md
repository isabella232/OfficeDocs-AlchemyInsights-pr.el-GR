---
title: Ανάπτυξη AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177547"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="d0b81-102">Ανάπτυξη AD FS</span><span class="sxs-lookup"><span data-stu-id="d0b81-102">Deploy AD FS</span></span>

<span data-ttu-id="d0b81-103">Μια ανάπτυξη των υπηρεσιών Active Directory Federation Services (AD FS) χρησιμοποιεί την υποδομή εσωτερικής εγκατάστασης για τον έλεγχο ταυτότητας των χρηστών για τις υπηρεσίες του Office 365.</span><span class="sxs-lookup"><span data-stu-id="d0b81-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="d0b81-104">Με την ομόσπονδη είσοδο, μπορείτε να επιτρέψετε στους χρήστες να πραγματοποιήσουν είσοδο σε υπηρεσίες και λογισμικό του Office 365 ως υπηρεσία (SAAS) που είναι ενσωματωμένες στο Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d0b81-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="d0b81-105">Η ομόσπονδη είσοδος πιστοποιεί τους χρήστες με την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης μέσω των υπηρεσιών AD FS.</span><span class="sxs-lookup"><span data-stu-id="d0b81-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="d0b81-106">Επίσης, ενώ είστε στο εταιρικό δίκτυο, οι χρήστες δεν θα χρειαστεί να επαναφερούν τους κωδικούς πρόσβασής τους.</span><span class="sxs-lookup"><span data-stu-id="d0b81-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="d0b81-107">Ο σύμβουλος ανάπτυξης των υπηρεσιών [AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) παρέχει αναλυτικές οδηγίες σχετικά με την ανάπτυξη μιας υποδομής ΥΠΗΡΕΣΙΏΝ AD FS εσωτερικής εγκατάστασης που ελέγχει τον έλεγχο ταυτότητας των χρηστών για τις υπηρεσίες του Microsoft 365 και του Office 365.</span><span class="sxs-lookup"><span data-stu-id="d0b81-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="d0b81-108">Με αυτόν τον οδηγό, ο οργανισμός σας μπορεί να εξετάζει στοιχεία και απαιτήσεις υπηρεσιών AD FS, να αποκτά και να εγκαθιστά πιστοποιητικά SSL που είναι απαραίτητα για την ανάπτυξη και να εγκαθιστά έναν απαιτούμενο διακομιστή μεσολάβησης εφαρμογών Web.</span><span class="sxs-lookup"><span data-stu-id="d0b81-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
