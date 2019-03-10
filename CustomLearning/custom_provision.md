---
author: pkrebs
ms.author: pkrebs
title: カスタム学習サイトをプロビジョニングする
ms.date: 02/10/2019
description: SharePoint プロビジョニングエンジンを使用して Office 365 サイト用のカスタム学習をプロビジョニングする
ms.openlocfilehash: a11975c7df1af9d01e2ca323d41cb5be602a1248
ms.sourcegitcommit: c358dcc2d69cc3db8fd24a1011550edebe0721fe
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2019
ms.locfileid: "30518178"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="9e304-103">カスタム学習をプロビジョニングする</span><span class="sxs-lookup"><span data-stu-id="9e304-103">Provision Custom Learning</span></span>

<span data-ttu-id="9e304-104">SharePoint Online プロビジョニングサービスを使用すると、Office 365 テナント管理者は、いくつかの簡単なクリックでプロビジョニングプロセスを開始できます。</span><span class="sxs-lookup"><span data-stu-id="9e304-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="9e304-105">プロビジョニングサービスは、カスタム学習をプロビジョニングするために推奨される方法です。</span><span class="sxs-lookup"><span data-stu-id="9e304-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="9e304-106">処理を開始するには、短時間で簡単です。</span><span class="sxs-lookup"><span data-stu-id="9e304-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="9e304-107">ただし、プロビジョニングサービスを開始する前に、プロビジョニングの前提条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="9e304-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e304-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e304-108">Prerequisites</span></span>
 
<span data-ttu-id="9e304-109">プロビジョニングサービス[SharePoint Online プロビジョニングサービス](https://provisioning.sharepointpnp.com)を使用してカスタム学習を正常にセットアップするには、プロビジョニングを実行するユーザーが次の前提条件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-109">To successfully set up Custom Learning with the Provisioning Service [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com), the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="9e304-110">カスタム学習をプロビジョニングするユーザーは、カスタム学習をプロビジョニングするテナントのテナントのアドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-110">The person provisioning Custom Learning must be a Tenant Administratorof the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="9e304-111">テナントアプリカタログは、SharePoint 管理センターの [アプリ] オプションで使用できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="9e304-112">組織に sharepoint テナントのアプリカタログがない場合は、 [sharepoint Online のドキュメント](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)を参照して作成します。</span><span class="sxs-lookup"><span data-stu-id="9e304-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="9e304-113">カスタム学習をプロビジョニングするユーザーは、テナントアプリカタログのサイトコレクションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="9e304-114">ユーザーのカスタム学習が、アプリカタログのサイトコレクションの所有者ではない場合は、[次の手順を完了](addappadmin.md)して続行します。</span><span class="sxs-lookup"><span data-stu-id="9e304-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="9e304-115">カスタム学習をプロビジョニングするには</span><span class="sxs-lookup"><span data-stu-id="9e304-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="9e304-116">にhttp://provisioning.sharepointpnp.com移動して、ホームページの右上隅から**サインイン**します。</span><span class="sxs-lookup"><span data-stu-id="9e304-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="9e304-117">サイトテンプレートをインストールする予定の対象となるテナントの資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="9e304-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome](media/inst_signin.png)

2. <span data-ttu-id="9e304-119">**組織の代わりに同意**をクリアし、[**同意**する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9e304-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![順番](media/inst_perms.png)

3. <span data-ttu-id="9e304-121">ソリューションギャラリーから [ **Office 365 のカスタム学習**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9e304-121">Select **Custom Learning for Office 365** from the solution gallery.</span></span>

![順番](media/inst_select.png)

4. <span data-ttu-id="9e304-123">ソリューションのホームページで、[**テナントに追加する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9e304-123">From the solution home page select **Add to your Tenant**</span></span>

![inst_select](media/inst_add.png)

5. <span data-ttu-id="9e304-125">ご使用のインストールに応じて、[プロビジョニング情報] ページのフィールドを入力します。</span><span class="sxs-lookup"><span data-stu-id="9e304-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="9e304-126">少なくとも、プロビジョニングプロセスに関する通知を取得する電子メールアドレスと、サイトをプロビジョニングする宛先の URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="9e304-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="9e304-127">サイトの宛先 URL を、"/sites/MyTraining" や "/teams/LearnOffice365" などの従業員にとってわかりやすいものにします。</span><span class="sxs-lookup"><span data-stu-id="9e304-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options](media/inst_options.png)

6. <span data-ttu-id="9e304-129">カスタム\*\*\*\* 学習をテナント環境にインストールする準備ができたら、[準備] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9e304-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="9e304-130">プロビジョニングプロセスには最大15分かかります。</span><span class="sxs-lookup"><span data-stu-id="9e304-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="9e304-131">サイトがアクセスできる状態になると、メールによって ([プロビジョニング] ページで入力した通知の電子メールアドレスに) 通知されます。</span><span class="sxs-lookup"><span data-stu-id="9e304-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="9e304-132">カスタム学習サイトをプロビジョニングするテナント管理者は、サイトに移動し、CustomLearningAdmin を開いてカスタム学習管理プロパティを初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open CustomLearningAdmin.aspx to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="9e304-133">この時点で、テナント管理者はサイトに所有者を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success"></a><span data-ttu-id="9e304-134">プロビジョニングが成功したことを検証する</span><span class="sxs-lookup"><span data-stu-id="9e304-134">Validate Provisioning Success</span></span>

<span data-ttu-id="9e304-135">プロビジョニングが完了すると、テナント管理者は PnP プロビジョニングサービスから電子メールを受信します。</span><span class="sxs-lookup"><span data-stu-id="9e304-135">When provisioning is complete, the Tenant Admin receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="9e304-136">管理者は、電子メールで提供されているサイトへのリンクをコピーして、指示に従ってサイトに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="9e304-136">The admin can copy the link to the site provided in the email, and then follow the instructions to go to the site.</span></span> <span data-ttu-id="9e304-137">または、テナント管理者は <YOUR-SITE-COLLECTION-URL>/sitepages/CustomLearningAdmin に移動できます。</span><span class="sxs-lookup"><span data-stu-id="9e304-137">Alternately, the tenant admin can navigate to <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx.</span></span> <span data-ttu-id="9e304-138">これにより、最初に使用するカスタム学習を設定する customconfig リストアイテムが初期化されます。</span><span class="sxs-lookup"><span data-stu-id="9e304-138">This initializes the CustomConfig list item that sets up Custom Learning for its first use.</span></span> <span data-ttu-id="9e304-139">このページを最初に開いたユーザーは、テナント管理者、サイトコレクション管理者、またはサイトの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-139">The person who first opens this page must be a Tenant Admin,Site Collection Admin, or Owner of the site.</span></span> <span data-ttu-id="9e304-140">次のようなページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="9e304-140">You should see a page that looks like this:</span></span> 

## <a name="add-owners-to-site"></a><span data-ttu-id="9e304-141">サイトに所有者を追加する</span><span class="sxs-lookup"><span data-stu-id="9e304-141">Add Owners to Site</span></span>
<span data-ttu-id="9e304-142">テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトに所有者を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e304-142">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign Owners to the site.</span></span> <span data-ttu-id="9e304-143">所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。</span><span class="sxs-lookup"><span data-stu-id="9e304-143">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="9e304-144">また、カスタム学習 Web パーツを通じて配信されるコンテンツを非表示にしたり、表示したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="9e304-144">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="9e304-145">また、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="9e304-145">They'll also have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="9e304-146">[SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9e304-146">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="9e304-147">[**高度なアクセス許可の設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9e304-147">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="9e304-148">[ **Office 365 所有者向けのカスタム学習] を**クリックします。</span><span class="sxs-lookup"><span data-stu-id="9e304-148">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="9e304-149">[**新しい** > **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加して、[**共有**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9e304-149">Click **New** > **Add Users to this group**, add the people you want to be Owners, and then click **Share**.</span></span>

8. <span data-ttu-id="9e304-150">ページの右上隅にある**次**のオプションをクリックして、サイトをフォローします。</span><span class="sxs-lookup"><span data-stu-id="9e304-150">Click the **Following** option in the upper right hand corner of the page to follow the site.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="9e304-151">次のステップ</span><span class="sxs-lookup"><span data-stu-id="9e304-151">Next Steps</span></span>
- <span data-ttu-id="9e304-152">webpart に含まれる[既定のコンテンツ](sitecontent.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e304-152">Explore the [default content](sitecontent.md) included in the webpart.</span></span>
