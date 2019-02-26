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
# <a name="provision-the-custom-learning-site"></a>カスタム学習サイトをプロビジョニングする

1. にhttp://provisioning.sharepointpnp.com移動して、ホームページの右上隅から**サインイン**します。 サイトテンプレートをインストールする予定の対象となるテナントの資格情報を使用してサインインします。

![pnphome](media/inst_signin.png)

2. **組織の代わりに同意**をクリアし、[**同意**する] を選択します。

![順番](media/inst_perms.png)

3. ソリューションギャラリーから [ **Office 365 のカスタム学習**] を選択します。

![順番](media/inst_select.png)

4. ソリューションのホームページで、[**テナントに追加する**] を選択します。

![inst_select](media/inst_add.png)

5. ご使用のインストールに応じて、[プロビジョニング情報] ページのフィールドを入力します。少なくとも、プロビジョニングプロセスに関する通知を取得する電子メールアドレスと、サイトをプロビジョニングする宛先の URL を入力します。  

> [!NOTE]
> サイトの宛先 URL を、"/sites/MyTraining" や "/teams/LearnOffice365" などの従業員にとってわかりやすいものにします。

![inst_options](media/inst_options.png)

6. テナント**** 環境に CLO365 をインストールする準備ができたら、[準備] を選択します。 プロビジョニングプロセスには最大15分かかります。サイトがアクセスできる状態になると、メールによって ([プロビジョニング] ページで入力した通知の電子メールアドレスに) 通知されます。

7. 準備が完了したことが通知されたら、[プロビジョニング] ページで入力した宛先 URL を参照します。

8. 右上隅にサイトをお気に入りに置いて、後で参照するために URL をブックマークにします。  

### <a name="next-steps"></a>次のステップ
- webpart に含まれる[既定のコンテンツ](sitecontent.md)について説明します。
- 組織のトレーニング環境を[カスタマイズ](customization.md)します。
- トレーニングソリューションの[導入を促進](driveadoption.md)します。
