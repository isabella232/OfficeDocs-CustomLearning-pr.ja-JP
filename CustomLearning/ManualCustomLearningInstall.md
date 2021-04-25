---
author: pkrebs
ms.author: pkrebs
title: 手動インストールのラーニング パス
ms.date: 02/18/2019
manager: bpardi
description: 手動インストールのラーニング パス
ms.service: sharepoint-online
ms.openlocfilehash: 7dd43e7ed66b7a8fdcd40d76d9d2bcb9403ad4bb
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999213"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a><span data-ttu-id="cbafe-103">365 のカスタム 学習を手動でインストールOfficeする</span><span class="sxs-lookup"><span data-stu-id="cbafe-103">Manually installing and configuring Custom Learning for Office 365</span></span>

<span data-ttu-id="cbafe-104">Microsoft Custom Learning Web パーツは [、SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) バージョン 1.7.1 を使用してビルドされます。</span><span class="sxs-lookup"><span data-stu-id="cbafe-104">The Microsoft Custom Learning Web Part is build using the [SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) version 1.7.1.</span></span>

<span data-ttu-id="cbafe-105">Web パーツとサイト コレクションを手動でインストールして構成するには、次の手順を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbafe-105">To manually install and configure the web part and site collection, you will need to complete the following steps:</span></span>

1. <span data-ttu-id="cbafe-106">すべての前提条件を満たしていることを検証します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-106">Validate that you have met all the prerequisites.</span></span>
1. <span data-ttu-id="cbafe-107">カスタムlearning.sppkg ファイルを 365 テナント Officeカタログにインストールします。</span><span class="sxs-lookup"><span data-stu-id="cbafe-107">Install the customlearning.sppkg file in your Office 365 Tenant App Catalog.</span></span>
1. <span data-ttu-id="cbafe-108">365 ホーム サイトのカスタム 学習として機能する最新Officeを指定します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-108">Provision/Identify a modern communication site to act as your Custom Learning for Office 365 home site.</span></span>
1. <span data-ttu-id="cbafe-109">カスタム学習が依存する適切な成果物を使用してテナントを構成する PowerShell スクリプトを実行します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-109">Execute a PowerShell script that will configure your tenant with the appropriate artifacts that Custom Learning depends on.</span></span>
1. <span data-ttu-id="cbafe-110">CustomLearningAdmin.aspx サイト ページに移動して管理 Web パーツを読み込み、カスタム コンテンツ構成を初期化します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-110">Navigate to the CustomLearningAdmin.aspx site page to load the admin web part to initialize the custom content configuration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbafe-111">前提条件</span><span class="sxs-lookup"><span data-stu-id="cbafe-111">Prerequisites</span></span>

<span data-ttu-id="cbafe-112">テナント全体のアプリ カタログをセットアップして構成している必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbafe-112">You must have set up and configured the tenant-wide App Catalog.</span></span> <span data-ttu-id="cbafe-113">[「365 テナントOfficeセットアップ」を参照](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)し、[アプリ カタログ サイトの作成] セクションに従います。</span><span class="sxs-lookup"><span data-stu-id="cbafe-113">See [Set up your Office 365 tenant](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) and follow the Create app catalog site section.</span></span> <span data-ttu-id="cbafe-114">テナント全体のアプリ カタログが既にプロビジョニングされている場合は、このセットアップ プロセスを完了するために、パッケージをアップロードする権限を持つアカウントにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbafe-114">If your tenant-wide App Catalog has already been provisioned, you will need access to an account that has rights to upload a package to it to complete this setup process.</span></span> <span data-ttu-id="cbafe-115">通常、このアカウントには SharePoint 管理者の役割があります。</span><span class="sxs-lookup"><span data-stu-id="cbafe-115">Generally this account has the SharePoint administrator role.</span></span> <span data-ttu-id="cbafe-116">その役割を持つアカウントが機能しない場合は、SharePoint 管理センターに移動し、アプリ カタログ サイト コレクションのサイト コレクション管理者を見つけて、サイト コレクション管理者の 1 人としてログインするか、サイト コレクション管理者に失敗した SharePoint 管理者アカウントを追加します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-116">If an account with that role does not work, go to the SharePoint admin center and find the Site Collection Administrators for the app catalog site collection and either log in as one of the Site Collection Administrators, or add the SharePoint administrator account that failed to the Site Collection Administrators.</span></span> <span data-ttu-id="cbafe-117">また、SharePoint テナント管理者であるアカウントにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbafe-117">You will also need access to an account that is a SharePoint Tenant Admin.</span></span>

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a><span data-ttu-id="cbafe-118">Web パーツをテナント アプリ カタログにアップロードする</span><span class="sxs-lookup"><span data-stu-id="cbafe-118">Upload the web part to the Tenant App Catalog</span></span>

<span data-ttu-id="cbafe-119">カスタム ラーニングを Office 365 に設定するには、customlearning.sppkg ファイルをテナント全体のアプリ カタログにアップロードして展開します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-119">To set up Custom Learning for Office 365, you upload the customlearning.sppkg file to the tenant-wide App Catalog and deploy it.</span></span> <span data-ttu-id="cbafe-120">アプリ [カタログにアプリを追加する](/sharepoint/use-app-catalog) 方法の詳細については、「アプリ カタログを使用して SharePoint Online 環境でカスタム ビジネス アプリを使用する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbafe-120">See [Use the App Catalog to make custom business apps available for your SharePoint Online environment](/sharepoint/use-app-catalog) for detailed instructions on how to add an app to the app catalog.</span></span>

## <a name="provisionidentify-modern-communication-site"></a><span data-ttu-id="cbafe-121">モダン コミュニケーション サイトのプロビジョニング/識別</span><span class="sxs-lookup"><span data-stu-id="cbafe-121">Provision/Identify Modern Communication Site</span></span>

<span data-ttu-id="cbafe-122">既存の SharePoint 通信サイトを識別するか、SharePoint Online テナントに新しい通信サイトをプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="cbafe-122">Either identify an existing SharePoint communication site or provision a new one in your SharePoint Online tenant.</span></span> <span data-ttu-id="cbafe-123">通信サイトを準備する方法の詳細については [、「SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) で通信サイトを作成する」を参照し、手順に従って通信サイトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-123">For more information about how to provision a communication site, see [Create a communication site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) and follow the steps to create a communication site.</span></span>

## <a name="set-permissions-for-the-site"></a><span data-ttu-id="cbafe-124">サイトのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="cbafe-124">Set permissions for the site</span></span>

<span data-ttu-id="cbafe-125">コンテンツを表示できる必要があるすべてのユーザーを Visitors グループに追加し、カスタムプレイリストをメンバー グループに管理できる必要があるすべてのユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-125">You will want to add everyone who should be able to view content to the Visitors group and everyone who should be able to administer custom playlists to the Members group.</span></span> <span data-ttu-id="cbafe-126">ユーザーが初めてサイト コレクション管理者または所有者グループの一部である必要がある場合は、カスタム学習用にサイトを構成します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-126">To configure the site for Custom Learning the first time the user must be either a site collection administrator or part of the Owners group.</span></span>

<span data-ttu-id="cbafe-127">365 App Officeカスタム学習をサイト コレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-127">Add Custom Learning for Office 365 App to the site collection.</span></span>

## <a name="execute-powershell-configuration-script"></a><span data-ttu-id="cbafe-128">PowerShell 構成スクリプトの実行</span><span class="sxs-lookup"><span data-stu-id="cbafe-128">Execute PowerShell Configuration Script</span></span>

<span data-ttu-id="cbafe-129">PowerShell スクリプトが含まれているので、ソリューションで使用する 3 つのテナント プロパティを作成するために実行 `CustomLearningConfiguration.ps1` する必要があります。 [](/sharepoint/dev/spfx/tenant-properties)</span><span class="sxs-lookup"><span data-stu-id="cbafe-129">A PowerShell script `CustomLearningConfiguration.ps1` is included that you will need to execute to create three [tenant properties](/sharepoint/dev/spfx/tenant-properties) that the solution uses.</span></span> <span data-ttu-id="cbafe-130">さらに、このスクリプトはサイト ページ[](/sharepoint/dev/spfx/web-parts/single-part-app-pages)ライブラリに 2 つの単一パーツ アプリ ページを作成し、管理者とユーザーの Web パーツを既知の場所でホストします。</span><span class="sxs-lookup"><span data-stu-id="cbafe-130">In addition, the script creates two [single part app pages](/sharepoint/dev/spfx/web-parts/single-part-app-pages) in the site pages library to host the admin and user web parts at a known location.</span></span>

### <a name="disabling-telemetry-collection"></a><span data-ttu-id="cbafe-131">テレメトリ コレクションの無効化</span><span class="sxs-lookup"><span data-stu-id="cbafe-131">Disabling Telemetry Collection</span></span>

<span data-ttu-id="cbafe-132">このソリューションの一部には、匿名化されたテレメトリ追跡オプトインが含まれます。既定ではオンに設定されています。</span><span class="sxs-lookup"><span data-stu-id="cbafe-132">Part of this solution includes anonymized telemetry tracking opt-in, which by default is set to on.</span></span> <span data-ttu-id="cbafe-133">手動インストールを実行し、テレメトリ追跡をオフにする場合は、スクリプトを変更して、$optInTelemetry 変数を $false `CustomlearningConfiguration.ps1` に設定します。</span><span class="sxs-lookup"><span data-stu-id="cbafe-133">If you are performing a manual install and you would like to turn telemetry tracking off, change the `CustomlearningConfiguration.ps1` script to set the $optInTelemetry variable to $false.</span></span>

<span data-ttu-id="cbafe-134">手動インストールを実行していない場合にテレメトリ追跡をオフにする場合は、実行時にテレメトリ追跡が無効にされる別のスクリプト `TelemetryOptOut.ps1` が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbafe-134">If you are not performing a manual install and would like to turn telemetry tracking off, a separate script `TelemetryOptOut.ps1` has been included that when run will disable telemetry tracking.</span></span>

## <a name="initialize-web-part-custom-configuration"></a><span data-ttu-id="cbafe-135">Web パーツのカスタム構成を初期化する</span><span class="sxs-lookup"><span data-stu-id="cbafe-135">Initialize web part custom configuration</span></span>

<span data-ttu-id="cbafe-136">PowerShell スクリプトが正常に実行された後、に移動します `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 。</span><span class="sxs-lookup"><span data-stu-id="cbafe-136">After the PowerShell script is successfully run, navigate to `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="cbafe-137">これにより、初めて使用するカスタム学習を設定する CustomConfig リスト アイテムが初期化されます。</span><span class="sxs-lookup"><span data-stu-id="cbafe-137">This initializes the CustomConfig list item that sets up custom learning for its first use.</span></span>

<span data-ttu-id="cbafe-138">これで構成が完了し、365 のカスタム 学習を使用してOfficeできます。</span><span class="sxs-lookup"><span data-stu-id="cbafe-138">The configuration is now complete and you can move forward with using Custom Learning for Office 365.</span></span> <span data-ttu-id="cbafe-139">詳細については、ユーザーのドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbafe-139">See the user documentation for more information.</span></span>
