---
title: Η εφαρμογή μου δεν εμφανίζεται στη Διαχείριση εφαρμογών
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454699"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Η εφαρμογή μου δεν εμφανίζεται στη Διαχείριση εφαρμογών

Εάν η εφαρμογή σας δεν εμφανίζεται στη Διαχείριση εφαρμογών, ελέγξτε τα εξής:

1. Μεταβείτε [στο Azure AD](https://aad.portal.azure.com/) και βρείτε το αναγνωριστικό εφαρμογής για την εφαρμογή σας, αναζητώντας το όνομα της εφαρμογής στην επάνω γραμμή στη σελίδα "Επισκόπηση".

1. Access Graph Explorer και αναζητήστε το αναγνωριστικό εφαρμογής στην κύρια υπηρεσία σας, χρησιμοποιώντας αυτό το ερώτημα και αντικαθιστώντας με το σχετικό αναγνωριστικό <appId> εφαρμογής: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Εάν δεν επιστραφούν αποτελέσματα, αναζητήστε το αναγνωριστικό εφαρμογής μέσα στην εφαρμογή χρησιμοποιώντας αυτό το ερώτημα και αντικαθιστώντας το με το σχετικό αναγνωριστικό <appId> εφαρμογής: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Εάν αντιμετωπίζετε προβλήματα με το ερώτημα, ανατρέξτε στο θέμα [Λήψη υποστήριξης.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Για περισσότερες πληροφορίες ή πληροφορίες σχετικά με τις Εφαρμογές σας στη Διαχείριση εφαρμογών, ανατρέξτε στο θέμα [Μάθετε περισσότερα σχετικά με την ορατότητα και τις ιδέες.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Για περισσότερες πληροφορίες σχετικά με την προβολή των εφαρμογών σας, ανατρέξτε [στο θέμα Προβολή των εφαρμογών σας.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
