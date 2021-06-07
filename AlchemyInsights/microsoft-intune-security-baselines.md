---
title: Χρήση Microsoft Intune γραμμών βάσης ασφαλείας για τη ρύθμιση Windows 10 συσκευών
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793697"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="bcc02-102">Χρήση Microsoft Intune γραμμών βάσης ασφαλείας για τη ρύθμιση Windows 10 συσκευών</span><span class="sxs-lookup"><span data-stu-id="bcc02-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="bcc02-103">Οι γραμμές βάσης ασφαλείας intune βοηθούν στην προστασία χρηστών και συσκευών.</span><span class="sxs-lookup"><span data-stu-id="bcc02-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="bcc02-104">Οι γραμμές βάσης ασφαλείας Windows προκαθορισμένες ρυθμίσεις που χρησιμοποιούνται για την εφαρμογή μιας γνωστής ομάδας ρυθμίσεων και προεπιλεγμένων τιμών που συνιστώνται από τις σχετικές ομάδες ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="bcc02-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="bcc02-105">Με τη δημιουργία ενός προφίλ γραμμής βάσης ασφαλείας στο Intune, δημιουργείτε ένα πρότυπο που αποτελείται από πολλά προφίλ ρύθμισης παραμέτρων συσκευής.</span><span class="sxs-lookup"><span data-stu-id="bcc02-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="bcc02-106">Όταν αναπτύσσετε γραμμές βάσης ασφαλείας σε ομάδες χρηστών ή συσκευών, οι ρυθμίσεις εφαρμόζονται σε συσκευές που εκτελούνται σε Windows 10 ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="bcc02-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="bcc02-107">Για παράδειγμα, η γραμμή βάσης ασφαλείας της Διαχείρισης κινητών συσκευών της Microsoft (MDM) ενεργοποιεί αυτόματα το BitLocker για αφαιρούμενες μονάδες δίσκου, απαιτεί τον κωδικό πρόσβασης για το ξεκλείδωμα μιας συσκευής και απενεργοποιεί τον βασικό έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="bcc02-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="bcc02-108">Όταν μια προεπιλεγμένη τιμή δεν λειτουργεί για το περιβάλλον σας, μπορείτε να προσαρμόσετε τη γραμμή βάσης για να εφαρμόσετε τις ρυθμίσεις που χρειάζεστε.</span><span class="sxs-lookup"><span data-stu-id="bcc02-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="bcc02-109">Οι γραμμές βάσης ασφαλείας βοηθούν επίσης στη δημιουργία μιας ασφαλούς ροής εργασίας από άκρο σε άκρο Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bcc02-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="bcc02-110">Μια γραμμή βάσης ασφαλείας περιλαμβάνει τις βέλτιστες πρακτικές και συστάσεις για ρυθμίσεις που επηρεάζουν την ασφάλεια.</span><span class="sxs-lookup"><span data-stu-id="bcc02-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="bcc02-111">Το Intune συνεργάζεται με την Windows ασφαλείας που δημιουργεί γραμμές βάσης για τις πολιτικές ομάδας, επομένως αυτές οι συστάσεις βασίζονται σε συμπαγείς οδηγίες και εκτεταμένη εμπειρία.</span><span class="sxs-lookup"><span data-stu-id="bcc02-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="bcc02-112">Εάν είστε νέος στο Intune και δεν είστε βέβαιοι από πού να ξεκινήσετε, οι γραμμές βάσης ασφαλείας σας βοηθούν να δημιουργήσετε και να αναπτύξετε γρήγορα ένα ασφαλές προφίλ.</span><span class="sxs-lookup"><span data-stu-id="bcc02-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="bcc02-113">Εάν χρησιμοποιείτε αυτήν τη στιγμή μια πολιτική ομάδας, η μετεγκατάσταση στο Intune για σκοπούς διαχείρισης είναι πολύ πιο εύκολη με τις γραμμές βάσης ασφαλείας, επειδή είναι ενσωματωμένες στο Intune και περιλαμβάνουν δυνατότητες διαχείρισης αιχμής.</span><span class="sxs-lookup"><span data-stu-id="bcc02-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="bcc02-114">Για να μάθετε περισσότερα, ανατρέξτε [Windows γραμμές βάσης ασφαλείας και](/windows/security/threat-protection/windows-security-baselines) διαχείριση [κινητών συσκευών.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="bcc02-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

