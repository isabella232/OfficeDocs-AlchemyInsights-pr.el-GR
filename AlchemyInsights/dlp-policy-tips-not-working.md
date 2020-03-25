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
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932586"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="7a019-102">Ζητήματα συμβουλής πολιτικής DLP</span><span class="sxs-lookup"><span data-stu-id="7a019-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="7a019-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="7a019-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7a019-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="7a019-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7a019-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="7a019-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7a019-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="7a019-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7a019-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="7a019-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7a019-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="7a019-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7a019-109">**Συμβουλές πολιτικής DLP**</span><span class="sxs-lookup"><span data-stu-id="7a019-109">**DLP policy tips**</span></span>

<span data-ttu-id="7a019-110">Όταν χρησιμοποιείτε **τις πολιτικές DLP**, οι χρήστες μπορούν να ειδοποιηθούν για μια παραβίαση πολιτικής με **συμβουλές πολιτικής**.</span><span class="sxs-lookup"><span data-stu-id="7a019-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="7a019-111">Οι διαχειριστές μπορούν να ρυθμίσουν τις παραμέτρους των συμβουλών πολιτικής για εμφάνιση κατά τον έλεγχο της πολιτικής DLP ή όταν η πολιτική βρίσκεται σε κατάσταση πλήρους επιβολής.</span><span class="sxs-lookup"><span data-stu-id="7a019-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="7a019-112">Για να ρυθμίσετε τις συμβουλές πολιτικής σχετικά με την πολιτική DLP στο κέντρο ασφάλειας και συμμόρφωσης σε κατάσταση πλήρους επιβολής, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="7a019-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="7a019-113">Βεβαιωθείτε ότι οι συμβουλές πολιτικής έχουν **ενεργοποιηθεί** στον κανόνα DLP χρησιμοποιώντας τα βήματα [εδώ](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="7a019-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="7a019-114">Βεβαιωθείτε ότι **το περιεχόμενό** σας ταιριάζει με αυτό που **απαιτείται** για την ενεργοποίηση του κανόνα που περιγράφεται σε αυτό το άρθρο [εδώ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="7a019-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="7a019-115">Οι συμβουλές πολιτικής εμφανίζονται τόσο στο OWA όσο και στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="7a019-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="7a019-116">Ωστόσο, όταν χρησιμοποιείτε **το Outlook 2013 ή νεότερη έκδοση**, οι συμβουλές πολιτικής εμφανίζονται μόνο υπό ορισμένες συνθήκες.</span><span class="sxs-lookup"><span data-stu-id="7a019-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="7a019-117">Αυτές οι συνθήκες παρατίθενται εδώ: [Υποστηριζόμενες συνθήκες για το Outlook 2013 ή νεότερη έκδοση για την εμφάνιση συμβουλών πολιτικής](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="7a019-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="7a019-118">Για πρόσθετες πληροφορίες σχετικά με τις συμβουλές πολιτικής DLP, ανατρέξτε στο θέμα: [Εμφάνιση συμβουλών πολιτικής για τις πολιτικές DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="7a019-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  