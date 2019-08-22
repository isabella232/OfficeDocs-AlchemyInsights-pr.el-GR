---
title: Περιορισμός της πρόσβασης στο SharePoint ή OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bc0028626c8934e57e5580477b193a70e49d87be
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504211"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="cddbb-102">Προστασία IRM σε αρχεία του SharePoint</span><span class="sxs-lookup"><span data-stu-id="cddbb-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="cddbb-103">Εντός του SharePoint ηλεκτρονική προστασία IRM εφαρμόζεται σε αρχεία στο επίπεδο λίστας και βιβλιοθήκης.</span><span class="sxs-lookup"><span data-stu-id="cddbb-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="cddbb-104">Ο οργανισμός σας για να χρησιμοποιήσετε την προστασία IRM, πρέπει πρώτα να ορίσει δικαιώματα διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="cddbb-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="cddbb-105">IRM εξαρτάται από την υπηρεσία διαχείρισης δικαιωμάτων Azure από Azure πληροφορίες προστασίας για την κρυπτογράφηση και να αντιστοιχίσετε περιορισμούς χρήσης.</span><span class="sxs-lookup"><span data-stu-id="cddbb-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="cddbb-106">Ορισμένα προγράμματα του Office 365 περιλαμβάνουν Διαχείριση δικαιωμάτων Azure, αλλά όχι όλα.</span><span class="sxs-lookup"><span data-stu-id="cddbb-106">Some Office 365 plans include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="cddbb-107">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα:</span><span class="sxs-lookup"><span data-stu-id="cddbb-107">To learn more, see:</span></span>

- <span data-ttu-id="cddbb-108">[Υπηρεσίες και εφαρμογές του Office πώς υποστηρίζουν διαχείριση δικαιωμάτων Azure](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span><span class="sxs-lookup"><span data-stu-id="cddbb-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="cddbb-109">[Ορισμός ασφαλείας Διαχείριση δικαιωμάτων πληροφοριών (IRM) στο Κέντρο διαχείρισης του SharePoint](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span><span class="sxs-lookup"><span data-stu-id="cddbb-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="cddbb-110">[Λίστες και βιβλιοθήκες εγγράφων του SharePoint τη δυνατότητα IRM](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span><span class="sxs-lookup"><span data-stu-id="cddbb-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="cddbb-111">[Διαχείριση δικαιωμάτων πληροφοριών στο Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span><span class="sxs-lookup"><span data-stu-id="cddbb-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="cddbb-112">[Πληροφορίες δικαιωμάτων διαχείρισης στο Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="cddbb-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span></span>


