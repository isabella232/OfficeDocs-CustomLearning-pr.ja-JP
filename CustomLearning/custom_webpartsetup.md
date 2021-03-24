---
author: pkrebs
ms.author: pkrebs
title: カスタム学習サイトのプロビジョニング
ms.date: 02/10/2019
description: SharePoint プロビジョニング エンジンを使用Office 365 サイトのカスタム 学習のプロビジョニング
ms.service: sharepoint online
ms.openlocfilehash: be45ade7588f08801062710d310ca967ddd23926
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162924"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="24b14-103">カスタム 学習の準備</span><span class="sxs-lookup"><span data-stu-id="24b14-103">Provision Custom Learning</span></span>

<span data-ttu-id="24b14-104">SharePoint Online Provisioning Service を使用すると、Office 365 テナント管理者は、数回クリックしてプロビジョニング プロセスを開始できます。</span><span class="sxs-lookup"><span data-stu-id="24b14-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="24b14-105">プロビジョニング サービスは、カスタム 学習をプロビジョニングするための推奨される方法です。</span><span class="sxs-lookup"><span data-stu-id="24b14-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="24b14-106">高速で簡単で、プロセスを開始するのに数分しかかからなくなっています。</span><span class="sxs-lookup"><span data-stu-id="24b14-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="24b14-107">ただし、プロビジョニング サービスの使用を開始する前に、プロビジョニングの前提条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="24b14-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24b14-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="24b14-108">Prerequisites</span></span>
 
<span data-ttu-id="24b14-109">プロビジョニング サービス [SharePoint Online](https://provisioning.sharepointpnp.com)プロビジョニング サービスを使用してカスタム 学習を正常にセットアップするには、プロビジョニングを行うユーザーが次の前提条件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-109">To successfully set up Custom Learning with the Provisioning Service [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com), the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="24b14-110">カスタム 学習をプロビジョニングするユーザーは、カスタム学習が準備されるテナントのテナント管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-110">The person provisioning Custom Learning must be a Tenant Administratorof the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="24b14-111">テナント アプリ カタログは、SharePoint 管理センターの [アプリ] オプション内で使用できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="24b14-112">組織に SharePoint テナント アプリ カタログが存在しない場合は [、SharePoint Online](/sharepoint/use-app-catalog) のドキュメントを参照して作成します。</span><span class="sxs-lookup"><span data-stu-id="24b14-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="24b14-113">カスタム 学習をプロビジョニングするユーザーは、テナント アプリ カタログのサイト コレクション所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="24b14-114">カスタム 学習をプロビジョニングするユーザーがアプリ カタログのサイト コレクション所有者ではない場合は、次の [手順を実行](addappadmin.md) して続行します。</span><span class="sxs-lookup"><span data-stu-id="24b14-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="24b14-115">カスタム 学習を準備するには</span><span class="sxs-lookup"><span data-stu-id="24b14-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="24b14-116">ホーム ページ http://provisioning.sharepointpnp.com の **右上隅** から移動してサインインします。</span><span class="sxs-lookup"><span data-stu-id="24b14-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="24b14-117">サイト テンプレートのインストールを計画している対象テナントの資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="24b14-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome.png](media/inst_signin.png)

2. <span data-ttu-id="24b14-119">組織の代理 **として [同意] をオフにし、[** 同意する] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="24b14-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![ 内](media/inst_perms.png)

3. <span data-ttu-id="24b14-121">ソリューション **ギャラリーから [カスタム Office 365]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="24b14-121">Select **Custom Learning for Office 365** from the solution gallery.</span></span>

![ 内](media/inst_select.png)

4. <span data-ttu-id="24b14-123">ソリューションのホーム ページで、[ **テナントに追加] を選択します。**</span><span class="sxs-lookup"><span data-stu-id="24b14-123">From the solution home page select **Add to your Tenant**</span></span>

![inst_select.png](media/inst_add.png)

5. <span data-ttu-id="24b14-125">インストールに応じて、プロビジョニング情報ページのフィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="24b14-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="24b14-126">少なくとも、プロビジョニング プロセスに関する通知を受け取る電子メール アドレスと、プロビジョニング先サイトの宛先 URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="24b14-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="24b14-127">"/sites/MyTraining" や "/teams/LearnOffice365" など、サイトのリンク先 URL を従業員に優しくします。</span><span class="sxs-lookup"><span data-stu-id="24b14-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="24b14-129">テナント環境 **にカスタム** 学習をインストールする準備ができたら、[プロビジョニング] を選択します。</span><span class="sxs-lookup"><span data-stu-id="24b14-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="24b14-130">プロビジョニングプロセスには最大15分かかります。</span><span class="sxs-lookup"><span data-stu-id="24b14-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="24b14-131">サイトにアクセスできるようになると、（プロビジョニングページで入力した通知メールアドレスに）メールで通知されます。</span><span class="sxs-lookup"><span data-stu-id="24b14-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="24b14-132">カスタム 学習サイトをプロビジョニングするテナント管理者は、サイトに移動し、CustomLearningAdmin.aspx を開いてカスタム学習管理者プロパティを初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open CustomLearningAdmin.aspx to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="24b14-133">この時点で、テナント管理者はサイトに所有者も割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success"></a><span data-ttu-id="24b14-134">プロビジョニングの成功を検証する</span><span class="sxs-lookup"><span data-stu-id="24b14-134">Validate Provisioning Success</span></span>

<span data-ttu-id="24b14-135">プロビジョニングが完了すると、テナント管理者は PnP プロビジョニング サービスから電子メールを受信します。</span><span class="sxs-lookup"><span data-stu-id="24b14-135">When provisioning is complete, the Tenant Admin receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="24b14-136">管理者は、電子メールで提供されているサイトへのリンクをコピーし、指示に従ってサイトに移動できます。</span><span class="sxs-lookup"><span data-stu-id="24b14-136">The admin can copy the link to the site provided in the email, and then follow the instructions to go to the site.</span></span> <span data-ttu-id="24b14-137">または、テナント管理者は、/SitePages/CustomLearningAdmin.aspx <YOUR-SITE-COLLECTION-URL>に移動できます。</span><span class="sxs-lookup"><span data-stu-id="24b14-137">Alternately, the tenant admin can navigate to <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx.</span></span> <span data-ttu-id="24b14-138">これにより、初めて使用するカスタム学習を設定する CustomConfig リスト アイテムが初期化されます。</span><span class="sxs-lookup"><span data-stu-id="24b14-138">This initializes the CustomConfig list item that sets up Custom Learning for its first use.</span></span> <span data-ttu-id="24b14-139">このページを最初に開くユーザーは、テナント管理者、サイト コレクション管理者、またはサイトの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-139">The person who first opens this page must be a Tenant Admin,Site Collection Admin, or Owner of the site.</span></span> <span data-ttu-id="24b14-140">次のようなページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="24b14-140">You should see a page that looks like this:</span></span> 

## <a name="add-owners-to-site"></a><span data-ttu-id="24b14-141">サイトに所有者を追加する</span><span class="sxs-lookup"><span data-stu-id="24b14-141">Add Owners to Site</span></span>
<span data-ttu-id="24b14-142">テナント管理者として、サイトをカスタマイズするユーザーになる可能性は低いので、所有者をサイトに割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="24b14-142">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign Owners to the site.</span></span> <span data-ttu-id="24b14-143">所有者はサイトに対する管理者権限を持ち、サイト ページを変更したり、サイトのブランドを変更したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="24b14-143">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="24b14-144">また、カスタム学習 Web パーツを通じて配信されたコンテンツを非表示にし、表示する機能も備っています。</span><span class="sxs-lookup"><span data-stu-id="24b14-144">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="24b14-145">また、カスタム プレイリストを作成し、カスタム サブカテゴリに割り当てる機能も備えます。</span><span class="sxs-lookup"><span data-stu-id="24b14-145">They'll also have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="24b14-146">[SharePoint の設定] **メニューの** [サイトのアクセス許可 **] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="24b14-146">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="24b14-147">[アクセス **許可の詳細設定] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="24b14-147">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="24b14-148">**[365 所有者のカスタムOffice] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="24b14-148">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="24b14-149">[**新しい**  >  **ユーザーをこのグループに追加** する] をクリックし、所有者になるユーザーを追加し、[共有] を **クリックします**。</span><span class="sxs-lookup"><span data-stu-id="24b14-149">Click **New** > **Add Users to this group**, add the people you want to be Owners, and then click **Share**.</span></span>

8. <span data-ttu-id="24b14-150">ページの **右上隅にある** [次へ] オプションをクリックして、サイトをフォローします。</span><span class="sxs-lookup"><span data-stu-id="24b14-150">Click the **Following** option in the upper right hand corner of the page to follow the site.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="24b14-151">次の手順</span><span class="sxs-lookup"><span data-stu-id="24b14-151">Next Steps</span></span>
- <span data-ttu-id="24b14-152">Web パーツ [に含まれる既定](sitecontent.md) のコンテンツを確認します。</span><span class="sxs-lookup"><span data-stu-id="24b14-152">Explore the [default content](sitecontent.md) included in the webpart.</span></span>