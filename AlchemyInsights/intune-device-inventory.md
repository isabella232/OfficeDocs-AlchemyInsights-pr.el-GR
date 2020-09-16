---
title: Απογραφή συσκευής Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667878"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="8c24e-102">Απογραφή συσκευής Intune</span><span class="sxs-lookup"><span data-stu-id="8c24e-102">Intune Device Inventory</span></span>

<span data-ttu-id="8c24e-103">Η λεπίδα Devices παρέχει στον διαχειριστή πληροφορίες για τις συσκευές που βρίσκονται υπό διαχείριση στο Intune σε βάση ανά συσκευή.</span><span class="sxs-lookup"><span data-stu-id="8c24e-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="8c24e-104">Οι πληροφορίες που εμφανίζονται περιλαμβάνουν: υλικό, ανακαλύφθηκαν εφαρμογές, κατάσταση συμμόρφωσης συσκευής και κατάσταση ρύθμισης παραμέτρων συσκευής.</span><span class="sxs-lookup"><span data-stu-id="8c24e-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="8c24e-105">Τα δεδομένα απογραφής για το υλικό και τις ανακαλυφθείσες εφαρμογές συλλέγονται σε έναν κύκλο επτά ημερών.</span><span class="sxs-lookup"><span data-stu-id="8c24e-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="8c24e-106">Οι εφαρμογές και τα συγκεκριμένα στοιχεία του υλικού που αναφέρθηκαν διαφέρουν ανάλογα με το λειτουργικό σύστημα της συσκευής και εάν η συσκευή είναι προσωπική ή εταιρική.</span><span class="sxs-lookup"><span data-stu-id="8c24e-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="8c24e-107">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα ανατρέξτε στο θέμα λεπτομέρειες συσκευής στο Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="8c24e-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="8c24e-108">**ΣΥΝΗΘΕΙΣ ΕΡΩΤΉΣΕΙΣ**</span><span class="sxs-lookup"><span data-stu-id="8c24e-108">**FAQ**</span></span>

<span data-ttu-id="8c24e-109">Ε: δεν λαμβάνω μια πλήρη λίστα απογραφής των εφαρμογών που υπάρχουν σε συσκευές Windows που έχουν εγγραφεί στο Intune.</span><span class="sxs-lookup"><span data-stu-id="8c24e-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="8c24e-110">Γιατί όχι?</span><span class="sxs-lookup"><span data-stu-id="8c24e-110">Why not?</span></span>

<span data-ttu-id="8c24e-111">Α: αυτήν τη στιγμή, μόνο οι σύγχρονες εφαρμογές παρατίθενται για υπολογιστές με Windows 10 που προσδιορίζονται ως εταιρικές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="8c24e-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="8c24e-112">Το Intune δεν συλλέγει πληροφορίες σχετικά με τις εφαρμογές Win32 που είναι εγκατεστημένες σε αυτές τις συσκευές.</span><span class="sxs-lookup"><span data-stu-id="8c24e-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="8c24e-113">Ε: Γιατί οι αριθμοί τηλεφώνου δεν συλλέγονται από όλες τις συσκευές;</span><span class="sxs-lookup"><span data-stu-id="8c24e-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="8c24e-114">Α: τα τηλέφωνα που κατηγοριοποιούνται ως εταιρικές συσκευές στο Intune δεν προσδιορίζονται με τον πλήρη αριθμό τηλεφώνου τους όταν, για παράδειγμα, εκτελείτε μια αναφορά απογραφής κινητής συσκευής.</span><span class="sxs-lookup"><span data-stu-id="8c24e-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="8c24e-115">Οι αριθμοί τηλεφώνου "μεταφορά σε εσάς" είναι πάντα μερικώς καλυμμένοι με αστερίσκους (\* \* \* \*) και εμφανίζουν μόνο τα τελευταία τέσσερα ψηφία.</span><span class="sxs-lookup"><span data-stu-id="8c24e-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>