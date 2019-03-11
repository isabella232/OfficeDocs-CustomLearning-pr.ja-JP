---
author: pkrebs
ms.author: pkrebs
title: スタンドアロン web パーツのセットアップ
ms.date: 02/10/2019
description: Office 365 マニュアル web パーツのセットアップのカスタム学習
ms.openlocfilehash: f5d94d673f491d5b5778ef73d518914dbd4cdbb9
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523061"
---
# <a name="stand-alone-web-part-setup"></a>スタンドアロン web パーツのセットアップ

カスタム学習は、既に設定されている SharePoint Online モダンコミュニケーションサイトが既に作成されている組織に対して手動のスタンドアロン web パーツセットアップを提供します。または、独自にカスタム学習 web パーツをセットアップする必要があります。コミュニケーションサイト。 手動セットアップでは、Windows PowerShell および SharePoint Online 管理シェルの操作が必要です。 カスタム学習 Web パーツを手動でセットアップする手順は、次のとおりです。

- すべての前提条件を満たしていることを確認します。
- Office 365 テナントのアプリカタログに customlearning ファイルをインストールします。
- Office 365 ホームサイト用のカスタム学習として機能するモダンコミュニケーションサイトをプロビジョニング/識別します。
- カスタム学習が依存する適切な成果物を使用してテナントを構成する PowerShell スクリプトを実行します。
- CustomLearningAdmin サイトページに移動して、管理者 web パーツを読み込んで、カスタムコンテンツ構成を初期化します。

> [!NOTE]
> カスタム学習をすばやく簡単にセットアップする方法については、「[カスタム学習を準備](installsitepackage.md)する」を参照してください。

## <a name="prerequisites"></a>前提条件
カスタム学習 web パーツを正常に手動でセットアップするには、次の前提条件を満たしている必要があります。 

- テナント全体のアプリカタログを設定して構成しておく必要があります。 「 [Office 365 テナントをセットアップ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)する」を参照して、「アプリカタログサイトを作成する」セクションに従ってください。 
- テナント全体のアプリカタログが既にプロビジョニングされている場合は、このセットアッププロセスを完了するためにパッケージをアップロードする権限を持つアカウントにアクセスする必要があります。 通常、これは SharePoint 管理者の役割を持つアカウントです。 
- その役割を持つアカウントが機能しない場合は、sharepoint 管理センターに移動して、アプリカタログサイトコレクションのサイトコレクション管理者を見つけ、いずれかのサイトコレクション管理者としてログインするか、または sharepoint 管理者アカウントを追加します。サイトコレクションの管理者に失敗しました。 
- SharePoint テナント管理者であるアカウントにもアクセスできる必要があります。

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>手順 1-GitHub から web パーツパッケージを取得し、スクリプトをセットアップする
セットアッププロセスの一環として、カスタム学習 Web パーツパッケージと PowerShell セットアップスクリプトが必要になります。

- [カスタムラーニング GitHub リポジトリ](https://github.com/pnp/custom-learning-office-365)に移動します。
- [**ダウンロード**] をクリックして、web パーツパッケージとスクリプトをローカルドライブに保存します。 このプロセスの後の手順で、スクリプトと web パーツパッケージを使用します。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>手順 2-テナントのアプリカタログに web パーツをアップロードする
Office 365 のカスタム学習をセットアップするには、customlearning ファイルをテナント全体のアプリカタログにアップロードして展開します。 アプリカタログにアプリを追加する方法の詳細については[、「アプリカタログを使用してカスタムビジネスアプリを SharePoint Online 環境で利用できるようにする」を](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)参照してください。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>手順 3-モダンコミュニケーションサイトをプロビジョニング/識別する
既存の sharepoint コミュニケーションサイトを識別するか、sharepoint Online テナントで新しいサイトをプロビジョニングします。 コミュニケーションサイトのプロビジョニング方法の詳細については、「 [SharePoint Online でコミュニケーションサイトを作成](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)する」を参照し、手順に従ってコミュニケーションサイトを作成してください。

## <a name="step-4---set-permissions-for-the-site"></a>手順 4-サイトのアクセス許可を設定する
サイトに対して次のアクセス許可が設定されていることを確認します。
- **サイトコレクションの管理者または所有者のグループ**権限。最初に使用するカスタム学習を設定する customconfig リストアイテムを初期化するために必要です。 
- **メンバーグループ**-permissons コンテンツの表示と表示、カスタムプレイリストの管理など、カスタム学習を管理するために必要です。
- **閲覧者グループ**-サイトコンテンツを表示するために必要なアクセス許可。 

## <a name="step-5--execute-powershell-configuration-script"></a>手順 5-PowerShell 構成スクリプトを実行する
ソリューションで使用`CustomLearningConfiguration.ps1`する3つの[テナントプロパティ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)を作成するために実行する必要がある PowerShell スクリプトが含まれています。 さらに、スクリプトは、管理者とユーザーの web パーツを既知の場所にホストするために、サイトページライブラリに2つの[単一パーツアプリページ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)を作成します。

### <a name="disabling-telemetry-collection"></a>テレメトリコレクションの無効化
このソリューションの一部には、既定でオンに設定されている匿名化テレメトリトラッキングオプトインが含まれています。 手動によるインストールを実行していて、テレメトリの追跡をオフにする場合は`CustomlearningConfiguration.ps1` 、$optInTelemetry 変数を $false に設定するようにスクリプトを変更してください。

手動インストールを実行しておらず、テレメトリトラッキングをオフにしたい場合は、実行`TelemetryOptOut.ps1`時にテレメトリ追跡を無効にする別のスクリプトが含まれています。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>プロビジョニングが成功したことを検証し、customconfig リストを初期化する

PowerShell スクリプトが正常に実行されたら、サイトに移動して、最初に使用するためにカスタム学習を設定する**customconfig**リストアイテムを初期化し、サイトが動作していることを確認します。

1. `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` に移動します。 **CustomLearningAdmin**を開くと、カスタム学習を設定する**customconfig**リストアイテムが初期化されます。 次のようなページが表示されます。

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>サイトに所有者を追加する
テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトにいくつかの所有者を割り当てる必要があります。 所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。 また、カスタム学習 Web パーツを通じて配信されるコンテンツを非表示にしたり、表示したりすることもできます。 さらに、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることができます。  

1. [SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。
2. [**高度なアクセス許可の設定**] をクリックします。
3. [ **Office 365 所有者向けのカスタム学習] を**クリックします。
4. [**新しい** > **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加します。 
5. 共有メッセージ内の[サイトを探索](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore)するためのリンクを追加し、[**共有**] をクリックします。

### <a name="next-steps"></a>次のステップ
- 組織のトレーニング環境を[カスタマイズ](custom_overview.md)します。

