---
title: Δημιουργία πολιτικών Intune και προφίλ
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 6700005
ms.openlocfilehash: 3fecad7d02b8e3148a3dd774d666fc4ed317204c
ms.sourcegitcommit: 7e2122a7e08525f628986978f396b3a138d2326d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/07/2019
ms.locfileid: "33661735"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="bb08a-102">Δημιουργία πολιτικής Intune και προφίλ</span><span class="sxs-lookup"><span data-stu-id="bb08a-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="bb08a-103">Σε Intune, μπορείτε να δημιουργήσετε πολιτικές και τα προφίλ που κάνετε διάφορα πράγματα.</span><span class="sxs-lookup"><span data-stu-id="bb08a-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="bb08a-104">**Η εγγραφή προφίλ**: προκαθορίσετε τις παραμέτρους των συσκευών σας από πλατφόρμα, ενεργοποίηση χρήστη συσχέτισης, χρησιμοποιούν έλεγχο ταυτότητας πολλών παραγόντων και πολλά άλλα.</span><span class="sxs-lookup"><span data-stu-id="bb08a-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span> 

  <span data-ttu-id="bb08a-105">[Τι είναι η συσκευή εγγραφής](https://docs.microsoft.com/intune/device-enrollment), και να δημιουργήσετε προφίλ εγγραφής για [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)και [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) έχουν καλή πόρους.</span><span class="sxs-lookup"><span data-stu-id="bb08a-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="bb08a-106">**Πολιτικές συμμόρφωσης**: Ορίστε τους κανόνες και τις ρυθμίσεις που πρέπει να ακολουθούν οι συσκευές είναι συμβατό.</span><span class="sxs-lookup"><span data-stu-id="bb08a-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="bb08a-107">Επίσης, μπορείτε να χρησιμοποιήσετε πολιτικές συμμόρφωσης για την παρακολούθηση συσκευές και να ειδοποιήσετε τους χρήστες για μη συμμόρφωση.</span><span class="sxs-lookup"><span data-stu-id="bb08a-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span> 

  <span data-ttu-id="bb08a-108">Γρήγορα αποτελέσματα με τις [πολιτικές συμμόρφωσης της συσκευής](https://docs.microsoft.com/intune/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="bb08a-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="bb08a-109">**Πολιτικές υπό όρους πρόσβασης**: Βοήθεια ασφαλής εταιρικούς πόρους, ανάλογα με τις συνθήκες που εισάγετε.</span><span class="sxs-lookup"><span data-stu-id="bb08a-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="bb08a-110">Για παράδειγμα, για συσκευές που δεν είναι συμβατή, χρησιμοποιήστε υπό όρους πρόσβασης για να περιορίσετε την πρόσβαση σε μηνύματα ηλεκτρονικού ταχυδρομείου και του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bb08a-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="bb08a-111">[Τι είναι η υπό όρους πρόσβασης](https://docs.microsoft.com/intune/conditional-access) και [Συνηθισμένοι τρόποι χρήσης υπό όρους πρόσβασης](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) είναι καλή πόροι για να ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="bb08a-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="bb08a-112">**Ρύθμιση παραμέτρων προφίλ**: Διαχείριση δυνατοτήτων και των ρυθμίσεων από συσκευές, συμπεριλαμβανομένων των ρυθμίσεων ηλεκτρονικού ταχυδρομείου, προσθέστε ένα δίκτυο WiFi, χρησιμοποιήστε ενσωματωμένα πρότυπα, δυνατότητες συσκευής ελέγχου iOS και macOS και άλλα.</span><span class="sxs-lookup"><span data-stu-id="bb08a-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span> 

  <span data-ttu-id="bb08a-113">Γρήγορα αποτελέσματα με [προφίλ ρύθμισης παραμέτρων συσκευής](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="bb08a-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="bb08a-114">Χρήσιμες συνδέσεις:</span><span class="sxs-lookup"><span data-stu-id="bb08a-114">Helpful links:</span></span>

- [<span data-ttu-id="bb08a-115">Συνήθεις ερωτήσεις, θέματα και λύσεις με πολιτικές συσκευών και προφίλ στο Intune</span><span class="sxs-lookup"><span data-stu-id="bb08a-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="bb08a-116">Αντιμετώπιση προβλημάτων σχετικά με πολιτικές και προφίλ στο Intune</span><span class="sxs-lookup"><span data-stu-id="bb08a-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
