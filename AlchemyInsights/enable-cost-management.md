---
title: Ενεργοποίηση διαχείρισης κόστους
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677735"
---
# <a name="enable-cost-management"></a><span data-ttu-id="992e3-102">Ενεργοποίηση διαχείρισης κόστους</span><span class="sxs-lookup"><span data-stu-id="992e3-102">Enable cost management</span></span>

<span data-ttu-id="992e3-103">**Τι σημαίνει το κόστος είναι απενεργοποιημένο για τον οργανισμό σας;**</span><span class="sxs-lookup"><span data-stu-id="992e3-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="992e3-104">Οι εταιρείες που χρησιμοποιούν λογαριασμούς Enterprise (EA) ή σύμβαση πελατών της Microsoft (MCA) μπορούν να απενεργοποιήσουν την πρόσβαση σε πληροφορίες κόστους και πληροφορίες τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="992e3-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="992e3-105">Μετά τη σύνδεση στο Azure Portal, μπορούν να χρησιμοποιήσουν τα API χρεώσεων για να λάβουν μέσω προγραμματισμού τιμολόγια (μόλις επιλέξει) και λεπτομέρειες χρήσης.</span><span class="sxs-lookup"><span data-stu-id="992e3-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="992e3-106">**Πώς μπορείτε να επιτρέψετε σε επιπλέον χρήστες να έχουν πρόσβαση σε τιμολόγια**</span><span class="sxs-lookup"><span data-stu-id="992e3-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="992e3-107">Μεταβείτε στις **συνδρομές Blade** στην πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="992e3-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="992e3-108">Επιλέξτε **τιμολόγια** και, στη συνέχεια, **πρόσβαση σε τιμολόγια**.</span><span class="sxs-lookup"><span data-stu-id="992e3-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="992e3-109">Ενεργοποιήστε την Access και, στη συνέχεια, αποθηκεύστε τις αλλαγές, για να επιτρέψετε στους χρήστες με ρόλους εύρους συνδρομής να κάνουν λήψη τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="992e3-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="992e3-110">Ο διαχειριστής λογαριασμού μπορεί επίσης να ρυθμίσει τις παραμέτρους ώστε να αποστέλλονται τιμολόγια μέσω ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="992e3-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="992e3-111">Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα λήψη τιμολογίου μέσω ηλεκτρονικού ταχυδρομείου](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="992e3-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="992e3-112">**Πώς μπορείτε να προσθέσετε χρήστες στο ρόλο του προγράμματος ανάγνωσης χρέωσης**</span><span class="sxs-lookup"><span data-stu-id="992e3-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="992e3-113">Μεταβείτε στις **συνδρομές Blade** στην πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="992e3-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="992e3-114">Επιλέξτε **Έλεγχος πρόσβασης (IAM)** και, στη συνέχεια, κάντε κλικ στην επιλογή **Προσθήκη**.</span><span class="sxs-lookup"><span data-stu-id="992e3-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="992e3-115">Επιλέξτε " **πρόγραμμα ανάγνωσης χρεώσεων** " στη σελίδα " **επιλογή ρόλου** ".</span><span class="sxs-lookup"><span data-stu-id="992e3-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="992e3-116">Πληκτρολογήστε το μήνυμα ηλεκτρονικού ταχυδρομείου του χρήστη που θέλετε να προσκαλέσετε και, στη συνέχεια, κάντε κλικ στο κουμπί **OK** για να στείλετε την πρόσκληση.</span><span class="sxs-lookup"><span data-stu-id="992e3-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="992e3-117">Ακολουθήστε τις οδηγίες που παρέχονται στο πλαίσιο πρόσκληση ηλεκτρονικού ταχυδρομείου για να συνδεθείτε ως αναγνώστης χρεώσεων.</span><span class="sxs-lookup"><span data-stu-id="992e3-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="992e3-118">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα εκχώρηση πρόσβασης σε χρέωση](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="992e3-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="992e3-119">**Προτεινόμενα έγγραφα**</span><span class="sxs-lookup"><span data-stu-id="992e3-119">**Recommended documents**</span></span>

- [<span data-ttu-id="992e3-120">Ενεργοποίηση των προβολών DA και AO μέσω της πύλης EA</span><span class="sxs-lookup"><span data-stu-id="992e3-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="992e3-121">Κόστος που περιλαμβάνεται στη διαχείριση κόστους</span><span class="sxs-lookup"><span data-stu-id="992e3-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="992e3-122">Υποστηριζόμενες προσφορές του Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="992e3-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="992e3-123">Αναθεώρηση κόστους στην ανάλυση κόστους</span><span class="sxs-lookup"><span data-stu-id="992e3-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="992e3-124">Παροχή πρόσβασης σε πληροφορίες χρέωσης</span><span class="sxs-lookup"><span data-stu-id="992e3-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="992e3-125">Επιλέξτε πρόσβαση σε συμφωνία πελατών της Microsoft</span><span class="sxs-lookup"><span data-stu-id="992e3-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






