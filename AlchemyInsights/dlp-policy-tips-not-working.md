---
title: Οι συμβουλές πολιτικής DLP δεν λειτουργούν
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958702"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="39b9d-102">Ζητήματα συμβουλής πολιτικής DLP</span><span class="sxs-lookup"><span data-stu-id="39b9d-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="39b9d-103">**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="39b9d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="39b9d-104">Για να ρυθμίσετε τις παραμέτρους συμβουλών πολιτικής σχετικά με την πολιτική DLP στο Κέντρο ασφάλειας & συμμόρφωσης σε λειτουργία πλήρους επιβολής, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="39b9d-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="39b9d-105">Βεβαιωθείτε ότι οι συμβουλές πολιτικής **έχουν ενεργοποιηθεί** στον κανόνα DLP.</span><span class="sxs-lookup"><span data-stu-id="39b9d-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="39b9d-106">Για τα βήματα, ανατρέξτε [στο θέμα Αποστολή ειδοποιήσεων ηλεκτρονικού ταχυδρομείου και εμφάνιση συμβουλών πολιτικής για τις πολιτικές DLP.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="39b9d-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="39b9d-107">Βεβαιωθείτε ότι το περιεχόμενό σας ταιριάζει με αυτό που απαιτείται για την ενεργοποίηση του κανόνα που περιγράφεται στους [ορισμούς οντότητας τύπου ευαίσθητων πληροφοριών.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="39b9d-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="39b9d-108">Οι συμβουλές πολιτικής εμφανίζονται τόσο στο OWA όσο και στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="39b9d-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="39b9d-109">Ωστόσο, όταν χρησιμοποιείτε το Outlook 2013 ή νεότερη έκδοση, οι συμβουλές πολιτικής εμφανίζονται μόνο υπό ορισμένες συνθήκες.</span><span class="sxs-lookup"><span data-stu-id="39b9d-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="39b9d-110">Για τη λίστα συγκεκριμένων συνθηκών, ανατρέξτε στο θέμα Υποστηριζόμενες συνθήκες για το [Outlook 2013 ή νεότερη έκδοση για την εμφάνιση συμβουλών πολιτικής.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="39b9d-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="39b9d-111">Για πληροφορίες σχετικά με τις συμβουλές πολιτικής DLP, ανατρέξτε στο θέμα ["Αναφορά συμβουλών πολιτικής DLP"](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) και ["Πίνακας υποστήριξης" για συμβουλές πολιτικής DLP.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="39b9d-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>