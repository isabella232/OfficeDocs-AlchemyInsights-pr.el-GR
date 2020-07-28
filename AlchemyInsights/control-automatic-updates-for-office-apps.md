---
title: Έλεγχος αυτόματων ενημερώσεων για εφαρμογές του Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439330"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="2c060-102">Έλεγχος αυτόματων ενημερώσεων για εφαρμογές του Office</span><span class="sxs-lookup"><span data-stu-id="2c060-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="2c060-103">Από προεπιλογή, οι ενημερώσεις για το Office Apps λαμβάνονται αυτόματα και εφαρμόζονται στο παρασκήνιο χωρίς καμία παρέμβαση του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="2c060-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="2c060-104">Ωστόσο, οι διαχειριστές μπορούν να ελέγχουν τον τρόπο εφαρμογής των ενημερώσεων χρησιμοποιώντας τις ρυθμίσεις του Office Update.</span><span class="sxs-lookup"><span data-stu-id="2c060-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="2c060-105">Οι ρυθμίσεις ενημέρωσης επιτρέπουν στους διαχειριστές να ενεργοποιούν ή να απενεργοποιούν τις αυτόματες ενημερώσεις, να εμφανίζουν ή να αποκρύπτουν το κουμπί **Άμεση ενημέρωση** στο Office, να ορίσουν προθεσμίες ενημέρωσης και πολλά άλλα.</span><span class="sxs-lookup"><span data-stu-id="2c060-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="2c060-106">Για λεπτομερείς πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="2c060-106">For detailed information, see:</span></span>

- [<span data-ttu-id="2c060-107">Ρύθμιση παραμέτρων ενημέρωσης για το Office</span><span class="sxs-lookup"><span data-stu-id="2c060-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="2c060-108">Η αυτόματη ενημέρωση για το Office δεν είναι ενεργοποιημένη</span><span class="sxs-lookup"><span data-stu-id="2c060-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="2c060-109">Ορισμός του τρόπου ενημέρωσης του Office μετά την εγκατάστασή του</span><span class="sxs-lookup"><span data-stu-id="2c060-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="2c060-110">Για να εξετάσετε τις υπάρχουσες ρυθμίσεις ενημερωμένων εκδόσεων που εφαρμόζονται σε έναν υπολογιστή-πελάτη, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="2c060-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="2c060-111">Ανοίξτε τον Επεξεργαστή Μητρώου (Registry Editor) **μεταβαίνοντας στην επιλογή Έναρξη**  >  **Run**  >  **εκτέλεσης του regedit**.</span><span class="sxs-lookup"><span data-stu-id="2c060-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="2c060-112">Μεταβείτε στην ακόλουθη θέση και εξετάστε τις ρυθμίσεις του Office Update:</span><span class="sxs-lookup"><span data-stu-id="2c060-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="2c060-113">a.</span><span class="sxs-lookup"><span data-stu-id="2c060-113">a.</span></span> <span data-ttu-id="2c060-114">HKEY_LOCAL_MACHINE\ΛΟΓΙΣΜΙΚΟ\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="2c060-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="2c060-115">b.</span><span class="sxs-lookup"><span data-stu-id="2c060-115">b.</span></span> <span data-ttu-id="2c060-116">Κάντε κλικ στο κουμπί Για να κάνετε\ρύθμιση παραμέτρων</span><span class="sxs-lookup"><span data-stu-id="2c060-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="2c060-117">**Σημείωση**  Εάν έχει οριστεί το κλειδί OfficeMgmtCOM, ενδέχεται να εμφανιστεί το μήνυμα "Η διαχείριση των ενημερωμένων εκδόσεων γίνεται από το διαχειριστή του συστήματός σας" **στις**  >  **Account**  >  **Ενημερωμένες εκδόσεις του Office**Account Office .</span><span class="sxs-lookup"><span data-stu-id="2c060-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="2c060-118">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση ενημερώσεων σε εφαρμογές του Microsoft 365 με τη Διαχείριση ρύθμισης παραμέτρων τελικού σημείου της Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="2c060-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  