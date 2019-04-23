---
author: karuanag
ms.author: karuanag
title: 前提条件と決定事項
ms.date: 02/10/2019
description: カスタム学習のインストールおよびセットアップに関する決定事項と前提条件に関する情報
ms.openlocfilehash: b7864d13e6ccd9c3b41e445ea491aed3b3471aff
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055267"
---
## <a name="service-decisions"></a><span data-ttu-id="d2d65-103">サービスに関する決定事項</span><span class="sxs-lookup"><span data-stu-id="d2d65-103">Service Decisions</span></span>

<span data-ttu-id="d2d65-104">カスタム学習の前提条件が満たされていることを確認した後、カスタム学習の implemenation について次のような決定を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2d65-104">After you've ensured that the prerequisites for Custom Learning have been met, you'll need to make the following decisions about your implemenation of Custom Learning:</span></span>

1. <span data-ttu-id="d2d65-105">**自社では、最新のインターフェイスを使用して既にトレーニングポータルが提供されていますか?**</span><span class="sxs-lookup"><span data-stu-id="d2d65-105">**Do you already have a training portal in your company with a modern interface?**</span></span>

- <span data-ttu-id="d2d65-106">**はい**これらの質問に対する回答が [はい] の場合は、既存のサイトの環境内に[web パーツをインストール](installwebpart.md)することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d2d65-106">**YES** If your answer to these questions are yes, then [installing the webpart](installwebpart.md) within that existing site experience is our recommended course of action.</span></span>
- <span data-ttu-id="d2d65-107">**いいえ**「いいえ」と答えた場合は[、完全なカスタム学習サイトパッケージをインストールする](installsitepackage.md)ことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d2d65-107">**NO** If you answer no we suggest [installing the full Custom Learning site](installsitepackage.md) package.</span></span>  <span data-ttu-id="d2d65-108">これにより、エンドユーザーにとって重要なその他の情報を拡張できる、最新の SharePoint Online コミュニケーションサイトが準備されます。</span><span class="sxs-lookup"><span data-stu-id="d2d65-108">This will prepare you with a modern SharePoint Online communication site that your can expand to house other information that is important to your end users.</span></span>  <span data-ttu-id="d2d65-109">サイトをカスタマイズしても、web パーツのコンテンツ更新を取得する機能に影響はありません。</span><span class="sxs-lookup"><span data-stu-id="d2d65-109">Customizing the site will not impact the webpart's ability to get content updates.</span></span> 

2. <span data-ttu-id="d2d65-110">**Office 365 管理者**</span><span class="sxs-lookup"><span data-stu-id="d2d65-110">**Are you an Office 365 Administrator?**</span></span>

- <span data-ttu-id="d2d65-111">**はい**。どちらのインストールにも適切な権限があります。</span><span class="sxs-lookup"><span data-stu-id="d2d65-111">**YES**:  You have the appropriate rights for either installation.</span></span>
- <span data-ttu-id="d2d65-112">**いいえ**: Office 365 管理者に問い合わせてください。または、所有しているサイトコレクションに web パーツをインストールします</span><span class="sxs-lookup"><span data-stu-id="d2d65-112">**NO**: Contact your Office 365 Administrator for assistance or install the webpart in a site collection you own</span></span>

3. <span data-ttu-id="d2d65-113">**組織に正式なトレーニング部署がありますか。**</span><span class="sxs-lookup"><span data-stu-id="d2d65-113">**Do you have a formal training department in your organization?**</span></span>

- <span data-ttu-id="d2d65-114">**はい**: これらのソリューションを使用して、カスタマイズされた追加のトレーニングコンテンツを提供する方法については、必ずご確認ください。</span><span class="sxs-lookup"><span data-stu-id="d2d65-114">**YES**:  Make sure to engage them and let them know how they can use these solutions to deliver additional, customized training content.</span></span>
- <span data-ttu-id="d2d65-115">**いいえ**:[セルフサービス導入キット](driveadoption.md)を使用して、エンドユーザーがサイトを認識できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d2d65-115">**NO**:  Use our [self service adoption kit](driveadoption.md) to make your end-users aware the site is available to help them.</span></span>

4. <span data-ttu-id="d2d65-116">**組織にユーザーコミュニティがありますか。 これは、テクノロジについて理解しているユーザーの公式または非公式のグループ (power users と呼ばれることもありますが、詳細について説明しているもの) のいずれかです。**</span><span class="sxs-lookup"><span data-stu-id="d2d65-116">**Do you have a user community in your organization?  This would be either a formal or informal group of users who like to know more about technology, sometimes called power users or just those interested to learn more.**</span></span>

- <span data-ttu-id="d2d65-117">**はい**: カスタム学習サイトの環境を使用して、新規または既存のユーザーコミュニティフォーラムへのリンクを提供できます。</span><span class="sxs-lookup"><span data-stu-id="d2d65-117">**YES**:  You can use the Custom Learning site experience to provide links to any new or existing user community forums.</span></span>
- <span data-ttu-id="d2d65-118">**いいえ**: 内部ユーザーグループを開始することを検討して、ユーザーが自分の成功を共有し、互いに情報を共有できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d2d65-118">**NO**:  Consider starting an internal user group so people can share their success and learn from each other.</span></span>  <span data-ttu-id="d2d65-119">内部ユーザーグループを育成する時間がない場合、従業員は、毎月のトレーニング、オンラインコミュニティのメンバーシップ、および Office 365 のツールとリソースへの早期アクセスのために、 [microosft Office 365 チャンピオンコミュニティ](https://aka.ms/O365Champions)に参加できます。</span><span class="sxs-lookup"><span data-stu-id="d2d65-119">If you don't have time to nurture an internal user group you and your employees can join the [Microosft Office 365 Champion community](https://aka.ms/O365Champions) for monthly training, membership in the online community and early access to tools and resources for Office 365.</span></span>

5.  <span data-ttu-id="d2d65-120">**サイトのメンテナンスやサポートに関する質問を行うことができますか。**</span><span class="sxs-lookup"><span data-stu-id="d2d65-120">**Will you be accountable for site maintenance or support questions?**</span></span>

- <span data-ttu-id="d2d65-121">**はい**: カスタム学習サイトのサポートを容易にするために、Office 365 の機能を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d2d65-121">**YES**: We suggest using the capabilities of Office 365 to make Custom Learning site support easier.</span></span>  <span data-ttu-id="d2d65-122">サービスのサブスクリプションと組織の規模に応じて、次のようないくつかのアイデアがあります。</span><span class="sxs-lookup"><span data-stu-id="d2d65-122">Some ideas, depending on your service subscription and organization size are:</span></span>
    1. <span data-ttu-id="d2d65-123">大規模な組織では、サイトのフィードバックを得るために、パブリック Yammer コミュニティを準備できます。</span><span class="sxs-lookup"><span data-stu-id="d2d65-123">Large organizations can provision a public Yammer community to get feedback on the site</span></span>
    2. <span data-ttu-id="d2d65-124">最大2500人のユーザーが Microsoft teams に参加して、質問や会話を共有できます。</span><span class="sxs-lookup"><span data-stu-id="d2d65-124">Up to 2500 people can join a Microsoft Team to ask questions and share conversation</span></span>
    3. <span data-ttu-id="d2d65-125">正式なサポートチケットのプロセスは、フォーム、フロー、SharePoint Online のリスト、または会社の IT サポートのために既に提供されている他のサードパーティ製のツールを使用して suppored ことができます。</span><span class="sxs-lookup"><span data-stu-id="d2d65-125">A formal support ticketing process can be suppored with Forms, Flow and SharePoint Online lists or through other 3rd party tools which you may already have for IT support in your company.</span></span> 
- <span data-ttu-id="d2d65-126">**いいえ**: SharePoint Online のサポートを提供する IT スタッフとサイトまたは web パーツのインストールについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d2d65-126">**NO**:  Discuss the installation of the site/webpart with your IT staff who provide SharePoint Online support.</span></span>  

### <a name="next-steps---site-provisioninginstallsitepackagemd-or-webpartinstallwebpartmd-installation-steps"></a><span data-ttu-id="d2d65-127">次の手順-[サイトプロビジョニング](installsitepackage.md)または[web パーツ](installwebpart.md)のインストール手順</span><span class="sxs-lookup"><span data-stu-id="d2d65-127">Next Steps - [Site Provisioning](installsitepackage.md) or [webpart](installwebpart.md) installation steps</span></span>