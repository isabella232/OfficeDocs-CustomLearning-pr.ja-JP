---
author: pkrebs
ms.author: pkrebs
title: 手動インストールのラーニング パス
ms.date: 02/18/2019
manager: bpardi
description: 手動インストールのラーニング パス
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575972"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a><span data-ttu-id="91176-103">ユーザー設定のカスタム 学習を手動でインストールして構成Office 365</span><span class="sxs-lookup"><span data-stu-id="91176-103">Manually installing and configuring Custom Learning for Office 365</span></span>

<span data-ttu-id="91176-104">Microsoft Custom Learning Web パーツは、バージョン 1.7.1 [SharePoint Frameworkを](/sharepoint/dev/spfx/sharepoint-framework-overview)使用してビルドされます。</span><span class="sxs-lookup"><span data-stu-id="91176-104">The Microsoft Custom Learning Web Part is build using the [SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) version 1.7.1.</span></span>

<span data-ttu-id="91176-105">Web パーツとサイト コレクションを手動でインストールして構成するには、次の手順を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="91176-105">To manually install and configure the web part and site collection, you will need to complete the following steps:</span></span>

1. <span data-ttu-id="91176-106">すべての前提条件を満たしていることを検証します。</span><span class="sxs-lookup"><span data-stu-id="91176-106">Validate that you have met all the prerequisites.</span></span>
1. <span data-ttu-id="91176-107">テナント アプリ カタログに customlearning.sppkg ファイルOffice 365インストールします。</span><span class="sxs-lookup"><span data-stu-id="91176-107">Install the customlearning.sppkg file in your Office 365 Tenant App Catalog.</span></span>
1. <span data-ttu-id="91176-108">ホーム サイトのカスタム 学習として機能する最新のコミュニケーション サイトをプロビジョニングOffice 365します。</span><span class="sxs-lookup"><span data-stu-id="91176-108">Provision/Identify a modern communication site to act as your Custom Learning for Office 365 home site.</span></span>
1. <span data-ttu-id="91176-109">カスタム学習が依存する適切な成果物を使用してテナントを構成する PowerShell スクリプトを実行します。</span><span class="sxs-lookup"><span data-stu-id="91176-109">Execute a PowerShell script that will configure your tenant with the appropriate artifacts that Custom Learning depends on.</span></span>
1. <span data-ttu-id="91176-110">CustomLearningAdmin.aspx サイト ページに移動して管理 Web パーツを読み込み、カスタム コンテンツ構成を初期化します。</span><span class="sxs-lookup"><span data-stu-id="91176-110">Navigate to the CustomLearningAdmin.aspx site page to load the admin web part to initialize the custom content configuration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91176-111">前提条件</span><span class="sxs-lookup"><span data-stu-id="91176-111">Prerequisites</span></span>

<span data-ttu-id="91176-112">テナント全体のアプリ カタログをセットアップして構成している必要があります。</span><span class="sxs-lookup"><span data-stu-id="91176-112">You must have set up and configured the tenant-wide App Catalog.</span></span> <span data-ttu-id="91176-113">「[アプリ カタログ サイトのOffice 365を設定し、[](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)アプリ カタログ サイトの作成] セクションに従います。</span><span class="sxs-lookup"><span data-stu-id="91176-113">See [Set up your Office 365 tenant](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) and follow the Create app catalog site section.</span></span> <span data-ttu-id="91176-114">テナント全体のアプリ カタログが既にプロビジョニングされている場合は、このセットアップ プロセスを完了するために、パッケージをアップロードする権限を持つアカウントにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="91176-114">If your tenant-wide App Catalog has already been provisioned, you will need access to an account that has rights to upload a package to it to complete this setup process.</span></span> <span data-ttu-id="91176-115">通常、このアカウントには管理者SharePointがあります。</span><span class="sxs-lookup"><span data-stu-id="91176-115">Generally this account has the SharePoint administrator role.</span></span> <span data-ttu-id="91176-116">その役割を持つアカウントが機能しない場合は、SharePoint 管理センターに移動し、アプリ カタログ サイト コレクションのサイト コレクション管理者を見つけて、サイト コレクション管理者の 1 人としてログインするか、サイト コレクション管理者に失敗した SharePoint 管理者アカウントを追加します。</span><span class="sxs-lookup"><span data-stu-id="91176-116">If an account with that role does not work, go to the SharePoint admin center and find the Site Collection Administrators for the app catalog site collection and either log in as one of the Site Collection Administrators, or add the SharePoint administrator account that failed to the Site Collection Administrators.</span></span> <span data-ttu-id="91176-117">また、テナント管理者の管理者であるアカウントSharePoint必要があります。</span><span class="sxs-lookup"><span data-stu-id="91176-117">You will also need access to an account that is a SharePoint Tenant Admin.</span></span>

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a><span data-ttu-id="91176-118">アップロード Web パーツをテナント アプリ カタログに追加する</span><span class="sxs-lookup"><span data-stu-id="91176-118">Upload the web part to the Tenant App Catalog</span></span>

<span data-ttu-id="91176-119">カスタム ラーニング を Office 365設定するには、customlearning.sppkg ファイルをテナント全体のアプリ カタログにアップロードして展開します。</span><span class="sxs-lookup"><span data-stu-id="91176-119">To set up Custom Learning for Office 365, you upload the customlearning.sppkg file to the tenant-wide App Catalog and deploy it.</span></span> <span data-ttu-id="91176-120">アプリ[カタログにアプリを](/sharepoint/use-app-catalog)追加する方法の詳細については、「アプリ カタログを使用して、SharePoint Online 環境でカスタム ビジネス アプリを使用する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91176-120">See [Use the App Catalog to make custom business apps available for your SharePoint Online environment](/sharepoint/use-app-catalog) for detailed instructions on how to add an app to the app catalog.</span></span>

## <a name="provisionidentify-modern-communication-site"></a><span data-ttu-id="91176-121">モダン コミュニケーション サイトのプロビジョニング/識別</span><span class="sxs-lookup"><span data-stu-id="91176-121">Provision/Identify Modern Communication Site</span></span>

<span data-ttu-id="91176-122">既存の通信サイトをSharePointするか、オンライン テナントに新しい通信サイトをSharePointします。</span><span class="sxs-lookup"><span data-stu-id="91176-122">Either identify an existing SharePoint communication site or provision a new one in your SharePoint Online tenant.</span></span> <span data-ttu-id="91176-123">通信サイトを準備する方法の詳細については[、「SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)で通信サイトを作成する」を参照し、手順に従って通信サイトを作成します。</span><span class="sxs-lookup"><span data-stu-id="91176-123">For more information about how to provision a communication site, see [Create a communication site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) and follow the steps to create a communication site.</span></span>

## <a name="set-permissions-for-the-site"></a><span data-ttu-id="91176-124">サイトのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="91176-124">Set permissions for the site</span></span>

<span data-ttu-id="91176-125">コンテンツを表示できる必要があるすべてのユーザーを Visitors グループに追加し、カスタムプレイリストをメンバー グループに管理できる必要があるすべてのユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="91176-125">You will want to add everyone who should be able to view content to the Visitors group and everyone who should be able to administer custom playlists to the Members group.</span></span> <span data-ttu-id="91176-126">ユーザーが初めてサイト コレクション管理者または所有者グループの一部である必要がある場合は、カスタム学習用にサイトを構成します。</span><span class="sxs-lookup"><span data-stu-id="91176-126">To configure the site for Custom Learning the first time the user must be either a site collection administrator or part of the Owners group.</span></span>

<span data-ttu-id="91176-127">アプリのカスタム学習Office 365サイト コレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="91176-127">Add Custom Learning for Office 365 App to the site collection.</span></span>

## <a name="execute-powershell-configuration-script"></a><span data-ttu-id="91176-128">PowerShell 構成スクリプトの実行</span><span class="sxs-lookup"><span data-stu-id="91176-128">Execute PowerShell Configuration Script</span></span>

<span data-ttu-id="91176-129">PowerShell スクリプトが含まれているので、ソリューションで使用する 3 つのテナント プロパティを作成するために実行 `CustomLearningConfiguration.ps1` する必要があります。 [](/sharepoint/dev/spfx/tenant-properties)</span><span class="sxs-lookup"><span data-stu-id="91176-129">A PowerShell script `CustomLearningConfiguration.ps1` is included that you will need to execute to create three [tenant properties](/sharepoint/dev/spfx/tenant-properties) that the solution uses.</span></span> <span data-ttu-id="91176-130">さらに、このスクリプトはサイト ページ[](/sharepoint/dev/spfx/web-parts/single-part-app-pages)ライブラリに 2 つの単一パーツ アプリ ページを作成し、管理者とユーザーの Web パーツを既知の場所でホストします。</span><span class="sxs-lookup"><span data-stu-id="91176-130">In addition, the script creates two [single part app pages](/sharepoint/dev/spfx/web-parts/single-part-app-pages) in the site pages library to host the admin and user web parts at a known location.</span></span>

### <a name="disabling-telemetry-collection"></a><span data-ttu-id="91176-131">テレメトリ コレクションの無効化</span><span class="sxs-lookup"><span data-stu-id="91176-131">Disabling Telemetry Collection</span></span>

<span data-ttu-id="91176-132">このソリューションの一部には、匿名化されたテレメトリ追跡オプトインが含まれます。既定ではオンに設定されています。</span><span class="sxs-lookup"><span data-stu-id="91176-132">Part of this solution includes anonymized telemetry tracking opt-in, which by default is set to on.</span></span> <span data-ttu-id="91176-133">手動インストールを実行し、テレメトリ追跡をオフにする場合は、スクリプトを変更して、$optInTelemetry 変数を $false `CustomlearningConfiguration.ps1` に設定します。</span><span class="sxs-lookup"><span data-stu-id="91176-133">If you are performing a manual install and you would like to turn telemetry tracking off, change the `CustomlearningConfiguration.ps1` script to set the $optInTelemetry variable to $false.</span></span>

<span data-ttu-id="91176-134">手動インストールを実行していない場合にテレメトリ追跡をオフにする場合は、実行時にテレメトリ追跡が無効にされる別のスクリプト `TelemetryOptOut.ps1` が含まれています。</span><span class="sxs-lookup"><span data-stu-id="91176-134">If you are not performing a manual install and would like to turn telemetry tracking off, a separate script `TelemetryOptOut.ps1` has been included that when run will disable telemetry tracking.</span></span>

## <a name="initialize-web-part-custom-configuration"></a><span data-ttu-id="91176-135">Web パーツのカスタム構成を初期化する</span><span class="sxs-lookup"><span data-stu-id="91176-135">Initialize web part custom configuration</span></span>

<span data-ttu-id="91176-136">PowerShell スクリプトが正常に実行された後、に移動します `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 。</span><span class="sxs-lookup"><span data-stu-id="91176-136">After the PowerShell script is successfully run, navigate to `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="91176-137">これにより、初めて使用するカスタム学習を設定する CustomConfig リスト アイテムが初期化されます。</span><span class="sxs-lookup"><span data-stu-id="91176-137">This initializes the CustomConfig list item that sets up custom learning for its first use.</span></span>

<span data-ttu-id="91176-138">これで構成が完了し、ユーザー設定にカスタム 学習を使用Office 365。</span><span class="sxs-lookup"><span data-stu-id="91176-138">The configuration is now complete and you can move forward with using Custom Learning for Office 365.</span></span> <span data-ttu-id="91176-139">詳細については、ユーザーのドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="91176-139">See the user documentation for more information.</span></span>
