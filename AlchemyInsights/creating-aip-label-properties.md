---
title: Δημιουργία πολιτικών ετικετών AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732175"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="0a1a5-102">Δημιουργία πολιτικών ετικετών AIP</span><span class="sxs-lookup"><span data-stu-id="0a1a5-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="0a1a5-103">Οι ετικέτες προστασίας πληροφοριών Azure (AIP) μπορούν να χρησιμοποιηθούν με το πλήρες εύρος των δεδομένων που συνήθως δημιουργεί ένας οργανισμός και αποθηκεύει, από τη χαμηλότερη ταξινόμηση των προσωπικών δεδομένων, μέχρι την υψηλότερη κατάταξη άκρως εμπιστευτικών δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="0a1a5-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="0a1a5-104">Οι πολιτικές προστασίας πληροφοριών του Azure ισχύουν για το κλασικό πρόγραμμα-πελάτη προστασίας πληροφοριών Azure (AIP) και όχι το  [πρόγραμμα-πελάτη ενοποιημένων ετικετών AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="0a1a5-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="0a1a5-105">Μπορείτε να ρυθμίσετε τις παραμέτρους πολλών στοιχείων σε μια πολιτική του AIP, συμπεριλαμβανομένων των επιλογών όπως:</span><span class="sxs-lookup"><span data-stu-id="0a1a5-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="0a1a5-106">Επιλογή για την οποία η ετικέτα θα επιτρέπει στους διαχειριστές ή τους χρήστες να ταξινομούν και να προστατεύουν (προαιρετικά) έγγραφα και μηνύματα ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="0a1a5-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="0a1a5-107">Επιλογή για την επιβολή ταξινόμησης όταν οι χρήστες αποθηκεύουν έγγραφα και στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="0a1a5-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="0a1a5-108">Επιλογή για αυτόματη σήμανση ενός μηνύματος ηλεκτρονικού ταχυδρομείου, με βάση τα συνημμένα του.</span><span class="sxs-lookup"><span data-stu-id="0a1a5-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="0a1a5-109">Επιλογή για να ελέγξετε εάν η γραμμή προστασίας πληροφοριών εμφανίζεται στις εφαρμογές του Office</span><span class="sxs-lookup"><span data-stu-id="0a1a5-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="0a1a5-110">Για πρόσθετες επιλογές και πληροφορίες σχετικά με τις πολιτικές προστασίας πληροφοριών του Azure, ανατρέξτε στο θέμα: [Επισκόπηση της πολιτικής προστασίας πληροφοριών του Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="0a1a5-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="0a1a5-111">Για άλλους χρήσιμους πόρους σχετικά με τις πολιτικές AIP, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="0a1a5-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="0a1a5-112">Πρόγραμμα εκμάθησης: ρύθμιση των παραμέτρων πολιτικής προστασίας πληροφοριών Azure και δημιουργία νέας ετικέτας</span><span class="sxs-lookup"><span data-stu-id="0a1a5-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="0a1a5-113">Ρύθμιση παραμέτρων της πολιτικής προστασίας πληροφοριών του Azure</span><span class="sxs-lookup"><span data-stu-id="0a1a5-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="0a1a5-114">Δημιουργία και ρύθμιση παραμέτρων ετικετών ευαισθησίας και των πολιτικών τους</span><span class="sxs-lookup"><span data-stu-id="0a1a5-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="0a1a5-115">Οδηγοί οδηγιών για συνηθισμένα σενάρια που χρησιμοποιούν την προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="0a1a5-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="0a1a5-116">Αναθεώρηση τεκμηρίωσης προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="0a1a5-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="0a1a5-117">Απαιτήσεις για την προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="0a1a5-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="0a1a5-118">Πρόγραμμα εκμάθησης γρήγορης εκκίνησης για την προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="0a1a5-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="0a1a5-119">Λήψη προγράμματος-πελάτη προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="0a1a5-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)