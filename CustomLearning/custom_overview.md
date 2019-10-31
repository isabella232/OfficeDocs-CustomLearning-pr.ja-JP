---
author: pkrebs
ms.author: pkrebs
title: 学習経路をカスタマイズする
ms.date: 02/18/2019
description: 学習経路をカスタマイズする
ms.openlocfilehash: 15d782455204cf043937bec03041a85abc9e4ee3
ms.sourcegitcommit: 3b8896c81ad2adbcfdbda658482847af5fccb264
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/30/2019
ms.locfileid: "37886640"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="6846d-103">学習経路をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="6846d-103">Customize learning pathways</span></span>

<span data-ttu-id="6846d-104">Microsoft 365 learning の経路は、組織のコンテンツをカスタマイズするためのさまざまな方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="6846d-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="6846d-105">たとえば、次のようなことが可能です。</span><span class="sxs-lookup"><span data-stu-id="6846d-105">For example, you can:</span></span>  
- <span data-ttu-id="6846d-106">ラーニングパス SharePoint サイトを変更します。サイト名、ロゴ、およびそれらを変更します。</span><span class="sxs-lookup"><span data-stu-id="6846d-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="6846d-107">[質問をお寄せください] と [ヘルプを表示] ページを変更して、独自のヘルプセンターを作成します。</span><span class="sxs-lookup"><span data-stu-id="6846d-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="6846d-108">組織でサポートされているサービスまたは機能を反映するためにコンテンツを表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="6846d-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="6846d-109">ユーザーのニーズに特化したカスタムの再生リストおよびサブカテゴリを作成する</span><span class="sxs-lookup"><span data-stu-id="6846d-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="6846d-110">Microsoft Teams の導入、Outlook mobile、Microsoft 365 との共同作業の促進など、ビジネス成果をサポートするためにフィルター処理されたコンテンツを含むランディングページを作成します。</span><span class="sxs-lookup"><span data-stu-id="6846d-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="6846d-112">要件とアクセス許可</span><span class="sxs-lookup"><span data-stu-id="6846d-112">Requirements and Permissions</span></span>

<span data-ttu-id="6846d-113">「学習経路のカスタマイズ」のガイダンスを開始する前に、SharePoint テナント管理者によって学習経路が設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6846d-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="6846d-114">設定されているかどうかがわからない場合は、SharePoint テナント管理者に連絡して、学習経路が準備されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6846d-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="6846d-115">また、ラーニングパス SharePoint サイトの URL を取得するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6846d-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="6846d-116">テナント管理者とラーニング経路がプロビジョニングされていない場合は、「[学習経路のプロビジョニング](custom_provision.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6846d-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="6846d-117">学習経路をプロビジョニングするためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="6846d-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="6846d-118">テナント管理者 (Office 365 全体管理者とも呼ばれる)</span><span class="sxs-lookup"><span data-stu-id="6846d-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="6846d-119">サイトでの所有者権限を持つ SharePoint サイトコレクション管理者</span><span class="sxs-lookup"><span data-stu-id="6846d-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="6846d-120">学習経路管理機能を使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="6846d-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="6846d-121">サイト コレクションの管理者</span><span class="sxs-lookup"><span data-stu-id="6846d-121">Site Collection Administrator</span></span>
- <span data-ttu-id="6846d-122">SharePoint 所有者またはメンバーのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="6846d-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="6846d-123">ユーザーとしてラーニングパスサイトを使用するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="6846d-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="6846d-124">Office 365 のユーザー権限/SharePoint サイト訪問者のアクセス許可またはそれ以上</span><span class="sxs-lookup"><span data-stu-id="6846d-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="6846d-125">カスタマイズの概要</span><span class="sxs-lookup"><span data-stu-id="6846d-125">Get started with customization</span></span>
<span data-ttu-id="6846d-126">サイトと web パーツをカスタマイズするために必要なアクセス許可があることを確認したら、カスタマイズプロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="6846d-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="6846d-127">開始するには、「[ラーニングパスサイトに移動する](custom_goto.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6846d-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>