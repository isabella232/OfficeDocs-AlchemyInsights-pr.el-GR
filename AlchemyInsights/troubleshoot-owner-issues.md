---
title: Αντιμετώπιση προβλημάτων κατόχων
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901006"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="a70d7-102">Αντιμετώπιση προβλημάτων κατόχων</span><span class="sxs-lookup"><span data-stu-id="a70d7-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="a70d7-103">Για να αντιμετωπίσετε προβλήματα που σχετίζονται με τον κάτοχο, εκτελέστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="a70d7-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="a70d7-104">[Προσθήκη ή αλλαγή των διαχειριστών συνδρομής Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): οι ομάδες του Azure Active Directory (Azure AD) ανήκουν και διαχειρίζονται οι κάτοχοι της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="a70d7-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="a70d7-105">Οι κάτοχοι ομάδων μπορούν να είναι χρήστες ή αρχές υπηρεσίας και έχουν τη δυνατότητα να διαχειρίζονται την ομάδα, συμπεριλαμβανομένης της ιδιότητας μέλους.</span><span class="sxs-lookup"><span data-stu-id="a70d7-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="a70d7-106">Μόνο οι υπάρχοντες κάτοχοι ομάδας ή ομάδα-διαχειριστές μπορούν να εκχωρήσουν κατόχους ομάδας.</span><span class="sxs-lookup"><span data-stu-id="a70d7-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="a70d7-107">Οι κάτοχοι ομάδων δεν υποχρεούνται να είναι μέλη της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="a70d7-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="a70d7-108">[Προσθήκη ή αλλαγή των διαχειριστών συνδρομής Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): αυτό το άρθρο περιγράφει τον τρόπο με τον οποίο μπορείτε να προσθέσετε ή να αλλάξετε το ρόλο διαχειριστή για ένα χρήστη που χρησιμοποιεί το Azure RBAC στο πεδίο της συνδρομής.</span><span class="sxs-lookup"><span data-stu-id="a70d7-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="a70d7-109">Χρησιμοποιήστε το PowerShell για να προσθέσετε έναν κάτοχο ομάδας ή έναν κάτοχο εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="a70d7-109">Use PowerShell to add a group owner or an application owner.</span></span>
