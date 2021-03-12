---
title: Παράδειγμα πολιτικής προστασίας του Microsoft Defender για το Office 365 κατά του ηλεκτρονικού "ψαρέματος"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746853"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="ff21d-102">Παράδειγμα πολιτικής προστασίας του Microsoft Defender για το Office 365 κατά του ηλεκτρονικού "ψαρέματος"</span><span class="sxs-lookup"><span data-stu-id="ff21d-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="ff21d-103">Αυτές οι ρυθμίσεις ενεργοποιούν μια πολιτική που *ονομάζεται Τομέας και Διευθύνων Σύμβουλος.*</span><span class="sxs-lookup"><span data-stu-id="ff21d-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="ff21d-104">Αυτή η πολιτική παρέχει προστασία χρήστη και τομέα από απομίμηση και, στη συνέχεια, εφαρμόζει την πολιτική σε όλα τα μηνύματα ηλεκτρονικού ταχυδρομείου που λαμβάνονται από τους χρήστες εντός του τομέα.</span><span class="sxs-lookup"><span data-stu-id="ff21d-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="ff21d-105">Πρώτα, προσθέστε τις ακόλουθες πληροφορίες για να δημιουργήσετε την πολιτική:</span><span class="sxs-lookup"><span data-stu-id="ff21d-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="ff21d-106">**Όνομα:** Περιγραφή τομέα και **διευθύνοντος σύμβουλου:** Εξασφαλίζει ότι ο Διευθύνων Σύμβουλος και ο τομέας σας δεν μιμηθείτε.</span><span class="sxs-lookup"><span data-stu-id="ff21d-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="ff21d-107">**Εφαρμόζεται σε**: Επιλέξτε **τον τομέα παραλήπτη.**</span><span class="sxs-lookup"><span data-stu-id="ff21d-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="ff21d-108">Στην **περιοχή "Οποιοδήποτε από αυτά",** **επιλέξτε "Επιλογή"** και, στη συνέχεια, επιλέξτε έναν τομέα.</span><span class="sxs-lookup"><span data-stu-id="ff21d-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="ff21d-109">Επιλέξτε **+ Προσθήκη.**</span><span class="sxs-lookup"><span data-stu-id="ff21d-109">Select **+ Add**.</span></span> <span data-ttu-id="ff21d-110">Επιλέξτε το πλαίσιο ελέγχου δίπλα στο όνομα του τομέα στη λίστα (για παράδειγμα, contoso.com ) και, *στη* συνέχεια, επιλέξτε **"Προσθήκη".**</span><span class="sxs-lookup"><span data-stu-id="ff21d-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="ff21d-111">Επιλέξτε **"Τέλος".**</span><span class="sxs-lookup"><span data-stu-id="ff21d-111">Select **Done**.</span></span>
- <span data-ttu-id="ff21d-112">Μετά τη δημιουργία της πολιτικής, μπορείτε να ρυθμίσετε με ακρίβεια την πολιτική, χρησιμοποιώντας τις ακόλουθες επιλογές:</span><span class="sxs-lookup"><span data-stu-id="ff21d-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="ff21d-113">**Προσθήκη χρηστών για προστασία:** Για αυτό το παράδειγμα, προσθέστε τουλάχιστον τη διεύθυνση ηλεκτρονικού ταχυδρομείου του διευθύνοντος σύμβουλου.</span><span class="sxs-lookup"><span data-stu-id="ff21d-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="ff21d-114">**Προσθέστε τομείς για προστασία:** Προσθέστε τον εταιρικό τομέα που περιλαμβάνει το γραφείο του Διευθύνοντος Σύμβουλου.</span><span class="sxs-lookup"><span data-stu-id="ff21d-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="ff21d-115">**Επιλέξτε ενέργειες:** Για την περίπτωση αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου από έναν απρόσωπο **χρήστη,** επιλέξτε "Ανακατεύθυνση μηνύματος σε άλλη διεύθυνση ηλεκτρονικού ταχυδρομείου" **και,** στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του διαχειριστή ασφαλείας (για παράδειγμα, *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="ff21d-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="ff21d-116">Για **την περίπτωση αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου από έναν τομέα απομίμησης,** επιλέξτε **"Καραντίνα" του μηνύματος.**</span><span class="sxs-lookup"><span data-stu-id="ff21d-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="ff21d-117">**Ευφυΐα** γραμματοκιβωτίου: Από προεπιλογή, αυτή η επιλογή είναι ενεργοποιημένη όταν δημιουργείτε μια νέα πολιτική προστασίας από το ηλεκτρονικό "ψάρεμα".</span><span class="sxs-lookup"><span data-stu-id="ff21d-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="ff21d-118">Αφήστε αυτήν τη ρύθμιση **σε αυτήν την** επιλογή για καλύτερα αποτελέσματα.</span><span class="sxs-lookup"><span data-stu-id="ff21d-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="ff21d-119">**Προσθήκη αξιόπιστων αποστολέων και τομέων:** Για αυτό το παράδειγμα, μην ορίσετε παρακάμψεις.</span><span class="sxs-lookup"><span data-stu-id="ff21d-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="ff21d-120">Αφού εξετάσετε τις ρυθμίσεις σας, επιλέξτε "Δημιουργία αυτής **της πολιτικής" ή** **"Αποθήκευση",** ανάλογα με την περίπτωση.</span><span class="sxs-lookup"><span data-stu-id="ff21d-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="ff21d-121">Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα Πολιτικές προστασίας από το ηλεκτρονικό "ψάρεμα" στο Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="ff21d-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
