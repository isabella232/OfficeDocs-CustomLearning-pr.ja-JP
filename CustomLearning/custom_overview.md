---
author: pkrebs
ms.author: pkrebs
title: 学習経路をカスタマイズする
ms.date: 02/18/2019
manager: bpardi
audience: admin
ms.topic: article
description: 学習経路をカスタマイズする
ms.service: sharepoint-online
ms.openlocfilehash: a5087096ec3bd7c1194aab9dd089276fc196a736
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999503"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="69b6e-103">学習経路をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="69b6e-103">Customize learning pathways</span></span>

<span data-ttu-id="69b6e-104">Microsoft 365 ラーニング パスには、組織のコンテンツをカスタマイズできるさまざまな方法があります。</span><span class="sxs-lookup"><span data-stu-id="69b6e-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="69b6e-105">たとえば、次のようなことが可能です。</span><span class="sxs-lookup"><span data-stu-id="69b6e-105">For example, you can:</span></span>  
- <span data-ttu-id="69b6e-106">SharePoint サイトの学習経路を変更する - サイト名、ロゴ、およびそれらを変更します。</span><span class="sxs-lookup"><span data-stu-id="69b6e-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="69b6e-107">[質問] ページと [ヘルプの取得] ページを変更して、独自のヘルプ センターを作成します。</span><span class="sxs-lookup"><span data-stu-id="69b6e-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="69b6e-108">組織でサポートされているサービスまたは機能を反映するコンテンツを非表示または表示する</span><span class="sxs-lookup"><span data-stu-id="69b6e-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="69b6e-109">ユーザーのニーズに合ったカスタムプレイリストとサブカテゴリを構築する</span><span class="sxs-lookup"><span data-stu-id="69b6e-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="69b6e-110">Microsoft Teams、Outlook mobile の導入の促進、Microsoft 365 との共同作業など、ビジネスの成果をサポートするためにコンテンツがフィルター処理されたランディング ページを構築します。</span><span class="sxs-lookup"><span data-stu-id="69b6e-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![一般的な Microsoft ラーニング パスの写真コレクション。](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="69b6e-112">要件とアクセス許可</span><span class="sxs-lookup"><span data-stu-id="69b6e-112">Requirements and Permissions</span></span>

<span data-ttu-id="69b6e-113">[学習経路のカスタマイズ] ガイダンスを開始する前に、SharePoint テナント管理者が学習経路を設定してください。</span><span class="sxs-lookup"><span data-stu-id="69b6e-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="69b6e-114">セットアップされたのか不明な場合は、SharePoint テナント管理者に問い合わせて、学習経路が準備されたと確認してください。</span><span class="sxs-lookup"><span data-stu-id="69b6e-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="69b6e-115">また、学習経路 SharePoint サイトの URL も必ず取得してください。</span><span class="sxs-lookup"><span data-stu-id="69b6e-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="69b6e-116">テナント管理者であり、ラーニング パスがプロビジョニングされていない場合は、「Provision learning [pathways」を参照してください](custom_provision.md)。</span><span class="sxs-lookup"><span data-stu-id="69b6e-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="69b6e-117">学習経路を準備するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="69b6e-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="69b6e-118">テナント管理者 (365 グローバルOfficeとも呼ばれる)</span><span class="sxs-lookup"><span data-stu-id="69b6e-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="69b6e-119">サイトの所有者アクセス許可を持つ SharePoint サイト コレクション管理者</span><span class="sxs-lookup"><span data-stu-id="69b6e-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="69b6e-120">ラーニング パスの管理機能を使用するアクセス許可</span><span class="sxs-lookup"><span data-stu-id="69b6e-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="69b6e-121">サイト コレクションの管理者</span><span class="sxs-lookup"><span data-stu-id="69b6e-121">Site Collection Administrator</span></span>
- <span data-ttu-id="69b6e-122">SharePoint 所有者またはメンバーのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="69b6e-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="69b6e-123">ラーニング パス サイトをユーザーとして使用するアクセス許可</span><span class="sxs-lookup"><span data-stu-id="69b6e-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="69b6e-124">Office 365 ユーザー アクセス許可/SharePoint サイト訪問者アクセス許可以上</span><span class="sxs-lookup"><span data-stu-id="69b6e-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="69b6e-125">カスタマイズを始めましょう</span><span class="sxs-lookup"><span data-stu-id="69b6e-125">Get started with customization</span></span>
<span data-ttu-id="69b6e-126">サイトと Web パーツをカスタマイズするために必要なアクセス許可が付与された後は、カスタマイズ プロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="69b6e-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="69b6e-127">開始するには、「Go [to the learning pathways site」を参照してください](custom_goto.md)。</span><span class="sxs-lookup"><span data-stu-id="69b6e-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>