---
author: pkrebs
ms.author: pkrebs
title: 概要
ms.date: 02/18/2019
description: Office 365 の管理者向けのカスタム学習の概要
ms.openlocfilehash: 98187038b66252523c74d88dd9bfd0f217591bc5
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2019
ms.locfileid: "30087536"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="0f78c-103">学習環境をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="0f78c-103">Customize the Learning Experience</span></span>

<span data-ttu-id="0f78c-p101">office 365 のカスタム学習の概要組織内での office 365 の使用と導入を高速化するために設計された、Microsoft の新しいソリューション。カスタム学習を使用すると、次のことができます。</span><span class="sxs-lookup"><span data-stu-id="0f78c-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>
- <span data-ttu-id="0f78c-106">ご使用の環境で Office 365 learning と導入のコンテンツを調整する</span><span class="sxs-lookup"><span data-stu-id="0f78c-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="0f78c-107">組織でサポートされているサービスまたは機能を反映するためにコンテンツを表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="0f78c-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="0f78c-108">コンテンツとユーザーを最新の状態にして、Microsoft からの学習コンテンツを最新の状態に保つ</span><span class="sxs-lookup"><span data-stu-id="0f78c-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="0f78c-109">ユーザーのニーズに特化したカスタムの再生リストとカテゴリを作成する</span><span class="sxs-lookup"><span data-stu-id="0f78c-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="0f78c-111">カスタム学習のしくみ</span><span class="sxs-lookup"><span data-stu-id="0f78c-111">How does Custom Learning work?</span></span>

<span data-ttu-id="0f78c-112">カスタム学習 Office 365 (カスタム学習の省略) は、次の3つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="0f78c-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="0f78c-113">Microsoft online カタログからのコンテンツのライブフィード</span><span class="sxs-lookup"><span data-stu-id="0f78c-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="0f78c-114">SharePoint コミュニケーションサイト</span><span class="sxs-lookup"><span data-stu-id="0f78c-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="0f78c-115">SharePoint web パーツ</span><span class="sxs-lookup"><span data-stu-id="0f78c-115">a SharePoint web part</span></span> 

![cg-howitworks](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="0f78c-117">要件とアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f78c-117">Requirements and Permissions</span></span>

<span data-ttu-id="0f78c-p102">このガイドを開始する前に、SharePoint テナント管理者によってカスタム学習が設定されていることを確認してください。セットアップされているかどうかがわからない場合は、SharePoint テナント管理者に連絡して、カスタム学習がインストールされていることを確認してください。また、カスタムラーニング SharePoint サイトの URL を取得するようにしてください。テナント管理者であり、カスタム学習がインストールされていない場合は、「custom learning for Office 365 インストールガイド」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f78c-p102">Before getting started with this guide, ensure that Custom Learning has been set up by your  SharePoint tenant administrator. If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-to-install-custom-learning"></a><span data-ttu-id="0f78c-122">カスタム学習をインストールするためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f78c-122">Permissions to install Custom Learning</span></span>

- <span data-ttu-id="0f78c-123">Office 365 グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="0f78c-123">Office 365 Global Administrator</span></span>
- <span data-ttu-id="0f78c-124">SharePoint 管理者</span><span class="sxs-lookup"><span data-stu-id="0f78c-124">SharePoint Administrator</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="0f78c-125">カスタム学習管理機能を使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f78c-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="0f78c-126">Office 365 sharepoint 管理者/sharepoint サイト所有者のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f78c-126">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="0f78c-127">sharepoint サイトコレクション管理者/sharepoint サイト所有者のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f78c-127">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="0f78c-128">ユーザーとしてカスタム学習サイトを使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f78c-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="0f78c-129">Office 365 のユーザー権限/SharePoint サイト訪問者のアクセス許可またはそれ以上</span><span class="sxs-lookup"><span data-stu-id="0f78c-129">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>


