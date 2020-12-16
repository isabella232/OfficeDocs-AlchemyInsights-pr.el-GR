---
title: Μεταφορά υπηρεσιών-μετακίνηση όλων των υπηρεσιών RDFE σε άλλη συνδρομή
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692043"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="3058e-102">Μεταφορά υπηρεσιών-μετακίνηση όλων των υπηρεσιών RDFE σε άλλη συνδρομή</span><span class="sxs-lookup"><span data-stu-id="3058e-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="3058e-103">**Μετακίνηση πόρων**</span><span class="sxs-lookup"><span data-stu-id="3058e-103">**Move resources**</span></span>

<span data-ttu-id="3058e-104">Οι πόροι Azure μπορούν να μετακινηθούν είτε σε μια άλλη συνδρομή Azure είτε στην ομάδα πόρων κάτω από την ίδια συνδρομή με τη χρήση της πύλης Azure, του Azure PowerShell, του Azure CLI ή του API REST για τη μετακίνηση πόρων.</span><span class="sxs-lookup"><span data-stu-id="3058e-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="3058e-105">Για να μπορέσετε να μετακινήσετε πόρους, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="3058e-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="3058e-106">Λίστα ελέγχου πριν από τη μετακίνηση πόρων</span><span class="sxs-lookup"><span data-stu-id="3058e-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="3058e-107">Υπηρεσίες που μπορούν να μετακινηθούν</span><span class="sxs-lookup"><span data-stu-id="3058e-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3058e-108">Πώς να επικυρώσετε την κίνηση</span><span class="sxs-lookup"><span data-stu-id="3058e-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="3058e-109">Μετακίνηση οδηγιών για τις υπηρεσίες</span><span class="sxs-lookup"><span data-stu-id="3058e-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="3058e-110">Για να μετακινήσετε υπάρχοντες πόρους σε μια άλλη ομάδα πόρων ή συνδρομή, μπορείτε να χρησιμοποιήσετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="3058e-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="3058e-111">Πύλη Azure</span><span class="sxs-lookup"><span data-stu-id="3058e-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="3058e-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3058e-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="3058e-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="3058e-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="3058e-114">REST API</span><span class="sxs-lookup"><span data-stu-id="3058e-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="3058e-115">Πρόγραμμα εκμάθησης: [Μετακίνηση των πόρων Azure σε άλλη ομάδα πόρων ή συνδρομή](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="3058e-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="3058e-116">**Αντιμετώπιση σφαλμάτων με τη διαχείριση πόρων του Azure**</span><span class="sxs-lookup"><span data-stu-id="3058e-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="3058e-117">Ανατρέξτε στα παρακάτω άρθρα για να μάθετε περισσότερα σχετικά με ορισμένα συνηθισμένα σφάλματα ανάπτυξης του Azure και να λάβετε πληροφορίες για να τα επιλύσετε.</span><span class="sxs-lookup"><span data-stu-id="3058e-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="3058e-118">Εάν δεν μπορείτε να βρείτε τον κωδικό σφάλματος για το σφάλμα ανάπτυξης, ανατρέξτε στο θέμα [Εύρεση κωδικού σφάλματος](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="3058e-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="3058e-119">Αντιμετώπιση σφαλμάτων ανάπτυξης</span><span class="sxs-lookup"><span data-stu-id="3058e-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="3058e-120">Αντιμετώπιση προβλημάτων μετακίνησης πόρων Azure σε νέα ομάδα πόρων ή συνδρομή</span><span class="sxs-lookup"><span data-stu-id="3058e-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="3058e-121">Λάβετε υπόψη ότι, εάν θέλετε να αναβαθμίσετε τη συνδρομή σας στο Azure, όπως η μετάβαση από τη δυνατότητα "δωρεάν" σε "Pay-as-you-Go", θα χρειαστεί να μετατρέψετε τη συνδρομή σας.</span><span class="sxs-lookup"><span data-stu-id="3058e-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="3058e-122">Για να αναβαθμίσετε μια δωρεάν δοκιμαστική έκδοση, ανατρέξτε στο θέμα [αναβάθμιση της δωρεάν δοκιμαστικής έκδοσης ή της συνδρομής σας στο Microsoft φανταστούμε ότι θα πληρώσετε-as-you-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="3058e-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="3058e-123">Για να αλλάξετε ένα λογαριασμό Pay-as-you-Go, ανατρέξτε [στο θέμα Αλλαγή της συνδρομής σας με τη συνδρομή Azure Pay-as-you-Go σε διαφορετική προσφορά](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="3058e-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="3058e-124">**Για να προσθέσετε ή να συσχετίσετε μια συνδρομή Azure στο μισθωτή του Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="3058e-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="3058e-125">Πραγματοποιήστε είσοδο και επιλέξτε τη συνδρομή που θέλετε να χρησιμοποιήσετε από τη [σελίδα "συνδρομές" στην πύλη Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="3058e-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="3058e-126">Επιλέξτε **αλλαγή καταλόγου**.</span><span class="sxs-lookup"><span data-stu-id="3058e-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="3058e-127">Εξετάστε τυχόν προειδοποιήσεις που εμφανίζονται και, στη συνέχεια, επιλέξτε **Αλλαγή**.</span><span class="sxs-lookup"><span data-stu-id="3058e-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="3058e-128">Ο κατάλογος έχει αλλάξει για τη συνδρομή και θα λάβετε ένα μήνυμα επιτυχίας.</span><span class="sxs-lookup"><span data-stu-id="3058e-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="3058e-129">Χρησιμοποιήστε την εναλλαγή *καταλόγων* για να μεταβείτε στον νέο σας κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="3058e-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="3058e-130">Μπορεί να χρειαστούν έως και 10 λεπτά για να εμφανιστούν όλα τα στοιχεία σωστά.</span><span class="sxs-lookup"><span data-stu-id="3058e-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="3058e-131">**Προτεινόμενα έγγραφα**</span><span class="sxs-lookup"><span data-stu-id="3058e-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="3058e-132">Μεταφορά της κυριότητας μιας συνδρομής Azure</span><span class="sxs-lookup"><span data-stu-id="3058e-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="3058e-133">Μετακίνηση πόρων σε νέα ομάδα πόρων ή συνδρομή</span><span class="sxs-lookup"><span data-stu-id="3058e-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="3058e-134">Διαχείριση πόρων με χρήση της πύλης Azure</span><span class="sxs-lookup"><span data-stu-id="3058e-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
