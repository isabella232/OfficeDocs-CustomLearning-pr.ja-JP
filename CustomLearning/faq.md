---
author: karuanag
ms.author: karuanag
title: Office 365 ソリューションのカスタム学習に関してよく寄せられる質問
ms.date: 02/10/2019
description: Office 365 のカスタム学習に関するよく寄せられる質問の情報
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056011"
---
# <a name="frequently-asked-questions"></a><span data-ttu-id="22787-103">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="22787-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="22787-104">1. Office 365 用のカスタム学習をテナント環境にインストールするための要件は何ですか。</span><span class="sxs-lookup"><span data-stu-id="22787-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="22787-105">SharePoint Online とコミュニケーションサイトが有効になっている。</span><span class="sxs-lookup"><span data-stu-id="22787-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="22787-106">CLO365 をプロビジョニングするユーザーは、インストール先のテナントのテナント管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="22787-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="22787-107">テナント ' App Catalog ' は、SharePoint 管理センターの [アプリ] オプション内で使用できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="22787-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="22787-108">CLO365 をプロビジョニングするユーザーは、インストール先のテナントのアプリカタログのサイトコレクション管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="22787-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="22787-109">2. どの言語が Office 365 用のカスタム学習で利用できますか?</span><span class="sxs-lookup"><span data-stu-id="22787-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="22787-110">Office 365 のカスタム学習は、現在英語版でのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="22787-110">Custom Learning for Office 365 is currently available only in English.</span></span> <span data-ttu-id="22787-111">自動エンドツーエンドプロビジョニングは、英語のテナントでのみ機能します。</span><span class="sxs-lookup"><span data-stu-id="22787-111">Automatic end-to-end provisioning only works with English tenants.</span></span> <span data-ttu-id="22787-112">今後のリリースでは、追加の言語が追加される場合があります。</span><span class="sxs-lookup"><span data-stu-id="22787-112">Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="22787-113">3. テナント環境にサイトをインストールするのにどれくらいの時間がかかりますか?</span><span class="sxs-lookup"><span data-stu-id="22787-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="22787-114">インストールのテストに基づき、15分未満で完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="22787-114">Based on our testing of the installation, it should take less than 15 minutes.</span></span> <span data-ttu-id="22787-115">これには、要件に合わせてサイトをカスタマイズするのに必要な時間は含まれません。</span><span class="sxs-lookup"><span data-stu-id="22787-115">This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="22787-116">4. Office 365 のカスタム学習は、プライマリ SharePoint サイトコレクションのサブサイトにすることができますか。</span><span class="sxs-lookup"><span data-stu-id="22787-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="22787-117">いいえ。</span><span class="sxs-lookup"><span data-stu-id="22787-117">No.</span></span> <span data-ttu-id="22787-118">サイトは、コミュニケーションサイトテンプレートに基づいています。これは、常にルートサイトコレクションであることを意図しています。</span><span class="sxs-lookup"><span data-stu-id="22787-118">The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="22787-119">エンドユーザーがサイトにアクセスするために必要なアクセス許可について考慮することが重要です。</span><span class="sxs-lookup"><span data-stu-id="22787-119">It is important to consider the permissions your end users will need to access the site.</span></span> <span data-ttu-id="22787-120">多くの組織では、セキュリティまたはユーザーグループを定義しています。</span><span class="sxs-lookup"><span data-stu-id="22787-120">Most organizations have defined security or user groups.</span></span> <span data-ttu-id="22787-121">従業員コミュニティに対してを開始する準備ができたら、適切なセキュリティグループを新しいトレーニングポータルに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="22787-121">You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="22787-122">5. サイトを再インストールする必要があります。どうしたらいいでしょう。</span><span class="sxs-lookup"><span data-stu-id="22787-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="22787-123">[ここで](custom_provision.md)公開されているインストール手順に従います。</span><span class="sxs-lookup"><span data-stu-id="22787-123">Follow the installation instructions published [here](custom_provision.md).</span></span>

> [!NOTE]
> <span data-ttu-id="22787-124">以前のインストールでテレメトリを無効にしていて、テレメトリを無効にしたままにする場合は、ここでテレメトリを無効にするための手順に従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="22787-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="22787-125">6. Office 365 のカスタム学習の実装を更新しました。</span><span class="sxs-lookup"><span data-stu-id="22787-125">6. We made updates to our implementation of Custom Learning for Office 365.</span></span> <span data-ttu-id="22787-126">サイトを再インストールすると、これらの更新プログラム (サイトテンプレート、再生リストに加えられたもの) は失われますか?</span><span class="sxs-lookup"><span data-stu-id="22787-126">Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="22787-127">現在のインストール環境でサイトを再インストールすると、個々のページおよびカスタム再生リストに対するカスタマイズが失われます。</span><span class="sxs-lookup"><span data-stu-id="22787-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  