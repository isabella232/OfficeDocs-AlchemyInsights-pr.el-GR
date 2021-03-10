---
title: Χρήση των γραμμών βάσης ασφαλείας του Microsoft Intune για τη ρύθμιση παραμέτρων συσκευών με Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694431"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="86b1a-102">Χρήση των γραμμών βάσης ασφαλείας του Microsoft Intune για τη ρύθμιση παραμέτρων συσκευών με Windows 10</span><span class="sxs-lookup"><span data-stu-id="86b1a-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="86b1a-103">Οι γραμμές βάσης ασφαλείας Intune βοηθούν στην προστασία χρηστών και συσκευών.</span><span class="sxs-lookup"><span data-stu-id="86b1a-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="86b1a-104">Οι γραμμές βάσης ασφαλείας είναι προκαθορισμένες ομάδες των ρυθμίσεων των Windows που χρησιμοποιούνται για την εφαρμογή μιας γνωστής ομάδας ρυθμίσεων και προεπιλεγμένων τιμών που συνιστώνται από τις σχετικές ομάδες ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="86b1a-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="86b1a-105">Με τη δημιουργία ενός προφίλ γραμμής βάσης ασφαλείας στο Intune, μπορείτε να δημιουργήσετε ένα πρότυπο που αποτελείται από πολλά προφίλ ρύθμισης παραμέτρων συσκευής.</span><span class="sxs-lookup"><span data-stu-id="86b1a-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="86b1a-106">Όταν αναπτύσσετε γραμμές βάσης ασφαλείας σε ομάδες χρηστών ή συσκευών, οι ρυθμίσεις εφαρμόζονται σε συσκευές που εκτελούνται στα Windows 10 ή σε νεότερες εκδόσεις.</span><span class="sxs-lookup"><span data-stu-id="86b1a-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="86b1a-107">Για παράδειγμα, η γραμμή βάσης ασφαλείας της Διαχείρισης κινητών συσκευών (MDM) της Microsoft ενεργοποιεί αυτόματα (1) το BitLocker για αφαιρούμενες μονάδες δίσκου, (2) απαιτεί τον κωδικό πρόσβασης για το ξεκλείδωμα μιας συσκευής και (3) απενεργοποιεί τον βασικό έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="86b1a-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="86b1a-108">Όταν μια προεπιλεγμένη τιμή δεν λειτουργεί στο περιβάλλον σας, μπορείτε να προσαρμόσετε τη γραμμή βάσης για να εφαρμόσετε τις ρυθμίσεις που χρειάζεστε.</span><span class="sxs-lookup"><span data-stu-id="86b1a-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="86b1a-109">Οι γραμμές βάσης ασφαλείας βοηθούν επίσης στη δημιουργία μιας ασφαλούς ροής εργασίας από άκρο σε άκρο στο Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="86b1a-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="86b1a-110">Ακολουθούν ορισμένα πλεονεκτήματα αυτής της λειτουργικότητας:</span><span class="sxs-lookup"><span data-stu-id="86b1a-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="86b1a-111">Μια γραμμή βάσης ασφαλείας περιλαμβάνει τις βέλτιστες πρακτικές και συστάσεις για ρυθμίσεις που επηρεάζουν την ασφάλεια.</span><span class="sxs-lookup"><span data-stu-id="86b1a-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="86b1a-112">Επειδή το Intune συνεργάζεται με την ομάδα ασφαλείας των Windows που δημιουργεί γραμμές βάσης για πολιτικές ομάδας, αυτές οι συστάσεις βασίζονται σε σταθερή καθοδήγηση και εκτεταμένη εμπειρία.</span><span class="sxs-lookup"><span data-stu-id="86b1a-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="86b1a-113">Εάν δεν είστε νέοι στο Intune και δεν είστε βέβαιοι από πού να ξεκινήσετε, οι γραμμές βάσης ασφαλείας θα σας βοηθήσουν να δημιουργήσετε και να αναπτύξετε γρήγορα ένα ασφαλές προφίλ.</span><span class="sxs-lookup"><span data-stu-id="86b1a-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="86b1a-114">Εάν χρησιμοποιείτε μια πολιτική ομάδας τη συγκεκριμένη στιγμή, η μετεγκατάσταση στο Intune για σκοπούς διαχείρισης είναι πολύ πιο εύκολη με τις γραμμές βάσης ασφαλείας, επειδή αυτές οι γραμμές βάσης ασφάλειας είναι ενσωματωμένες στο Intune και περιλαμβάνουν δυνατότητες τελευταίας τεχνολογίας για διαχείριση.</span><span class="sxs-lookup"><span data-stu-id="86b1a-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="86b1a-115">Για περισσότερες πληροφορίες, ανατρέξτε στις [γραμμές βάσης ασφάλειας των Windows και](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) τη διαχείριση [κινητών συσκευών.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="86b1a-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>