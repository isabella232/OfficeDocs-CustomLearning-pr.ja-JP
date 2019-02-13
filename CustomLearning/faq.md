---
author: karuanag
ms.author: karuanag
title: よく寄せられる質問のソリューションを Office 365 のユーザー設定の学習
ms.date: 02/10/2019
description: Office 365 のカスタム学習するための質問の情報を掲載
ms.openlocfilehash: d8b5104e8feeaa4e70296f61594233b27363481b
ms.sourcegitcommit: f93a6a691331515ba10f4d43b491928ec268f0ec
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29952633"
---
# <a name="frequently-asked-questions"></a><span data-ttu-id="c3df2-103">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="c3df2-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="c3df2-104">1. テナント環境に Office 365 のユーザー設定の学習をインストールするための要件とは?</span><span class="sxs-lookup"><span data-stu-id="c3df2-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="c3df2-105">SharePoint Online との通信のサイトが有効になっています。</span><span class="sxs-lookup"><span data-stu-id="c3df2-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="c3df2-106">CLO365 を提供している個人は、インストール用のターゲット ・ テナントのテナント管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3df2-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="c3df2-107">テナント 'アプリケーション カタログ' は、SharePoint の管理センターの 'アプリケーション' オプションで使用可能なする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3df2-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="c3df2-108">CLO365 を提供している個人は、インストールのターゲット ・ テナントのアプリケーション カタログのサイト コレクションの管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3df2-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="c3df2-109">2. どのような言語は、で利用可能な Office 365 のユーザー設定の学習ですか。</span><span class="sxs-lookup"><span data-stu-id="c3df2-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="c3df2-p101">カスタムの Office 365 の学習は、英語のみで現在利用可能です。エンド ・ ツー ・ エンドの自動プロビジョニングは、テナントが英語でのみ機能します。その他の言語は、リリースの将来の追加があります。</span><span class="sxs-lookup"><span data-stu-id="c3df2-p101">Custom Learning for Office 365 is currently available only in English. Automatic end-to-end provisioning only works with English tenants. Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="c3df2-113">3 テナント環境でサイトをインストールするのには時間がかかりますか。</span><span class="sxs-lookup"><span data-stu-id="c3df2-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="c3df2-p102">インストールのテストに基づきと、15 分未満である必要がありますがかかります。これには、お客様の要件にサイトをカスタマイズするために必要な時間は含まれません。</span><span class="sxs-lookup"><span data-stu-id="c3df2-p102">Based on our testing of the installation, it should take less than 15 minutes. This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="c3df2-116">4. 行うものでは、カスタムの Office 365 のプライマリ SharePoint サイト コレクションのサブサイトを学習しますか。</span><span class="sxs-lookup"><span data-stu-id="c3df2-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="c3df2-p103">違います。サイトは、ルート サイト コレクションを常に説明したものである、通信のサイト テンプレートに基づきます。</span><span class="sxs-lookup"><span data-stu-id="c3df2-p103">No. The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="c3df2-p104">エンド ・ ユーザーがサイトにアクセスする必要があるアクセス許可を考慮する重要です。ほとんどの組織では、セキュリティまたはユーザーのグループを定義しています。従業員コミュニティにそれを起動する準備ができたら、新しいトレーニング ポータルに適切なセキュリティ グループを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3df2-p104">It is important to consider the permissions your end users will need to access the site. Most organizations have defined security or user groups. You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="c3df2-122">5 サイトを再インストールする必要がある.どうしたらいいでしょう。</span><span class="sxs-lookup"><span data-stu-id="c3df2-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="c3df2-123">インストール手順について公開されている[ここで](installsitepackage.md)次の。</span><span class="sxs-lookup"><span data-stu-id="c3df2-123">Follow the installation instructions published [here](installsitepackage.md).</span></span>

> [!NOTE]
> <span data-ttu-id="c3df2-124">「遠隔測定」以前インストール無効にして無効になっている「遠隔測定」を続行したい場合は、指示に従って、ここで「遠隔測定」を無効にするために必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3df2-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="c3df2-p105">6. 更新プログラムに加えた Office 365 のユーザー設定の学習の導入。失われます (サイト テンプレートでは、再生リストを作成します)、これらの更新プログラムをサイトを再インストールしている場合ですか。</span><span class="sxs-lookup"><span data-stu-id="c3df2-p105">6. We made updates to our implementation of Custom Learning for Office 365. Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="c3df2-127">現在インストールされている上、サイトを再インストールする場合、個々 のページおよびカスタム再生リストのカスタマイズ設定はすべて失われます。</span><span class="sxs-lookup"><span data-stu-id="c3df2-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  