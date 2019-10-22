---
author: pkrebs
ms.author: pkrebs
title: 概要
ms.date: 02/18/2019
description: Microsoft 365 学習経路の概要
ms.openlocfilehash: 74fac090177ad8009155e21a977b05ee2b742b3b
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247854"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="b3c77-103">学習環境をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="b3c77-103">Customize the learning experience</span></span>

<span data-ttu-id="b3c77-104">Microsoft 365 learning の方法を紹介します。 Microsoft の新しいソリューションでは、組織内での Office 365 の使用と導入を高速化するために設計されています。</span><span class="sxs-lookup"><span data-stu-id="b3c77-104">Introducing Microsoft 365 learning pathways, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="b3c77-105">ラーニング pathwyas を使用すると、次のことができます。</span><span class="sxs-lookup"><span data-stu-id="b3c77-105">With learning pathwyas, you can:</span></span>
- <span data-ttu-id="b3c77-106">ご使用の環境に合わせて Microsoft 365 learning と導入のコンテンツを調整する</span><span class="sxs-lookup"><span data-stu-id="b3c77-106">Tailor Microsoft 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="b3c77-107">組織でサポートされているサービスまたは機能を反映するためにコンテンツを表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="b3c77-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="b3c77-108">コンテンツとユーザーを最新の状態にして、Microsoft からの学習コンテンツを最新の状態に保つ</span><span class="sxs-lookup"><span data-stu-id="b3c77-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="b3c77-109">ユーザーのニーズに特化したカスタムの再生リストとカテゴリを作成する</span><span class="sxs-lookup"><span data-stu-id="b3c77-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="how-does-learning-pathways-work"></a><span data-ttu-id="b3c77-111">ラーニング経路のしくみ</span><span class="sxs-lookup"><span data-stu-id="b3c77-111">How does learning pathways work?</span></span>

<span data-ttu-id="b3c77-112">Office 365 の学習経路 (短い方の学習経路) は、次の3つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="b3c77-112">learning pathways for Office 365 (learning pathways for short) consists of three parts:</span></span> 
1. <span data-ttu-id="b3c77-113">Microsoft online カタログからのコンテンツのライブフィード</span><span class="sxs-lookup"><span data-stu-id="b3c77-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="b3c77-114">SharePoint コミュニケーションサイト</span><span class="sxs-lookup"><span data-stu-id="b3c77-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="b3c77-115">SharePoint web パーツ</span><span class="sxs-lookup"><span data-stu-id="b3c77-115">a SharePoint web part</span></span> 

![cg-howitworks](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="b3c77-117">要件とアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3c77-117">Requirements and Permissions</span></span>

<span data-ttu-id="b3c77-118">このガイドを開始する前に、学習経路が SharePoint テナント管理者によって設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b3c77-118">Before getting started with this guide, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="b3c77-119">設定されているかどうかがわからない場合は、SharePoint テナント管理者に連絡して、学習経路が準備されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b3c77-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="b3c77-120">また、ラーニングパス SharePoint サイトの URL を取得するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="b3c77-120">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="b3c77-121">テナント管理者とラーニング経路がプロビジョニングされていない場合は、「[学習経路のプロビジョニング](custom_provision.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3c77-121">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="b3c77-122">学習経路をプロビジョニングするためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3c77-122">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="b3c77-123">テナント管理者 (Office 365 全体管理者とも呼ばれる)</span><span class="sxs-lookup"><span data-stu-id="b3c77-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="b3c77-124">サイトでの所有者権限を持つ SharePoint サイトコレクション管理者</span><span class="sxs-lookup"><span data-stu-id="b3c77-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="b3c77-125">学習経路管理機能を使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3c77-125">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="b3c77-126">サイト コレクションの管理者</span><span class="sxs-lookup"><span data-stu-id="b3c77-126">Site Collection Administrator</span></span>
- <span data-ttu-id="b3c77-127">SharePoint 所有者またはメンバーのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3c77-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="b3c77-128">ユーザーとしてラーニングパスサイトを使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3c77-128">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="b3c77-129">Office 365 のユーザー権限/SharePoint サイト訪問者のアクセス許可またはそれ以上</span><span class="sxs-lookup"><span data-stu-id="b3c77-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="b3c77-130">カスタマイズの概要</span><span class="sxs-lookup"><span data-stu-id="b3c77-130">Get started with customization</span></span>
<span data-ttu-id="b3c77-131">サイトと web パーツをカスタマイズするために必要なアクセス許可があることを確認したら、カスタマイズプロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="b3c77-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="b3c77-132">開始するには、「[ラーニングパスサイトに移動する](custom_goto.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3c77-132">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>