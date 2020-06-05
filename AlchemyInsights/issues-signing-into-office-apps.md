---
title: Ζητήματα που σχετίζονται με την είσοδο στο Microsoft 365 εφαρμογές
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579865"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="93e8d-102">Επιδιόρθωση του μηνύματος "Η μονάδα αξιόπιστης πλατφόρμας του υπολογιστή σας δεν λειτουργεί σωστά"</span><span class="sxs-lookup"><span data-stu-id="93e8d-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="93e8d-103">Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="93e8d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="93e8d-104">Εγκαταστήστε τις πιο πρόσφατες ενημερωμένες εκδόσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [το Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="93e8d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="93e8d-105">[Καταργήστε τις πιστοποιήσεις του Office χρησιμοποιώντας](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="93e8d-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="93e8d-106">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0.</span><span class="sxs-lookup"><span data-stu-id="93e8d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="93e8d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="93e8d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="93e8d-108">Δοκιμάστε τη [διαδικασία αποκατάστασης χρήστη](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) για να διορθώσετε αποτυχίες λειτουργικής μονάδας αξιόπιστης πλατφόρμας (TPM).</span><span class="sxs-lookup"><span data-stu-id="93e8d-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="93e8d-109">Ορίστε το EnableADAL = 0 χρησιμοποιώντας τα ακόλουθα βήματα:</span><span class="sxs-lookup"><span data-stu-id="93e8d-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="93e8d-110">Κάντε δεξί κλικ στο κουμπί "Έναρξη των Windows", επιλέξτε **"Εκτέλεση",** πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="93e8d-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="93e8d-111">Επιλέξτε **Ναι** για να επιτρέψετε στον Επεξεργαστή Μητρώου (Registry Editor) να κάνει αλλαγές στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="93e8d-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="93e8d-112">Στον Επεξεργαστή Μητρώου ( Registry Editor), προσθέστε μια τιμή DWORD του **EnableADAL** με ρύθμιση **0** κάτω από HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="93e8d-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="93e8d-113">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ζητήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση για τη δημιουργία του Office 2016 16.0.7967 στα Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="93e8d-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>