---
title: Δημιουργία πολιτικών ετικετών AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569201"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="85f6f-102">Δημιουργία πολιτικών ετικετών AIP</span><span class="sxs-lookup"><span data-stu-id="85f6f-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="85f6f-103">Οι ετικέτες Προστασίας Πληροφοριών Azure (AIP) μπορούν να χρησιμοποιηθούν με το πλήρες φάσμα δεδομένων που δημιουργεί και αποθηκεύει συνήθως ένας οργανισμός, από τη χαμηλότερη ταξινόμηση προσωπικών δεδομένων, έως την υψηλότερη ταξινόμηση άκρως εμπιστευτικών δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="85f6f-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="85f6f-104">Οι πολιτικές προστασίας πληροφοριών Azure εφαρμόζονται στο κλασικό πρόγραμμα-πελάτη Προστασίας πληροφοριών Azure (AIP) και όχι στον [υπολογιστή-πελάτη ενοποιημένης επισήμανσης AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="85f6f-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="85f6f-105">Μπορείτε να ρυθμίσετε τις παραμέτρους πολλών στοιχείων σε μια πολιτική AIP, συμπεριλαμβανομένων επιλογών όπως:</span><span class="sxs-lookup"><span data-stu-id="85f6f-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="85f6f-106">Επιλογή για την οποία η ετικέτα θα επιτρέπει στους διαχειριστές ή στο χρήστη να ταξινομούν και να προφυλάσσουν (προαιρετικά) έγγραφα και μηνύματα ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="85f6f-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="85f6f-107">Επιλογή επιβολής ταξινόμησης όταν οι χρήστες αποθηκεύουν έγγραφα και στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="85f6f-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="85f6f-108">Επιλογή αυτόματης επισήμανσης ενός μηνύματος ηλεκτρονικού ταχυδρομείου, με βάση τα συνημμένα του.</span><span class="sxs-lookup"><span data-stu-id="85f6f-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="85f6f-109">Δυνατότητα ελέγχου εάν η γραμμή "Προστασία πληροφοριών" εμφανίζεται στις εφαρμογές του Office</span><span class="sxs-lookup"><span data-stu-id="85f6f-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="85f6f-110">Για πρόσθετες επιλογές και πληροφορίες σχετικά με τις πολιτικές προστασίας πληροφοριών Azure, [ανατρέξτε στο θέμα: Επισκόπηση της πολιτικής προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="85f6f-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="85f6f-111">Για άλλους χρήσιμους πόρους σχετικά με τις πολιτικές AIP, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="85f6f-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="85f6f-112">Πρόγραμμα εκμάθησης: Ρύθμιση παραμέτρων πολιτικής προστασίας πληροφοριών Azure και δημιουργία νέας ετικέτας</span><span class="sxs-lookup"><span data-stu-id="85f6f-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="85f6f-113">Ρύθμιση παραμέτρων της πολιτικής προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="85f6f-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="85f6f-114">Δημιουργία και ρύθμιση παραμέτρων ετικετών ευαισθησίας και των πολιτικών τους</span><span class="sxs-lookup"><span data-stu-id="85f6f-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="85f6f-115">Οδηγίες για κοινά σενάρια που χρησιμοποιούν την Προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="85f6f-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="85f6f-116">Αναθεώρηση της τεκμηρίωσης προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="85f6f-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="85f6f-117">Απαιτήσεις για την προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="85f6f-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="85f6f-118">Πρόγραμμα εκμάθησης γρήγορης εκκίνησης για την Προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="85f6f-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="85f6f-119">Λήψη προγράμματος-πελάτη προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="85f6f-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)