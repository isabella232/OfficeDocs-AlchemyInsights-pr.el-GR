---
title: 646 Τρόπος ρύθμισης παραμέτρων του AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722541"
---
# <a name="configure-sync-features"></a><span data-ttu-id="a02e0-102">Ρύθμιση παραμέτρων δυνατοτήτων συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="a02e0-102">Configure sync features</span></span>

<span data-ttu-id="a02e0-103">Το Azure AD Connect περιλαμβάνει πολλές δυνατότητες που είναι ενεργοποιημένες από προεπιλογή ή τις οποίες μπορείτε να ενεργοποιήσετε αργότερα.</span><span class="sxs-lookup"><span data-stu-id="a02e0-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="a02e0-104">Ορισμένες δυνατότητες απαιτούν πρόσθετες ρυθμίσεις παραμέτρων σε συγκεκριμένα περιβάλλοντα.</span><span class="sxs-lookup"><span data-stu-id="a02e0-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="a02e0-105">[Το φιλτράρισμα](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) περιορίζει τα αντικείμενα που συγχρονίζονται με Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a02e0-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="a02e0-106">Από προεπιλογή, συγχρονίζονται όλοι οι χρήστες, οι επαφές, οι ομάδες και οι λογαριασμοί υπολογιστών των Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a02e0-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="a02e0-107">Μπορείτε να συμπεριλάβετε ή να εξαιρέσετε αντικείμενα που βασίζονται σε τομείς, δικαιώματα οδοποιίας ή άλλα χαρακτηριστικά.</span><span class="sxs-lookup"><span data-stu-id="a02e0-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="a02e0-108">[Ο συγχρονισμός κατακερματισμού κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) συγχρονίζει τον κατακερματισμό κωδικού πρόσβασης από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης σε Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a02e0-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="a02e0-109">Αυτό επιτρέπει τη διαχείριση κωδικών πρόσβασης σε μία θέση, αλλά τη χρήση του ίδιου κωδικού πρόσβασης τόσο σε περιβάλλονεσωτερικής εγκατάστασης όσο και σε περιβάλλοντα cloud.</span><span class="sxs-lookup"><span data-stu-id="a02e0-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="a02e0-110">Επειδή η υπηρεσία καταλόγου Active Directory είναι η έγκυρη προέλευση, μπορείτε να χρησιμοποιήσετε τις δικές σας πολιτικές κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="a02e0-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="a02e0-111">[Η επαναφορά κωδικού πρόσβασης από το χρήστη (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) επιτρέπει στους χρήστες να επαναφέρουν τους δικούς τους κωδικούς πρόσβασης στο cloud, ενώ εξακολουθούν να εφαρμόζουν την πολιτική κωδικού πρόσβασης εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="a02e0-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="a02e0-112">[Η επαναφορά συσκευής](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) επιτρέπει την εγγραφή καταχωρημένων συσκευών στο Azure AD στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, ώστε να μπορούν να χρησιμοποιηθούν για πρόσβαση υπό όρους.</span><span class="sxs-lookup"><span data-stu-id="a02e0-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="a02e0-113">[Η αποτροπή τυχαίων διαγραφών](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) είναι ενεργοποιημένη από προεπιλογή για την αποτροπή πάρα πολλών ταυτόχρονων διαγραφών αντικειμένων (περισσότερα από 500 αντικείμενα ανά συγχρονισμό).</span><span class="sxs-lookup"><span data-stu-id="a02e0-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="a02e0-114">Μπορείτε να αλλάξετε αυτήν τη ρύθμιση για να ικανοποιήσετε τις ανάγκες του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="a02e0-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="a02e0-115">[Η αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) είναι ενεργοποιημένη από προεπιλογή για τις εγκαταστάσεις εξπρές και διασφαλίζει ότι η έκδοση του Azure AD Connect είναι πάντα τρέχουσα.</span><span class="sxs-lookup"><span data-stu-id="a02e0-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
