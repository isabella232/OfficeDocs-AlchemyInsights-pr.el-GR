---
title: 646 Τρόπος ρύθμισης των παραμέτρων AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499670"
---
# <a name="configure-sync-features"></a><span data-ttu-id="cabe1-102">Ρυθμίσετε τις δυνατότητες συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="cabe1-102">Configure sync features</span></span>

<span data-ttu-id="cabe1-p101">Σύνδεση AD Azure περιλαμβάνει διάφορες δυνατότητες που ενεργοποιούνται από προεπιλογή ή που μπορείτε να ενεργοποιήσετε αργότερα. Ορισμένες δυνατότητες απαιτούν πρόσθετες ρυθμίσεις παραμέτρων στο συγκεκριμένο περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="cabe1-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="cabe1-p102">[Φιλτράρισμα](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) όρια τα αντικείμενα συγχρονίζονται Azure AD. Από προεπιλογή, όλες οι χρήστες, επαφές, ομάδες, και Windows 10 λογαριασμούς υπολογιστών συγχρονίζονται. Μπορείτε να συμπεριλάβετε ή να εξαιρέσετε αντικείμενα που βασίζονται σε τομείς, οργανικές μονάδες ή άλλα χαρακτηριστικά.</span><span class="sxs-lookup"><span data-stu-id="cabe1-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="cabe1-p103">[Ολοκληρωθεί ο συγχρονισμός κατακερματισμού κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) συγχρονίζει το κλειδί κατακερματισμού κωδικού πρόσβασης από το Active Directory εσωτερικής εγκατάστασης Azure AD. Αυτό επιτρέπει τη Διαχείριση κωδικού πρόσβασης σε μία θέση, αλλά τον ίδιο κωδικό πρόσβασης και στα δύο εσωτερικής εγκατάστασης και σύννεφο περιβάλλοντα. Επειδή η υπηρεσία καταλόγου Active Directory είναι η αξιόπιστη πηγή, μπορείτε να χρησιμοποιήσετε τις δικές σας πολιτικές κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="cabe1-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="cabe1-111">[Αυτοεξυπηρέτησης επαναφορά του κωδικού πρόσβασης (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) επιτρέπει στους χρήστες να επαναφέρετε τους κωδικούς πρόσβασής τους στο σύννεφο κατά την εφαρμογή εξακολουθεί να σας πολιτική κωδικού πρόσβασης σε χώρους.</span><span class="sxs-lookup"><span data-stu-id="cabe1-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="cabe1-112">[Συσκευή αντιγραφής](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) επιτρέπει στις συσκευές εγγεγραμμένων στο Azure AD να συνταχθούν πίσω στο Active Directory εσωτερικής εγκατάστασης ώστε να μπορεί να χρησιμοποιηθεί για την υπό όρους πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="cabe1-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="cabe1-p104">[Αποτροπή ακούσιας διαγραφών](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) είναι ενεργοποιημένη από προεπιλογή για την αποτροπή διαγραφές πάρα πολλές ταυτόχρονες αντικειμένου (περισσότερα από 500 αντικείμενα ανά συγχρονισμού). Μπορείτε να αλλάξετε αυτήν τη ρύθμιση για τις ανάγκες της εταιρείας σας.</span><span class="sxs-lookup"><span data-stu-id="cabe1-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="cabe1-115">[Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) είναι ενεργοποιημένη από προεπιλογή για εγκαταστάσεις express και διασφαλίζει τη δική σας έκδοση του σύνδεση AD Azure είναι πάντα ενημερωμένα.</span><span class="sxs-lookup"><span data-stu-id="cabe1-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

