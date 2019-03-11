---
author: pkrebs
ms.author: pkrebs
title: 概要
ms.date: 02/18/2019
description: Office 365 の管理者向けのカスタム学習の概要
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523021"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="9a588-103">学習環境をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="9a588-103">Customize the Learning Experience</span></span>

<span data-ttu-id="9a588-104">office 365 のカスタム学習の概要組織内での office 365 の使用と導入を高速化するために設計された、Microsoft の新しいソリューション。</span><span class="sxs-lookup"><span data-stu-id="9a588-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="9a588-105">カスタム学習を使用すると、次のことができます。</span><span class="sxs-lookup"><span data-stu-id="9a588-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="9a588-106">ご使用の環境で Office 365 learning と導入のコンテンツを調整する</span><span class="sxs-lookup"><span data-stu-id="9a588-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="9a588-107">組織でサポートされているサービスまたは機能を反映するためにコンテンツを表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="9a588-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="9a588-108">コンテンツとユーザーを最新の状態にして、Microsoft からの学習コンテンツを最新の状態に保つ</span><span class="sxs-lookup"><span data-stu-id="9a588-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="9a588-109">ユーザーのニーズに特化したカスタムの再生リストとカテゴリを作成する</span><span class="sxs-lookup"><span data-stu-id="9a588-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="9a588-111">カスタム学習のしくみ</span><span class="sxs-lookup"><span data-stu-id="9a588-111">How does Custom Learning work?</span></span>

<span data-ttu-id="9a588-112">カスタム学習 Office 365 (カスタム学習の省略) は、次の3つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="9a588-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="9a588-113">Microsoft online カタログからのコンテンツのライブフィード</span><span class="sxs-lookup"><span data-stu-id="9a588-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="9a588-114">SharePoint コミュニケーションサイト</span><span class="sxs-lookup"><span data-stu-id="9a588-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="9a588-115">SharePoint web パーツ</span><span class="sxs-lookup"><span data-stu-id="9a588-115">a SharePoint web part</span></span> 

![cg-howitworks](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="9a588-117">要件とアクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a588-117">Requirements and Permissions</span></span>

<span data-ttu-id="9a588-118">このガイドを開始する前に、SharePoint テナント管理者によってカスタム学習が設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="9a588-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="9a588-119">セットアップされているかどうかがわからない場合は、SharePoint テナント管理者に連絡して、カスタム学習が準備されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="9a588-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="9a588-120">また、カスタムラーニング SharePoint サイトの URL を取得するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="9a588-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="9a588-121">テナント管理者であり、カスタム学習がプロビジョニングされていない場合は、「[カスタム学習のプロビジョニング](custom_provision.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a588-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="9a588-122">カスタム学習をプロビジョニングするためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a588-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="9a588-123">テナント管理者 (Office 365 全体管理者とも呼ばれる)</span><span class="sxs-lookup"><span data-stu-id="9a588-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="9a588-124">サイトでの所有者権限を持つ SharePoint サイトコレクション管理者</span><span class="sxs-lookup"><span data-stu-id="9a588-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="9a588-125">カスタム学習管理機能を使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a588-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="9a588-126">サイト コレクションの管理者</span><span class="sxs-lookup"><span data-stu-id="9a588-126">Site Collection Administrator</span></span>
- <span data-ttu-id="9a588-127">SharePoint 所有者またはメンバーのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a588-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="9a588-128">ユーザーとしてカスタム学習サイトを使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a588-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="9a588-129">Office 365 のユーザー権限/SharePoint サイト訪問者のアクセス許可またはそれ以上</span><span class="sxs-lookup"><span data-stu-id="9a588-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="9a588-130">カスタマイズの概要</span><span class="sxs-lookup"><span data-stu-id="9a588-130">Get started with customization</span></span>
<span data-ttu-id="9a588-131">サイトと web パーツをカスタマイズするために必要なアクセス許可があることを確認したら、カスタマイズプロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="9a588-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="9a588-132">開始するには、「[カスタム学習サイトに移動する](custom_goto.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a588-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>