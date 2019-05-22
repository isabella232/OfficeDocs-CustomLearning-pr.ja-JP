---
author: pkrebs
ms.author: pkrebs
title: マイクロソフトの365ラーニングパスサイトを準備する
ms.date: 02/10/2019
description: SharePoint プロビジョニングサービスを使用して Microsoft 365 learning の方法のサイトをプロビジョニングする
ms.openlocfilehash: e48052a395a8669ef684110a1c93409f5859a1d2
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334747"
---
# <a name="provision-microsoft-365-learning-pathways"></a><span data-ttu-id="829da-103">Microsoft 365 learning の経路をプロビジョニングする</span><span class="sxs-lookup"><span data-stu-id="829da-103">Provision Microsoft 365 learning pathways</span></span>

<span data-ttu-id="829da-104">SharePoint Online プロビジョニングサービスを使用すると、Office 365 テナント管理者は、いくつかの簡単なクリックでプロビジョニングプロセスを開始できます。</span><span class="sxs-lookup"><span data-stu-id="829da-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="829da-105">プロビジョニングサービスは、学習経路をプロビジョニングするために推奨される方法です。</span><span class="sxs-lookup"><span data-stu-id="829da-105">The Provisioning Service is the recommended way to provision learning pathways.</span></span> <span data-ttu-id="829da-106">処理を開始するには、短時間で簡単です。</span><span class="sxs-lookup"><span data-stu-id="829da-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="829da-107">ただし、プロビジョニングサービスを開始する前に、プロビジョニングの前提条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="829da-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="829da-108">5/21/2019 の間、Microsoft 365 learning の経路は、以前は Office 365 のカスタム学習と呼ばれていたソリューションの新しい名前です。</span><span class="sxs-lookup"><span data-stu-id="829da-108">As of 5/21/2019, Microsoft 365 learning pathways is the new name for the solution formerly known as Custom Learning for Office 365.</span></span> <span data-ttu-id="829da-109">組織内で Office 365 のカスタム学習機能を既にプロビジョニングしていて、ソリューションを更新する場合は、「 [Microsoft 365 Learning ・パスの ReadMe](https://github.com/pnp/custom-learning-office-365)」の「ソリューションを更新する」の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="829da-109">If you have already provisioned Custom Learning for Office 365 in your organization and want to update the solution, follow the “Updating the solution” instructions in the [Microsoft 365 learning pathways ReadMe](https://github.com/pnp/custom-learning-office-365).</span></span> <span data-ttu-id="829da-110">初めて Microsoft 365 learning の経路情報をプロビジョニングする場合は、「microsoft 365 learning の経路」のドキュメントの「 [microsoft 365 learning のラーニングをプロビジョニング]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision)する」の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="829da-110">If you are provisioning Microsoft 365 learning pathways for the first time, see [Provision Microsoft 365 learning pathways instructions]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) in the Microsoft 365 learning pathways documentation.</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="829da-111">前提条件</span><span class="sxs-lookup"><span data-stu-id="829da-111">Prerequisites</span></span>
 
<span data-ttu-id="829da-112">プロビジョニングサービスで Microsoft 365 learning の経路を正しく設定するには、プロビジョニングを実行するユーザーが次の前提条件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-112">To successfully set up Microsoft 365 learning pathways with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="829da-113">ユーザープロビジョニングの学習経路は、学習経路がプロビジョニングされるテナントのテナント管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-113">The person provisioning learning pathways must be a Tenant Administrator of the tenant where learning pathways will be provisioned.</span></span>  
- <span data-ttu-id="829da-114">テナントアプリカタログは、SharePoint 管理センターの [アプリ] オプションで使用できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-114">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="829da-115">組織に SharePoint テナントのアプリカタログがない場合は、 [Sharepoint Online のドキュメント](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)を参照して作成します。</span><span class="sxs-lookup"><span data-stu-id="829da-115">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="829da-116">ユーザープロビジョニングの学習経路は、テナントのアプリカタログのサイトコレクションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-116">The person provisioning learning pathways must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="829da-117">学習経路をプロビジョニングするユーザーがアプリカタログのサイトコレクションの所有者ではない場合は、[次の手順を実行](addappadmin.md)して続行します。</span><span class="sxs-lookup"><span data-stu-id="829da-117">If the person provisioning learning pathways is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-learning-pathways"></a><span data-ttu-id="829da-118">学習経路をプロビジョニングするには</span><span class="sxs-lookup"><span data-stu-id="829da-118">To provision learning pathways</span></span>

1. <span data-ttu-id="829da-119">にhttp://provisioning.sharepointpnp.com移動して、ホームページの右上隅から**サインイン**します。</span><span class="sxs-lookup"><span data-stu-id="829da-119">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="829da-120">サイトテンプレートをインストールする予定の対象となるテナントの資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="829da-120">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome](media/inst_signin.png)

2. <span data-ttu-id="829da-122">**組織の代わりに同意**をクリアし、[**同意**する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="829da-122">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![順番](media/inst_perms.png)

<span data-ttu-id="829da-124">プロビジョニングサービスには、テナントのアプリカタログを作成し、アプリケーションをテナントのアプリカタログにインストールし、サイトテンプレートをプロビジョニングするためのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="829da-124">The provisioning service requires these permissions to create the tenant app catalog, install the application into the tenant app catalog and provision the site template.</span></span> <span data-ttu-id="829da-125">テナントに全体的な影響がありません。これらのアクセス許可は、ソリューションのインストールの目的で明示的に使用されます。</span><span class="sxs-lookup"><span data-stu-id="829da-125">There is no overall impact on your tenant and these permissions are explicitly used for the purpose of the solution installation.</span></span> <span data-ttu-id="829da-126">インストールを続行するには、これらのアクセス許可を受け入れる必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-126">You must accept these permissions to proceed with the installation.</span></span>

3. <span data-ttu-id="829da-127">ページを下にスクロールし、[**ソリューション**] タブを選択してから、[ **Office 365 の学習経路**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="829da-127">Scroll down the page, select the **Solutions** tab, and then select **learning pathways for Office 365**.</span></span> 

![順番](media/inst_select.png)

4. <span data-ttu-id="829da-129">[**テナントに追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="829da-129">Select **Add to your tenant**</span></span>

![inst_select](media/inst_add.png)

5. <span data-ttu-id="829da-131">ご使用のインストールに応じて、[プロビジョニング情報] ページのフィールドを入力します。</span><span class="sxs-lookup"><span data-stu-id="829da-131">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="829da-132">少なくとも、プロビジョニングプロセスに関する通知を取得する電子メールアドレスと、サイトをプロビジョニングする宛先の URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="829da-132">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="829da-133">サイトの宛先 URL を、"/sites/MyTraining" や "/teams/LearnMicrosoft365" などの従業員にとってわかりやすいものにします。</span><span class="sxs-lookup"><span data-stu-id="829da-133">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnMicrosoft365".</span></span>

![inst_options](media/inst_options.png)

6. <span data-ttu-id="829da-135">テナント\*\*\*\* 環境に学習経路をインストールする準備ができたら、[準備] を選択します。</span><span class="sxs-lookup"><span data-stu-id="829da-135">Select **Provision** when ready to install learning pathways into your tenant environment.</span></span>  <span data-ttu-id="829da-136">プロビジョニングプロセスには最大15分かかります。</span><span class="sxs-lookup"><span data-stu-id="829da-136">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="829da-137">サイトがアクセスできる状態になると、メールによって ([プロビジョニング] ページで入力した通知の電子メールアドレスに) 通知されます。</span><span class="sxs-lookup"><span data-stu-id="829da-137">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="829da-138">ラーニングポイントサイトをプロビジョニングするテナント管理者は、サイトに移動し、 **CustomLearningAdmin**を開いて学習経路管理プロパティを初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-138">The Tenant Admin who provisions the learning pathways site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize learning pathways Admin properties.</span></span> <span data-ttu-id="829da-139">この時点で、テナント管理者はサイトに所有者を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-139">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="829da-140">プロビジョニングが成功したことを検証し、CustomConfig リストを初期化する</span><span class="sxs-lookup"><span data-stu-id="829da-140">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="829da-141">プロビジョニングが完了すると、サイトをプロビジョニングしたテナント管理者が、PnP プロビジョニングサービスから電子メールを受信します。</span><span class="sxs-lookup"><span data-stu-id="829da-141">When provisioning is complete, the Tenant Admin who provisioned the site, receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="829da-142">電子メールには、サイトへのリンクが含まれています。</span><span class="sxs-lookup"><span data-stu-id="829da-142">The email contains a link to the site.</span></span> <span data-ttu-id="829da-143">この時点で、テナント管理者は、電子メールで提供されているリンクを使用してサイトに移動し、最初に使用するサイトを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-143">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="829da-144">`<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx` に移動します。</span><span class="sxs-lookup"><span data-stu-id="829da-144">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="829da-145">**CustomLearningAdmin**を開くと、最初に使用するための学習経路を設定する**customconfig**リストアイテムが初期化されます。</span><span class="sxs-lookup"><span data-stu-id="829da-145">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up learning pathways for first use.</span></span> <span data-ttu-id="829da-146">次のようなページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="829da-146">You should see a page that looks like this:</span></span>

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="829da-148">サイトに所有者を追加する</span><span class="sxs-lookup"><span data-stu-id="829da-148">Add Owners to Site</span></span>
<span data-ttu-id="829da-149">テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトにいくつかの所有者を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="829da-149">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="829da-150">所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。</span><span class="sxs-lookup"><span data-stu-id="829da-150">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="829da-151">また、ラーニングパス Web パーツを通じて配信されるコンテンツを非表示にし、表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="829da-151">They also have the ability to hide and show content delivered through the learning pathways Web part.</span></span> <span data-ttu-id="829da-152">さらに、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="829da-152">In addition, they'll have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="829da-153">[SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="829da-153">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="829da-154">[**高度なアクセス許可の設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="829da-154">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="829da-155">[ **Microsoft 365 learning の経路の所有者**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="829da-155">Click **Microsoft 365 learning pathways Owners**.</span></span>
4. <span data-ttu-id="829da-156">[**新しい** > **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="829da-156">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="829da-157">共有メッセージ内の[サイトを探索](custom_exploresite.md)するためのリンクを追加し、[**共有**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="829da-157">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

### <a name="next-steps"></a><span data-ttu-id="829da-158">次のステップ</span><span class="sxs-lookup"><span data-stu-id="829da-158">Next Steps</span></span>
- <span data-ttu-id="829da-159">サイトと web パーツで提供される[既定のコンテンツ](custom_exploresite.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="829da-159">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
