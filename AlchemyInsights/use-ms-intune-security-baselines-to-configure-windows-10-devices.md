---
title: Χρήση των γραμμών βάσης ασφαλείας του Microsoft Intune για τη ρύθμιση παραμέτρων των συσκευών Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573399"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="bacb5-102">Χρήση των γραμμών βάσης ασφαλείας του Microsoft Intune για τη ρύθμιση παραμέτρων των συσκευών Windows 10</span><span class="sxs-lookup"><span data-stu-id="bacb5-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="bacb5-103">Οι γραμμές βάσης ασφαλείας Intune συμβάλλουν στην προστασία των χρηστών και των συσκευών.</span><span class="sxs-lookup"><span data-stu-id="bacb5-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="bacb5-104">Οι γραμμές βάσης ασφαλείας είναι οι προρυθμισμένες ομάδες των ρυθμίσεων των Windows που χρησιμοποιούνται για την εφαρμογή μιας γνωστής ομάδας ρυθμίσεων και προεπιλεγμένων τιμών που συνιστώνται από τις αντίστοιχες ομάδες ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="bacb5-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="bacb5-105">Δημιουργώντας ένα προφίλ γραμμής βάσης ασφαλείας στο Intune, δημιουργείτε ένα πρότυπο που αποτελείται από πολλά προφίλ ρύθμισης παραμέτρων συσκευής.</span><span class="sxs-lookup"><span data-stu-id="bacb5-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="bacb5-106">Όταν αναπτύσσετε γραμμές βάσης ασφαλείας σε ομάδες χρηστών ή συσκευών, οι ρυθμίσεις εφαρμόζονται σε συσκευές που εκτελούνται σε Windows 10 ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="bacb5-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="bacb5-107">Για παράδειγμα, η γραμμή βάσης ασφαλείας MDM αυτόματα (1) ενεργοποιεί το BitLocker για αφαιρούμενες μονάδες δίσκου, (2) απαιτεί τον κωδικό πρόσβασης για το ξεκλείδωμα μιας συσκευής και (3) απενεργοποιεί τον βασικό έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="bacb5-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="bacb5-108">Όταν μια προεπιλεγμένη τιμή δεν λειτουργεί για το περιβάλλον σας, προσαρμόστε τη γραμμή βάσης για να εφαρμόσετε τις ρυθμίσεις που χρειάζεστε.</span><span class="sxs-lookup"><span data-stu-id="bacb5-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="bacb5-109">Οι γραμμές βάσης ασφαλείας συμβάλλουν επίσης στη δημιουργία μιας ασφαλούς ροής εργασίας από τερματικό σε τερματικό στο Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bacb5-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="bacb5-110">Τα παρακάτω είναι ορισμένα πλεονεκτήματα:</span><span class="sxs-lookup"><span data-stu-id="bacb5-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="bacb5-111">Μια γραμμή βάσης ασφαλείας περιλαμβάνει τις βέλτιστες πρακτικές και συστάσεις για τις ρυθμίσεις που επηρεάζουν την ασφάλεια.</span><span class="sxs-lookup"><span data-stu-id="bacb5-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="bacb5-112">Επειδή οι συνεργάτες του Intune με την ομάδα ασφαλείας των Windows που δημιουργούν γραμμές βάσης για τις πολιτικές ομάδας, αυτές οι συστάσεις βασίζονται σε σταθερή καθοδήγηση και εκτεταμένη εμπειρία.</span><span class="sxs-lookup"><span data-stu-id="bacb5-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="bacb5-113">Εάν δεν είστε εξοικειωμένοι με το Intune και δεν είστε βέβαιοι από πού να ξεκινήσετε, τότε οι γραμμές βάσης ασφαλείας θα σας βοηθήσουν να δημιουργήσετε και να αναπτύξετε γρήγορα ένα ασφαλές προφίλ.</span><span class="sxs-lookup"><span data-stu-id="bacb5-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="bacb5-114">Εάν χρησιμοποιείτε μια πολιτική ομάδας και, στη συνέχεια, η μετεγκατάσταση σε Windows Intune για λόγους διαχείρισης είναι πολύ πιο εύκολη με τις γραμμές βάσης ασφαλείας, επειδή είναι ενσωματωμένες στο Intune και περιλαμβάνουν δυνατότητες αιχμής για τη διαχείριση.</span><span class="sxs-lookup"><span data-stu-id="bacb5-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="bacb5-115">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα [γραμμές βάσης ασφαλείας των Windows](https://go.microsoft.com/fwlink/?linkid=2141503) και [διαχείριση κινητών συσκευών](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="bacb5-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>