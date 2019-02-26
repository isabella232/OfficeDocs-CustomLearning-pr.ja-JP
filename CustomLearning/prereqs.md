---
author: karuanag
ms.author: karuanag
title: インストールの前提条件
ms.date: 02/11/2019
description: カスタム学習のインストールおよびセットアップに関する決定事項と前提条件に関する情報
ms.openlocfilehash: 1a57e8fbecfbce4608c8dcb618f4fdc007467789
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989718"
---
# <a name="getting-started"></a><span data-ttu-id="711ac-103">はじめに</span><span class="sxs-lookup"><span data-stu-id="711ac-103">Getting Started</span></span>

<span data-ttu-id="711ac-p101">Office 365 のカスタム学習を使用すると、組織にオンデマンドのトレーニングソリューションを提供できます。 ここでは、展開を成功させるために必要な前提条件と決定事項について説明します。</span><span class="sxs-lookup"><span data-stu-id="711ac-p101">Custom Learning for Office 365 will allow you to provide on-demand training solutions for your organization.  Here we will discuss the pre-requisites and decisions you will need to make for a successful deployment.</span></span>

<span data-ttu-id="711ac-p102">次の手順では、Office 365 (CLO365) のカスタム学習をプロビジョニングする方法について概説します。これには、テナント環境への CLO365 コミュニケーションサイトテンプレートとカスタム学習 web パーツのインストールが含まれます。次の手順では、sharepoint online プロビジョニングサービスを使用したhttps://provisioning.sharepointpnp.com CLO365 のインストールについて説明します。既存の sharepoint online コミュニケーションサイトで使用するためにカスタム学習 web パーツのみをインストールすることに関心がある場合は、「」を参照してください。[カスタム web パーツをインストール](installwebpart.md)する手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="711ac-p102">The following instructions outline how to provision Custom Learning for Office 365 (CLO365), including the installation of the CLO365 communication site template and the Custom Learning web part, into your tenant environment. These instructions cover the installation of CLO365 via the SharePoint Online Provisioning Service at https://provisioning.sharepointpnp.com    If you are interested in installing just the Custom Learning web part for use on an existing SharePoint Online communication site, please refer to the instructions for [installing the custom webpart](installwebpart.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="711ac-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="711ac-108">Prerequisites</span></span>
 
<span data-ttu-id="711ac-109">[SharePoint Online プロビジョニングサービス](https://provisioning.sharepointpnp.com)経由で CLO365 を正常にインストールするには、次の前提条件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="711ac-109">To successfully install CLO365 via the [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com) you must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="711ac-110">CLO365 をプロビジョニングするユーザーは、インストール先のテナントのテナント管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="711ac-110">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>  
- <span data-ttu-id="711ac-p103">テナント ' App Catalog ' は、SharePoint 管理センターの [アプリ] オプション内で使用できる必要があります。現在、アプリカタログを持っていない場合は、 [SharePoint Online のドキュメント](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)を参照してこの機能を準備します。</span><span class="sxs-lookup"><span data-stu-id="711ac-p103">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center. If you do not have an app catalog currently refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to provision this feature.</span></span>  
- <span data-ttu-id="711ac-p104">CLO365 をプロビジョニングするユーザーは、インストールのターゲットテナントのアプリカタログのサイトコレクションの所有者である必要があります。CLO365 インストーラーがアプリカタログのサイトコレクションの所有者ではない場合は、[次の手順を完了](addappadmin.md)して続行します。</span><span class="sxs-lookup"><span data-stu-id="711ac-p104">The individual that will be provisioning CLO365 must be a site collection owner of the app catalog in the target tenant for install. If the CLO365 installer is not a site collection owner of the app catalog [complete these instructions](addappadmin.md) and continue.</span></span>  

### <a name="next-steps---service-decisionsservicedecisionsmd"></a><span data-ttu-id="711ac-115">次の手順-[サービスの決定](servicedecisions.md)</span><span class="sxs-lookup"><span data-stu-id="711ac-115">Next Steps - [Service Decisions](servicedecisions.md)</span></span>
