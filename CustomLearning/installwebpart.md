---
author: karuanag
ms.author: karuanag
title: カスタム学習ソリューション web パーツのインストール
ms.date: 02/10/2019
description: カスタム学習ソリューション web パーツのインストール手順
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989688"
---
# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="5e417-103">カスタム学習ソリューション web パーツのインストール</span><span class="sxs-lookup"><span data-stu-id="5e417-103">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="5e417-104">テナント全体へのインストールの前提条件</span><span class="sxs-lookup"><span data-stu-id="5e417-104">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="5e417-p101">テナント全体にカスタム学習 web パーツをインストールするには、Office 365 の管理アクセス許可を持っている必要があります。 これらのアクセス許可がない場合は、Office 365 管理者と連携するか、または個々のサイトコレクションの web パーツをインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="5e417-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="5e417-107">ユーザーまたは Office 365 管理者は、web パーツを受信するために、テナント全体の[アプリカタログ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)または[サイトコレクションのアプリカタログ](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)をセットアップして構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e417-107">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="5e417-p102">SharePoint Online のみをサポートしています。web パーツは、オンプレミスの SharePoint の任意のバージョンへのインストールをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="5e417-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="5e417-110">テナントにカスタム学習 web パーツを追加する</span><span class="sxs-lookup"><span data-stu-id="5e417-110">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="5e417-p103">カスタム学習 web パーツをダウンロードして、ローカルドライブに保存します。 このファイルの名前は "ms-カスタム-learning. sppkg" です。 ファイルの名前やサフィックスを変更しないでください。</span><span class="sxs-lookup"><span data-stu-id="5e417-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="5e417-114">テナントの[Office 365 管理ポータル](https://admin.microsoft.com/AdminPortal/Home#/homepage)に移動します。</span><span class="sxs-lookup"><span data-stu-id="5e417-114">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="5e417-p104">左側のナビゲーションで、[管理センター]、[SharePoint] のどちらかを選択します。これは、新しいタブに表示されます。の sharepoint 管理センターで、[アプリ]、[アプリカタログ]、[sharepoint 用アプリ] の順番でクリックします。</span><span class="sxs-lookup"><span data-stu-id="5e417-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="5e417-117">[web パーツのアップロード] を選択し、ダウンロードした「ms (カスタム-learning) ファイル」を選択します。</span><span class="sxs-lookup"><span data-stu-id="5e417-117">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="5e417-118">このテナント全体のインストールの場合は、[組織内のすべてのソリューションでこのソリューションを使用できるようにする] の横にあるチェックボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="5e417-118">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  
 
> [!NOTE]
> <span data-ttu-id="5e417-p105">web パーツがインストールされると、SharePoint Online の webpart ギャラリーに表示されます。 **ギャラリー内の webpart には、「Microsoft Learning」という名前が付けられます**。</span><span class="sxs-lookup"><span data-stu-id="5e417-p105">Once the webpart is installed you will find it in your webpart gallery in SharePoint Online.  **In the gallery the webpart is named "Microsoft Learning"**</span></span>

![ソリューションを展開する](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="5e417-122">Microsoft Learning webpart を SharePoint Online ページに追加する</span><span class="sxs-lookup"><span data-stu-id="5e417-122">Add the Microsoft Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="5e417-p106">テナントにカスタム学習をインストールした後、Web パーツを SharePoint ページに追加することができます。Office 365 を実行すると、サイトで Windows 10 のトレーニングを利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="5e417-p106">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do Office 365 and Windows 10 training is available to your site.</span></span>

1. <span data-ttu-id="5e417-125">[全幅] 列レイアウトにカスタム学習 web パーツを追加します。</span><span class="sxs-lookup"><span data-stu-id="5e417-125">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint ページレイアウト](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="5e417-p107">SharePoint ページで、[セクションの追加] を選択し、[全角列] を選択します。 次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e417-p107">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![addwebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="5e417-p108">[Microsoft Learning] を選択します。 次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e417-p108">Select Microsoft Learning.  You should now see the following:</span></span> 

![カスタム学習 web パーツ](media/clo365addwebpart.png)

 <span data-ttu-id="5e417-133">タイルをクリックして、ソリューションに含まれる既定のコンテンツを調べることができるようになります。</span><span class="sxs-lookup"><span data-stu-id="5e417-133">You can now click on the tiles to explore the default content included in the solution.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="5e417-134">次のステップ</span><span class="sxs-lookup"><span data-stu-id="5e417-134">Next Steps</span></span>
- <span data-ttu-id="5e417-135">webpart に含まれる[既定のコンテンツ](webpartcontent.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="5e417-135">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="5e417-136">組織のトレーニング環境を[カスタマイズ](customization.md)します。</span><span class="sxs-lookup"><span data-stu-id="5e417-136">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="5e417-137">トレーニングソリューションの[導入を促進](driveadoption.md)します。</span><span class="sxs-lookup"><span data-stu-id="5e417-137">[Drive adoption](driveadoption.md) of your training solution.</span></span>

