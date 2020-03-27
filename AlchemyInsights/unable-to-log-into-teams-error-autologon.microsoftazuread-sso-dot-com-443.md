---
title: Δεν είναι δυνατή η σύνδεση στo Τεαμσ λόγω σφάλματος autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931898"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="67917-102">Δεν είναι δυνατή η σύνδεση στo Teams λόγω σφάλματος autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="67917-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="67917-103">Εάν είναι ενεργοποιημένη η ομαλή SSO ως έλεγχος ταυτότητας O365, η διεύθυνση URL "autologon.microsoftazuread-sso.com" μπορεί να χρειαστεί να προστεθεί σε τοποθεσίες intranet.</span><span class="sxs-lookup"><span data-stu-id="67917-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="67917-104">Εάν έχει προστεθεί στο παρελθόν σε αξιόπιστες τοποθεσίες και η ομαλή SSO χρησιμοποιείται, θα πρέπει να καταργηθεί από αξιόπιστες τοποθεσίες.</span><span class="sxs-lookup"><span data-stu-id="67917-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="67917-105">Ανατρέξτε στο θέμα [Λίστα ελέγχου αντιμετώπισης προβλημάτων ομαλής SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="67917-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="67917-106">Ακολουθήστε τα παρακάτω βήματα για να προσθέσετε μια διεύθυνση URL στη λίστα τοποθεσίων Intranet:</span><span class="sxs-lookup"><span data-stu-id="67917-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="67917-107">Ανοίξτε τον Internet Explorer κάνοντας κλικ στο κουμπί **Έναρξη**.</span><span class="sxs-lookup"><span data-stu-id="67917-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="67917-108">Στο πλαίσιο αναζήτησης, πληκτρολογήστε Internet Explorer και, στη συνέχεια, στη λίστα αποτελεσμάτων, κάντε κλικ στην επιλογή **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="67917-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="67917-109">Κάντε κλικ στο κουμπί **Εργαλεία** και, στη συνέχεια, κάντε κλικ στο στοιχείο **Επιλογές Internet**.</span><span class="sxs-lookup"><span data-stu-id="67917-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="67917-110">Κάντε κλικ στην καρτέλα **Ασφάλεια**.</span><span class="sxs-lookup"><span data-stu-id="67917-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="67917-111">Τώρα, κάντε κλικ στις Τοποθεσίες τοπικού intranet και, στη συνέχεια, κάντε κλικ στο κουμπί τοποθεσίες και, στη συνέχεια, στο κουμπί \*\*Για προχωρημένους.</span><span class="sxs-lookup"><span data-stu-id="67917-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="67917-112">Πληκτρολογήστε τη διεύθυνση URL της τοποθεσίας Web και κάντε κλικ στην επιλογή **Προσθήκη**.</span><span class="sxs-lookup"><span data-stu-id="67917-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="67917-113">Όταν τελειώσετε, κάντε κλικ στην επιλογή **Κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="67917-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="67917-114">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τεκμηρίωση για την ανάπτυξη ομαλής SSO για το O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (περιλαμβάνει διαδικασία που βασίζεται σε πολιτική για την προσθήκη μιας διεύθυνσης URL σε τοποθεσίες intranet στο βήμα 3).</span><span class="sxs-lookup"><span data-stu-id="67917-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
