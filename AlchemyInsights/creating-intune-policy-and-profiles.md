---
title: Δημιουργία πολιτικών και προφίλ Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: af8f1a3dfaccaca52f187f387274d63b22631b2d
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704642"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="1d33a-102">Δημιουργία πολιτικής και προφίλ Intune</span><span class="sxs-lookup"><span data-stu-id="1d33a-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="1d33a-103">Στο Intune, μπορείτε να δημιουργήσετε πολιτικές και προφίλ που κάνουν διαφορετικά πράγματα.</span><span class="sxs-lookup"><span data-stu-id="1d33a-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="1d33a-104">**Προφίλ εγγραφής: Προδιαμορφώστε** τις συσκευές σας ανά πλατφόρμα, ενεργοποιήστε τη συνάφεια των χρηστών, χρησιμοποιήστε έλεγχο ταυτότητας πολλών παραγόντων και πολλά άλλα.</span><span class="sxs-lookup"><span data-stu-id="1d33a-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="1d33a-105">[Τι είναι η εγγραφή συσκευών](https://docs.microsoft.com/intune/device-enrollment)και η δημιουργία προφίλ εγγραφής για [Android,](https://docs.microsoft.com/intune/android-enroll) [iOS,](https://docs.microsoft.com/intune/ios-enroll) [macOS](https://docs.microsoft.com/intune/macos-enroll)και [Windows είναι](https://docs.microsoft.com/intune/windows-enrollment-methods) καλοί πόροι.</span><span class="sxs-lookup"><span data-stu-id="1d33a-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="1d33a-106">**Πολιτικές συμμόρφωσης:** Ορίστε τους κανόνες και τις ρυθμίσεις που πρέπει να ακολουθήσουν οι συσκευές για να είναι συμβατές.</span><span class="sxs-lookup"><span data-stu-id="1d33a-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="1d33a-107">Μπορείτε επίσης να χρησιμοποιήσετε πολιτικές συμμόρφωσης για την παρακολούθηση συσκευών και την ειδοποίηση των χρηστών σχετικά με τη μη συμμόρφωση.</span><span class="sxs-lookup"><span data-stu-id="1d33a-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="1d33a-108">Γρήγορα αποτελέσματα με τις [πολιτικές συμμόρφωσης συσκευών.](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="1d33a-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="1d33a-109">**Πολιτικές πρόσβασης υπό όρους:** Βοηθήστε να ασφαλίσετε τους εταιρικούς πόρους, ανάλογα με τις συνθήκες που εισάγετε.</span><span class="sxs-lookup"><span data-stu-id="1d33a-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="1d33a-110">Για παράδειγμα, για συσκευές που δεν είναι συμβατές, χρησιμοποιήστε την πρόσβαση υπό όρους για να περιορίσετε την πρόσβαση στο ηλεκτρονικό ταχυδρομείο και το SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d33a-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="1d33a-111">[Αυτό που είναι η πρόσβαση υπό](https://docs.microsoft.com/intune/conditional-access) όρους και οι [συνηθισμένοι τρόποι χρήσης της πρόσβασης υπό όρους](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) είναι καλοί πόροι για να ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="1d33a-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="1d33a-112">**Προφίλ ρύθμισης παραμέτρων:** Διαχείριση δυνατοτήτων και ρυθμίσεων σε συσκευές, συμπεριλαμβανομένων των ρυθμίσεων ηλεκτρονικού ταχυδρομείου, προσθήκη δικτύου WiFi, χρήση ενσωματωμένων προτύπων, έλεγχος δυνατοτήτων συσκευής iOS και macOS και πολλά άλλα.</span><span class="sxs-lookup"><span data-stu-id="1d33a-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="1d33a-113">Γρήγορα αποτελέσματα με τα [προφίλ ρύθμισης παραμέτρων συσκευών.](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="1d33a-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="1d33a-114">Χρήσιμες συνδέσεις:</span><span class="sxs-lookup"><span data-stu-id="1d33a-114">Helpful links:</span></span>

- [<span data-ttu-id="1d33a-115">Συνήθεις ερωτήσεις, θέματα και λύσεις με τις πολιτικές και τα προφίλ συσκευών στο Intune</span><span class="sxs-lookup"><span data-stu-id="1d33a-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="1d33a-116">Αντιμετώπιση προβλημάτων με πολιτικές και προφίλ στο Intune</span><span class="sxs-lookup"><span data-stu-id="1d33a-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)
