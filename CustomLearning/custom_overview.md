---
author: pkrebs
ms.author: pkrebs
title: 概要
ms.date: 02/15/2019
description: Office 365 の管理者向けのカスタム学習の概要
ms.openlocfilehash: c4b9679ae5a7158306bfd53e345f8e892ab206bc
ms.sourcegitcommit: afb5502604d271f49f6d1133db9dfc499f710eec
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30064987"
---
# <a name="overview-of-custom-learning"></a><span data-ttu-id="25525-103">カスタム学習の概要</span><span class="sxs-lookup"><span data-stu-id="25525-103">Overview of Custom Learning</span></span>
<span data-ttu-id="25525-p101">office 365 のカスタム学習の概要組織内での office 365 の使用と導入を高速化するために設計された、Microsoft の新しいソリューション。カスタム学習を使用すると、次のことができます。</span><span class="sxs-lookup"><span data-stu-id="25525-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>

- <span data-ttu-id="25525-p102">Office 365 のカスタム学習を環境に合わせて調整します。ブランドとロゴ、トレーニングイベント、サポート情報を使用して、サイトページを変更します。組織でサポートされていないサービスまたは機能のコンテンツを表示または非表示にします。</span><span class="sxs-lookup"><span data-stu-id="25525-p102">Tailor Custom Learning for Office 365 to your environment. Modify site pages with your brand and logo, training events, and support info. Hide and show content for services or features that are not supported in your organization.</span></span> 
- <span data-ttu-id="25525-109">microsoft では、コンテンツとユーザーを最新の状態に保つことができます。カスタム学習によって、microsoft が最新の状態に保つことができる学習コンテンツの動的なフィードが提供されます。</span><span class="sxs-lookup"><span data-stu-id="25525-109">Let Microsoft keep your content and users up-to-date – Custom Learning provides a dynamic feed of learning content that Microsoft keeps up-to-date.</span></span> 
- <span data-ttu-id="25525-110">組織のポリシー、手順、およびカルチャを反映したカテゴリとカスタムの再生リストを作成します。これにより、ユーザーは各自のニーズに特化した学習コンテンツを使用してスキルを構築できるようになります。</span><span class="sxs-lookup"><span data-stu-id="25525-110">Build categories and custom playlists reflecting your organization’s policies, procedures, and culture, enabling users to build skills with learning content crafted specifically to their needs.</span></span>

![cg_introducing](media/cg_introducing.png)

## <a name="how-does-custom-learning-word"></a><span data-ttu-id="25525-112">カスタム学習 word について</span><span class="sxs-lookup"><span data-stu-id="25525-112">How does Custom Learning word?</span></span>
<span data-ttu-id="25525-113">カスタム学習 Office 365 (カスタム学習の省略) は、次の3つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="25525-113">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
- <span data-ttu-id="25525-114">SharePoint コミュニケーションサイト</span><span class="sxs-lookup"><span data-stu-id="25525-114">a SharePoint communication site</span></span>
- <span data-ttu-id="25525-115">SharePoint web パーツ</span><span class="sxs-lookup"><span data-stu-id="25525-115">a SharePoint web part</span></span>
- <span data-ttu-id="25525-116">Microsoft online カタログからのコンテンツのライブフィード</span><span class="sxs-lookup"><span data-stu-id="25525-116">a live feed of content from a Microsoft online catalog</span></span>

![cg_howitworks](media/cg_howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="25525-118">要件とアクセス許可</span><span class="sxs-lookup"><span data-stu-id="25525-118">Requirements and Permissions</span></span>
<span data-ttu-id="25525-p103">Office 365 のカスタム学習は、組織のテナント管理者によってインストールされている必要があります。テナント管理者のアクセス許可を持つユーザー。このガイドで説明されているカスタマイズ手順を開始する前に、SharePoint テナント管理者がカスタム学習をセットアップしていることを確認してください。わからない場合は、SharePoint テナント管理者に連絡して、カスタム学習がインストールされていることを確認してください。また、カスタムラーニング SharePoint サイトの URL を取得するようにしてください。テナント管理者であり、カスタム学習がインストールされていない場合は、「custom learning for Office 365 インストールガイド」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25525-p103">Custom Learning for Office 365 must be installed by your organization’s tenant administrator - someone who has Tenant Administrator permission. Before getting started with this customization procedures covered in this guide, ensure that Custom Learning has been set up by a SharePoint tenant administrator. If you’re not sure, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-required-for-custom-learning"></a><span data-ttu-id="25525-124">カスタム学習に必要なアクセス許可</span><span class="sxs-lookup"><span data-stu-id="25525-124">Permissions required for Custom Learning</span></span> 
<span data-ttu-id="25525-125">カスタム学習をインストール、カスタマイズ、および使用するために必要なアクセス許可の詳細を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="25525-125">Here’s a breakdown of the permissions required for installing, customizing, and using Custom Learning.</span></span> 

<span data-ttu-id="25525-126">**カスタム学習をインストールするためのアクセス許可**</span><span class="sxs-lookup"><span data-stu-id="25525-126">**Permissions to install Custom Learning**</span></span>
- <span data-ttu-id="25525-127">Office 365 グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="25525-127">Office 365 Global Administrator</span></span>
- <span data-ttu-id="25525-128">SharePoint 管理者</span><span class="sxs-lookup"><span data-stu-id="25525-128">SharePoint Administrator</span></span>

<span data-ttu-id="25525-129">**カスタム学習管理機能を使用するためのアクセス許可**</span><span class="sxs-lookup"><span data-stu-id="25525-129">**Permissions to use Custom Learning Administration features**</span></span>
- <span data-ttu-id="25525-130">Office 365 sharepoint 管理者/sharepoint サイト所有者のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="25525-130">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="25525-131">sharepoint サイトコレクション管理者/sharepoint サイト所有者のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="25525-131">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

<span data-ttu-id="25525-132">**カスタムラーニングサイトをユーザーとして使用するには**</span><span class="sxs-lookup"><span data-stu-id="25525-132">**To use the Custom Learning site as a user**</span></span>
- <span data-ttu-id="25525-133">Office 365 のユーザー権限/SharePoint サイト訪問者のアクセス許可またはそれ以上</span><span class="sxs-lookup"><span data-stu-id="25525-133">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>
- <span data-ttu-id="25525-134">必要なアクセス許可が付与されているかどうかがわからない場合は、SharePoint テナント管理者に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="25525-134">If you’re not sure if you’ve been granted the necessary permissions, contact your SharePoint Tenant Administrator.</span></span>

### <a name="next-steps"></a><span data-ttu-id="25525-135">次のステップ</span><span class="sxs-lookup"><span data-stu-id="25525-135">Next Steps</span></span>

- [<span data-ttu-id="25525-136">プレイリストをカスタマイズして共有する</span><span class="sxs-lookup"><span data-stu-id="25525-136">Customize and Share Playlists</span></span>](customplaylist.md)
- [<span data-ttu-id="25525-137">ドライブ導入</span><span class="sxs-lookup"><span data-stu-id="25525-137">Drive Adoption</span></span>](driveadoption.md) 