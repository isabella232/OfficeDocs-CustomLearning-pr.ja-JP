---
author: pkrebs
ms.author: pkrebs
title: カスタム学習サイトをプロビジョニングする
ms.date: 02/10/2019
description: SharePoint プロビジョニングエンジンを使用して Office 365 サイト用のカスタム学習をプロビジョニングする
ms.openlocfilehash: 868708f9f096c84d5ebc5f9bc4e21e558da84d2b
ms.sourcegitcommit: 5ea8d7fdc255ef7de06f41b3c794bc40551cf5bb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30577863"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="81ad4-103">カスタム学習をプロビジョニングする</span><span class="sxs-lookup"><span data-stu-id="81ad4-103">Provision Custom Learning</span></span> 

<span data-ttu-id="81ad4-104">SharePoint Online プロビジョニングサービスを使用すると、Office 365 テナント管理者は、いくつかの簡単なクリックでプロビジョニングプロセスを開始できます。</span><span class="sxs-lookup"><span data-stu-id="81ad4-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="81ad4-105">プロビジョニングサービスは、カスタム学習をプロビジョニングするために推奨される方法です。</span><span class="sxs-lookup"><span data-stu-id="81ad4-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="81ad4-106">処理を開始するには、短時間で簡単です。</span><span class="sxs-lookup"><span data-stu-id="81ad4-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="81ad4-107">ただし、プロビジョニングサービスを開始する前に、プロビジョニングの前提条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="81ad4-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81ad4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="81ad4-108">Prerequisites</span></span>
 
<span data-ttu-id="81ad4-109">プロビジョニングサービスを使用してカスタム学習を正常にセットアップするには、プロビジョニングを実行するユーザーが次の前提条件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-109">To successfully set up Custom Learning with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="81ad4-110">カスタム学習をプロビジョニングするユーザーは、カスタム学習をプロビジョニングするテナントのテナント管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-110">The person provisioning Custom Learning must be a Tenant Administrator of the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="81ad4-111">テナントアプリカタログは、SharePoint 管理センターの [アプリ] オプションで使用できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="81ad4-112">組織に sharepoint テナントのアプリカタログがない場合は、 [sharepoint Online のドキュメント](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)を参照して作成します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="81ad4-113">カスタム学習をプロビジョニングするユーザーは、テナントアプリカタログのサイトコレクションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="81ad4-114">ユーザーのカスタム学習が、アプリカタログのサイトコレクションの所有者ではない場合は、[次の手順を完了](addappadmin.md)して続行します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="81ad4-115">カスタム学習をプロビジョニングするには</span><span class="sxs-lookup"><span data-stu-id="81ad4-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="81ad4-116">にhttp://provisioning.sharepointpnp.com移動して、ホームページの右上隅から**サインイン**します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="81ad4-117">サイトテンプレートをインストールする予定の対象となるテナントの資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="81ad4-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome](media/inst_signin.png)

2. <span data-ttu-id="81ad4-119">**組織の代わりに同意**をクリアし、[**同意**する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![順番](media/inst_perms.png)

3. <span data-ttu-id="81ad4-121">ページを下にスクロールし、[**ソリューション**] タブを選択してから、[ **Office 365 のカスタム学習**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-121">Scroll down the page, select the **Solutions** tab, and then select **Custom learning for Office 365**.</span></span> 

![順番](media/inst_select.png)

4. <span data-ttu-id="81ad4-123">[**テナントに追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-123">Select **Add to your tenant**</span></span>

![inst_select](media/inst_add.png)

5. <span data-ttu-id="81ad4-125">ご使用のインストールに応じて、[プロビジョニング情報] ページのフィールドを入力します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="81ad4-126">少なくとも、プロビジョニングプロセスに関する通知を取得する電子メールアドレスと、サイトをプロビジョニングする宛先の URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="81ad4-127">サイトの宛先 URL を、"/sites/MyTraining" や "/teams/LearnOffice365" などの従業員にとってわかりやすいものにします。</span><span class="sxs-lookup"><span data-stu-id="81ad4-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options](media/inst_options.png)

6. <span data-ttu-id="81ad4-129">カスタム\*\*\*\* 学習をテナント環境にインストールする準備ができたら、[準備] を選択します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="81ad4-130">プロビジョニングプロセスには最大15分かかります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="81ad4-131">サイトがアクセスできる状態になると、メールによって ([プロビジョニング] ページで入力した通知の電子メールアドレスに) 通知されます。</span><span class="sxs-lookup"><span data-stu-id="81ad4-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="81ad4-132">カスタム学習サイトをプロビジョニングするテナント管理者は、サイトに移動し、 **CustomLearningAdmin**を開いてカスタム学習管理プロパティを初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="81ad4-133">この時点で、テナント管理者はサイトに所有者を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="81ad4-134">プロビジョニングが成功したことを検証し、customconfig リストを初期化する</span><span class="sxs-lookup"><span data-stu-id="81ad4-134">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="81ad4-135">プロビジョニングが完了すると、サイトをプロビジョニングしたテナント管理者が、PnP プロビジョニングサービスから電子メールを受信します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-135">When provisioning is complete, the Tenant Admin who provisioned the site, receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="81ad4-136">電子メールには、サイトへのリンクが含まれています。</span><span class="sxs-lookup"><span data-stu-id="81ad4-136">The email contains a link to the site.</span></span> <span data-ttu-id="81ad4-137">この時点で、テナント管理者は、電子メールで提供されているリンクを使用してサイトに移動し、最初に使用するサイトを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-137">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="81ad4-138">`<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx` に移動します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-138">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="81ad4-139">**CustomLearningAdmin**を開くと、カスタム学習を設定する**customconfig**リストアイテムが初期化されます。</span><span class="sxs-lookup"><span data-stu-id="81ad4-139">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up Custom Learning for first use.</span></span> <span data-ttu-id="81ad4-140">次のようなページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="81ad4-140">You should see a page that looks like this:</span></span>

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="81ad4-142">サイトに所有者を追加する</span><span class="sxs-lookup"><span data-stu-id="81ad4-142">Add Owners to Site</span></span>
<span data-ttu-id="81ad4-143">テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトにいくつかの所有者を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ad4-143">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="81ad4-144">所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。</span><span class="sxs-lookup"><span data-stu-id="81ad4-144">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="81ad4-145">また、カスタム学習 Web パーツを通じて配信されるコンテンツを非表示にしたり、表示したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="81ad4-145">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="81ad4-146">さらに、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="81ad4-146">In addition, they'll have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="81ad4-147">[SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="81ad4-147">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="81ad4-148">[**高度なアクセス許可の設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="81ad4-148">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="81ad4-149">[ **Office 365 所有者向けのカスタム学習] を**クリックします。</span><span class="sxs-lookup"><span data-stu-id="81ad4-149">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="81ad4-150">[**新しい** > **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-150">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="81ad4-151">共有メッセージ内の[サイトを探索](custom_exploresite.md)するためのリンクを追加し、[**共有**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="81ad4-151">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

### <a name="next-steps"></a><span data-ttu-id="81ad4-152">次のステップ</span><span class="sxs-lookup"><span data-stu-id="81ad4-152">Next Steps</span></span>
- <span data-ttu-id="81ad4-153">サイトと web パーツで提供される[既定のコンテンツ](custom_exploresite.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="81ad4-153">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
