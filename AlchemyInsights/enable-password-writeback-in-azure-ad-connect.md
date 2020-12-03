---
title: Ενεργοποίηση επανεγγραφής κωδικού στο Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560440"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="21c9c-102">Ενεργοποίηση επανεγγραφής κωδικού στο Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="21c9c-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="21c9c-103">Για την ενεργοποίηση επανεγγραφής επαναφοράς κωδικού πρόσβασης από τον χρήστη, πρώτα ενεργοποιήστε την επιλογή της επανεγγραφής στο Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="21c9c-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="21c9c-104">Από τον διακομιστή του Azure AD Connect σας, ολοκληρώστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="21c9c-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="21c9c-105">Συνδεθείτε στον διακομιστή Azure AD Connect σας και ξεκινήστε τον οδηγό ρύθμισης παραμέτρων του **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="21c9c-106">Στην **Αρχική** σελίδα, κάντε κλικ στην επιλογή **Ρύθμιση παραμέτρων**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="21c9c-107">Στη σελίδα **Πρόσθετες εργασίες**, επιλέξτε **Προσαρμογή επιλογών συγχρονισμού**, και στη συνέχεια κάντε κλικ στην επιλογή **Επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="21c9c-108">Στη σελίδα **Σύνδεση στο Azure AD**, πληκτρολογήστε τα διαπιστευτήρια καθολικού διαχειριστή του μισθωτή Azure σας, και στη συνέχεια κάντε κλικ στην επιλογή **Επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="21c9c-109">Στις σελίδες φιλτραρίσματος **Σύνδεση σε καταλόγους** και **Τομέας/OU**, κάντε κλικ στην επιλογή **Επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="21c9c-110">Στη σελίδα **Προαιρετικές δυνατότητες**, επιλέξτε το πλαίσιο δίπλα στην επιλογή **Επανεγγραφή κωδικού πρόσβασης** και κάντε κλικ στην επιλογή **Επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="21c9c-111">Στη σελίδα **Έτοιμοι για ρύθμιση παραμέτρων**, κάντε κλικ στην επιλογή **Ρύθμιση παραμέτρων** και περιμένετε να ολοκληρωθεί η διαδικασία.</span><span class="sxs-lookup"><span data-stu-id="21c9c-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="21c9c-112">Όταν δείτε το τέλος της ρύθμισης παραμέτρων, κάντε κλικ στην επιλογή **Έξοδος**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="21c9c-113">Με την επανεγγραφή κωδικού πρόσβασης ενεργοποιημένη στο Azure AD Connect, ρυθμίστε τις παραμέτρους επανεγγραφής στο Azure AD SSPR.</span><span class="sxs-lookup"><span data-stu-id="21c9c-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="21c9c-114">Για την ενεργοποίηση της επανεγγραφής κωδικού πρόσβασης στο SSPR, ολοκληρώστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="21c9c-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="21c9c-115">Συνδεθείτε στην πύλη Microsoft Azure χρησιμοποιώντας έναν λογαριασμός διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="21c9c-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="21c9c-116">Αναζητήστε και επιλέξτε το **Azure Active Directory**, κάντε κλικ στην επιλογή **Επαναφορά κωδικού πρόσβασης**, και στη συνέχεια κάντε κλικ στην επιλογή **Ενοποίηση εσωτερικής εγκατάστασης**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="21c9c-117">Ορισμός επιλογής **Επανεγγραφής κωδικών πρόσβασης στον κατάλογο εσωτερικής εγκατάστασης;** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="21c9c-118">Ορισμός επιλογής **Να επιτρέπεται στους χρήστες το ξεκλείδωμα λογαριασμών χωρίς επαναφορά κωδικού πρόσβασης;** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="21c9c-119">Όταν είστε έτοιμοι, κάντε κλικ στην **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="21c9c-119">When ready, click **Save**.</span></span>

<span data-ttu-id="21c9c-120">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Ενεργοποίηση επανεγγραφής επαναφοράς κωδικού πρόσβασης από τον χρήστη σε περιβάλλον εσωτερικής εγκατάστασης](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="21c9c-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="21c9c-121">Όταν ένας διαχειριστής επαναφέρει τον κωδικό πρόσβασης ενός χρήστη στην πύλη Microsoft Azure, εάν ο συγκεκριμένος χρήστης είναι εξωτερικός ή συγχρονίζονται οι κατακερματισμένοι κωδικοί πρόσβασης, τότε ο κωδικός πρόσβασης θα επανεγγραφεί σε εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="21c9c-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="21c9c-122">Η συγκεκριμένη λειτουργικότητα δεν υποστηρίζεται αυτή τη στιγμή από την πύλη διαχειριστή του Office.</span><span class="sxs-lookup"><span data-stu-id="21c9c-122">This functionality is currently not supported in the Office Admin portal.</span></span>