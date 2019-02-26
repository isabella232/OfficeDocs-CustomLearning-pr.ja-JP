---
author: karuanag
ms.author: karuanag
title: カスタム学習サイトをプロビジョニングする
ms.date: 02/10/2019
description: SharePoint プロビジョニングエンジンを使用して Office 365 サイト用のカスタム学習をプロビジョニングする
ms.openlocfilehash: e87fdcbc5bbe9b23937403d8c49a7446b7159dff
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989668"
---
# <a name="provision-the-custom-learning-site"></a><span data-ttu-id="94cff-103">カスタム学習サイトをプロビジョニングする</span><span class="sxs-lookup"><span data-stu-id="94cff-103">Provision the Custom Learning Site</span></span>

1. <span data-ttu-id="94cff-p101">にhttp://provisioning.sharepointpnp.com移動して、ホームページの右上隅から**サインイン**します。 サイトテンプレートをインストールする予定の対象となるテナントの資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="94cff-p101">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.  Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome](media/inst_signin.png)

2. <span data-ttu-id="94cff-107">**組織の代わりに同意**をクリアし、[**同意**する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="94cff-107">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![順番](media/inst_perms.png)

3. <span data-ttu-id="94cff-109">ソリューションギャラリーから [ **Office 365 のカスタム学習**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="94cff-109">Select **Custom Learning for Office 365** from the solution gallery.</span></span>

![順番](media/inst_select.png)

4. <span data-ttu-id="94cff-111">ソリューションのホームページで、[**テナントに追加する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="94cff-111">From the solution home page select **Add to your Tenant**</span></span>

![inst_select](media/inst_add.png)

5. <span data-ttu-id="94cff-p102">ご使用のインストールに応じて、[プロビジョニング情報] ページのフィールドを入力します。少なくとも、プロビジョニングプロセスに関する通知を取得する電子メールアドレスと、サイトをプロビジョニングする宛先の URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="94cff-p102">Complete the fields on the provisioning information page as appropriate for your installation. At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  

> [!NOTE]
> <span data-ttu-id="94cff-115">サイトの宛先 URL を、"/sites/MyTraining" や "/teams/LearnOffice365" などの従業員にとってわかりやすいものにします。</span><span class="sxs-lookup"><span data-stu-id="94cff-115">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options](media/inst_options.png)

6. <span data-ttu-id="94cff-p103">テナント\*\*\*\* 環境に CLO365 をインストールする準備ができたら、[準備] を選択します。 プロビジョニングプロセスには最大15分かかります。サイトがアクセスできる状態になると、メールによって ([プロビジョニング] ページで入力した通知の電子メールアドレスに) 通知されます。</span><span class="sxs-lookup"><span data-stu-id="94cff-p103">Select **Provision** when ready to install CLO365 into your tenant environment.  The provisioning process will take up to 15 minutes. You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span>

7. <span data-ttu-id="94cff-120">準備が完了したことが通知されたら、[プロビジョニング] ページで入力した宛先 URL を参照します。</span><span class="sxs-lookup"><span data-stu-id="94cff-120">When you have been notified that provisioning is complete browse to the destination URL you entered in the Provisioning page.</span></span>

8. <span data-ttu-id="94cff-121">右上隅にサイトをお気に入りに置いて、後で参照するために URL をブックマークにします。</span><span class="sxs-lookup"><span data-stu-id="94cff-121">Favorite the site in the upper right hand corner and bookmark the URL for future reference.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="94cff-122">次のステップ</span><span class="sxs-lookup"><span data-stu-id="94cff-122">Next Steps</span></span>
- <span data-ttu-id="94cff-123">webpart に含まれる[既定のコンテンツ](sitecontent.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="94cff-123">Explore the [default content](sitecontent.md) included in the webpart.</span></span>
- <span data-ttu-id="94cff-124">組織のトレーニング環境を[カスタマイズ](customization.md)します。</span><span class="sxs-lookup"><span data-stu-id="94cff-124">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="94cff-125">トレーニングソリューションの[導入を促進](driveadoption.md)します。</span><span class="sxs-lookup"><span data-stu-id="94cff-125">[Drive adoption](driveadoption.md) of your training solution.</span></span>
