---
title: Παράδειγμα πολιτικής του Microsoft Defender για το Office 365 κατά του ηλεκτρονικού "ψαρέματος"
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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694038"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="55f31-102">Παράδειγμα πολιτικής του Microsoft Defender για το Office 365 κατά του ηλεκτρονικού "ψαρέματος"</span><span class="sxs-lookup"><span data-stu-id="55f31-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="55f31-103">Αυτές οι ρυθμίσεις επιτρέπουν μια πολιτική που ονομάζεται *"Τομέας" και "Διευθύνων Σύμβουλος".*</span><span class="sxs-lookup"><span data-stu-id="55f31-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="55f31-104">Αυτή η πολιτική παρέχει προστασία χρήστη και τομέα από απομίμηση και, στη συνέχεια, εφαρμόζει την πολιτική σε όλα τα μηνύματα ηλεκτρονικού ταχυδρομείου που λαμβάνονται από χρήστες εντός του τομέα.</span><span class="sxs-lookup"><span data-stu-id="55f31-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="55f31-105">Πρώτα, προσθέστε τις ακόλουθες πληροφορίες για να δημιουργήσετε την πολιτική:</span><span class="sxs-lookup"><span data-stu-id="55f31-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="55f31-106">**Όνομα:** Περιγραφή τομέα και **διευθύνοντος σύμβουλου:** Εξασφαλίζει ότι ο Διευθύνων Σύμβουλος και ο τομέας σας δεν απομίμηση.</span><span class="sxs-lookup"><span data-stu-id="55f31-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="55f31-107">**Εφαρμόζεται σε:** Επιλέξτε **τον τομέα του παραλήπτη.**</span><span class="sxs-lookup"><span data-stu-id="55f31-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="55f31-108">Στην **περιοχή "Οποιοδήποτε από αυτά",** επιλέξτε **"Επιλογή"** και, στη συνέχεια, επιλέξτε έναν τομέα.</span><span class="sxs-lookup"><span data-stu-id="55f31-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="55f31-109">Επιλέξτε **+ Προσθήκη.**</span><span class="sxs-lookup"><span data-stu-id="55f31-109">Select **+ Add**.</span></span> <span data-ttu-id="55f31-110">Επιλέξτε το πλαίσιο ελέγχου δίπλα στο όνομα του τομέα στη λίστα (για παράδειγμα, *contoso.com*) και, στη συνέχεια, επιλέξτε **"Προσθήκη".**</span><span class="sxs-lookup"><span data-stu-id="55f31-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="55f31-111">Επιλέξτε **"Τέλος".**</span><span class="sxs-lookup"><span data-stu-id="55f31-111">Select **Done**.</span></span>
- <span data-ttu-id="55f31-112">Μετά τη δημιουργία της πολιτικής, μπορείτε να ρυθμίσετε με ακρίβεια την πολιτική χρησιμοποιώντας τις ακόλουθες επιλογές:</span><span class="sxs-lookup"><span data-stu-id="55f31-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="55f31-113">**Προσθέστε χρήστες για προστασία:** Για αυτό το παράδειγμα, προσθέστε τουλάχιστον τη διεύθυνση ηλεκτρονικού ταχυδρομείου του διευθύνοντος σύμβουλου.</span><span class="sxs-lookup"><span data-stu-id="55f31-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="55f31-114">**Προσθήκη τομέων για προστασία:** Προσθέστε τον εταιρικό τομέα που περιλαμβάνει το γραφείο του Διευθύνοντος Σύμβουλο.</span><span class="sxs-lookup"><span data-stu-id="55f31-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="55f31-115">**Επιλέξτε ενέργειες:** **Εάν** τα μηνύματα ηλεκτρονικού ταχυδρομείου αποστέλλονται από κάποιον απομίμηση χρήστη, επιλέξτε "Ανακατεύθυνση μηνύματος σε άλλη διεύθυνση ηλεκτρονικού ταχυδρομείου" **και,** στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του διαχειριστή ασφαλείας (για παράδειγμα, *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="55f31-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="55f31-116">Για **την περίπτωση που τα μηνύματα ηλεκτρονικού ταχυδρομείου αποστέλλονται από έναν τομέα απομίμησης,** επιλέξτε **"Καραντίνα" του μηνύματος.**</span><span class="sxs-lookup"><span data-stu-id="55f31-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="55f31-117">**Ευφυΐα** γραμματοκιβωτίου: Από προεπιλογή, αυτή η επιλογή είναι ενεργοποιημένη όταν δημιουργείτε μια νέα πολιτική καταπολέμησης του ηλεκτρονικού "ψαρέματος".</span><span class="sxs-lookup"><span data-stu-id="55f31-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="55f31-118">Αφήστε αυτήν τη ρύθμιση **στην επιλογή "Ναι"** για καλύτερα αποτελέσματα.</span><span class="sxs-lookup"><span data-stu-id="55f31-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="55f31-119">**Προσθήκη αξιόπιστων αποστολέων και τομέων:** Για αυτό το παράδειγμα, μην ορίσετε τυχόν παρακάμψεις.</span><span class="sxs-lookup"><span data-stu-id="55f31-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="55f31-120">Αφού εξετάσετε τις ρυθμίσεις σας, επιλέξτε "Δημιουργία **αυτής της πολιτικής" ή** **"Αποθήκευση",** ανάλογα με την περίπτωση.</span><span class="sxs-lookup"><span data-stu-id="55f31-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="55f31-121">Για να μάθετε περισσότερα, ανατρέξτε [στις πολιτικές προστασίας από το ηλεκτρονικό "ψάρεμα" στο Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="55f31-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
