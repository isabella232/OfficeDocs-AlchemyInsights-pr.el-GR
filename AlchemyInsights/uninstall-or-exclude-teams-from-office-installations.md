---
title: Απεγκατάσταση ή αποκλεισμός ομάδων από εγκαταστάσεις του Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 6fc5645028c9fb9df2606c0d03b67e87ae15087c
ms.sourcegitcommit: 1e5de64e34e9ba16185b3a895b3152ca61718f4b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37344238"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Απεγκατάσταση ή αποκλεισμός ομάδων από νέες ή υπάρχουσες εγκαταστάσεις του Office

Οι ομάδες της Microsoft περιλαμβάνονται τώρα ως μέρος του Office 365 ProPlus, Office 365 Business και Office για Mac.

- Χρησιμοποιήστε το [εργαλείο ανάπτυξης του Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) για να εξαιρέσετε ομάδες από νέες εγκαταστάσεις του Office.
- Για να *απεγκαταστήσετε* ομάδες από μια συσκευή που εκτελεί Windows, ανατρέξτε στο [άρθρο Κατάργηση εγκατάστασης ομάδων της Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Για να καθαρίσετε τις ομάδες της Microsoft από πολλούς υπολογιστές-στόχους ή χρήστες, ανατρέξτε στην [ανάπτυξη ομάδων της Microsoft εκκαθάριση](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Χρησιμοποιήστε την επιλογή [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) για να αποτρέψετε την αυτόματη εγκατάσταση των ομάδων της Microsoft με το Office.
- Χρησιμοποιήστε την επιλογή [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *πριν να εγκατασταθούν οι ομάδες*, για να αποτρέψετε την αυτόματη εκκίνηση των ομάδων της Microsoft μετά την εγκατάσταση.

Εάν χρησιμοποιείτε το Office για Mac, ανατρέξτε [στις εγκαταστάσεις των ομάδων της Microsoft σε Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).