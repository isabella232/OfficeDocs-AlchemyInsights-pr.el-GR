---
title: DLP Συμβουλές πολιτικής δεν λειτουργεί
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 6375fa8077529f36ae95d6632ad4d2db5625dc29
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977234"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="cf992-102">Ζητήματα συμβουλής πολιτικής DLP</span><span class="sxs-lookup"><span data-stu-id="cf992-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="cf992-103">**Σημαντικό:** Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες – Επισκεφθείτε [τις προσωρινές προσαρμογές δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="cf992-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="cf992-104">**Συμβουλές πολιτικής DLP**</span><span class="sxs-lookup"><span data-stu-id="cf992-104">**DLP policy tips**</span></span>

<span data-ttu-id="cf992-105">Όταν χρησιμοποιείτε **τις πολιτικές DLP**, οι χρήστες μπορούν να ειδοποιηθούν για μια παραβίαση πολιτικής με **συμβουλές πολιτικής**.</span><span class="sxs-lookup"><span data-stu-id="cf992-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="cf992-106">Οι διαχειριστές μπορούν να ρυθμίσουν τις παραμέτρους των συμβουλών πολιτικής για εμφάνιση κατά τον έλεγχο της πολιτικής DLP ή όταν η πολιτική βρίσκεται σε κατάσταση πλήρους επιβολής.</span><span class="sxs-lookup"><span data-stu-id="cf992-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="cf992-107">Για να ρυθμίσετε τις συμβουλές πολιτικής σχετικά με την πολιτική DLP στο κέντρο ασφάλειας και συμμόρφωσης σε κατάσταση πλήρους επιβολής, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="cf992-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="cf992-108">Βεβαιωθείτε ότι οι συμβουλές πολιτικής έχουν **ενεργοποιηθεί** στον κανόνα DLP χρησιμοποιώντας τα βήματα [εδώ](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="cf992-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="cf992-109">Βεβαιωθείτε ότι **το περιεχόμενό** σας ταιριάζει με αυτό που **απαιτείται** για την ενεργοποίηση του κανόνα που περιγράφεται σε αυτό το άρθρο [εδώ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="cf992-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="cf992-110">Οι συμβουλές πολιτικής εμφανίζονται τόσο στο OWA όσο και στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="cf992-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="cf992-111">Ωστόσο, όταν χρησιμοποιείτε **το Outlook 2013 ή νεότερη έκδοση**, οι συμβουλές πολιτικής εμφανίζονται μόνο υπό ορισμένες συνθήκες.</span><span class="sxs-lookup"><span data-stu-id="cf992-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="cf992-112">Αυτές οι συνθήκες παρατίθενται εδώ: [Υποστηριζόμενες συνθήκες για το Outlook 2013 ή νεότερη έκδοση για την εμφάνιση συμβουλών πολιτικής](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="cf992-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="cf992-113">Για πρόσθετες πληροφορίες σχετικά με τις συμβουλές πολιτικής DLP, ανατρέξτε στο θέμα: [Εμφάνιση συμβουλών πολιτικής για τις πολιτικές DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="cf992-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  