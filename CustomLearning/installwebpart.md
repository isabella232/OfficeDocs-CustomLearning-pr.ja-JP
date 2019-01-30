# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="fe22a-101">学習ソリューションの web パーツ、カスタムのインストール</span><span class="sxs-lookup"><span data-stu-id="fe22a-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="fe22a-102">テナント全体のインストールの前提条件</span><span class="sxs-lookup"><span data-stu-id="fe22a-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="fe22a-p101">全体のテナントの学習のカスタム web パーツをインストールするのには、Office 365 の管理者権限を持っている必要があります。 場合は、Office 365 の管理者で作業するか、個々 のサイト コレクションの web パーツをインストールするには、これらのアクセス許可がありません。</span><span class="sxs-lookup"><span data-stu-id="fe22a-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="fe22a-105">か、Office 365 の管理者のセットアップが必要し、テナント全体にわたる[アプリケーションのカタログ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)または[サイト コレクションのアプリケーション カタログ](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)は、web パーツが表示されるように構成します。]</span><span class="sxs-lookup"><span data-stu-id="fe22a-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="fe22a-p102">SharePoint Online 機能だけをサポートします。Web パーツは、社内設置型の SharePoint のすべてのバージョンにインストールするためのサポートではありません。</span><span class="sxs-lookup"><span data-stu-id="fe22a-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="fe22a-108">テナントに学習のカスタム web パーツを追加します。</span><span class="sxs-lookup"><span data-stu-id="fe22a-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="fe22a-p103">学習のカスタム web パーツをダウンロードし、ローカル ドライブに保存します。 このファイルを「ms ・ カスタム ・ learning.sppkg」といいます。 名またはファイルのサフィックスは変更されません。</span><span class="sxs-lookup"><span data-stu-id="fe22a-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="fe22a-112">テナントの[Office 365 管理ポータル](https://admin.microsoft.com/AdminPortal/Home#/homepage)に移動します。</span><span class="sxs-lookup"><span data-stu-id="fe22a-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="fe22a-p104">左側のナビゲーションから、管理センターでは、SharePoint を選択します。SharePoint 管理センターで [アプリケーション、アプリケーションのカタログ、SharePoint のアプリケーション、新しいタブに表示されます。</span><span class="sxs-lookup"><span data-stu-id="fe22a-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="fe22a-115">選択は、web パーツをアップロードするファイルを選択して「ms ・ カスタム ・ learning.sppkg」をダウンロードしました。</span><span class="sxs-lookup"><span data-stu-id="fe22a-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="fe22a-116">テナント全体のインストール] チェック ボックス」にこのソリューションを組織内のすべての位置を使用」</span><span class="sxs-lookup"><span data-stu-id="fe22a-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![ソリューションを導入します。](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="fe22a-118">お客様のラーニングの web パーツを SharePoint オンライン ページに追加します。</span><span class="sxs-lookup"><span data-stu-id="fe22a-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="fe22a-p105">カスタムの学習は、テナントのインストール後は、SharePoint ページに Web パーツを追加できます。実行すると、突然 Office 365 のトレーニングが利用できます。</span><span class="sxs-lookup"><span data-stu-id="fe22a-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="fe22a-121">全体の幅の列のレイアウトでは、学習のカスタム web パーツを追加します。</span><span class="sxs-lookup"><span data-stu-id="fe22a-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint ページのレイアウト](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="fe22a-p106">SharePoint ページでの追加」を選択して全体の幅の列を選択し。 次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fe22a-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="fe22a-p107">Microsoft ラーニングを選択します。 次が今すぐ表示されます。</span><span class="sxs-lookup"><span data-stu-id="fe22a-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![カスタムの web パーツを学習します。](media/clo365addwebpart.png)

 <span data-ttu-id="fe22a-129">ソリューションに含まれている既定のコンテンツを表示するタイルをクリックします。</span><span class="sxs-lookup"><span data-stu-id="fe22a-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="fe22a-130">次のステップ</span><span class="sxs-lookup"><span data-stu-id="fe22a-130">Next Steps</span></span>
- <span data-ttu-id="fe22a-131">Web パーツに含まれる[既定のコンテンツ](webpartcontent.md)を表示します。</span><span class="sxs-lookup"><span data-stu-id="fe22a-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="fe22a-132">[ユーザー設定](customization.md)、組織のトレーニング経験します。</span><span class="sxs-lookup"><span data-stu-id="fe22a-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="fe22a-133">トレーニング ソリューションの[採用を推進](driveadoption.md)をします。</span><span class="sxs-lookup"><span data-stu-id="fe22a-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

