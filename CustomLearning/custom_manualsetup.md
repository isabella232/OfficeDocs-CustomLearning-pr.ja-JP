---
author: pkrebs
ms.author: pkrebs
title: スタンドアロン web パーツのセットアップ
ms.date: 02/10/2019
description: Microsoft 365 learning ・経路手動 web パーツのセットアップ
ms.openlocfilehash: f3271dbd75ee18db7f89fdd15ebb35c1b2bf7d97
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247872"
---
# <a name="stand-alone-web-part-setup"></a>スタンドアロン web パーツのセットアップ

Microsoft 365 の学習経路は、既に確立されている SharePoint Online モダンコミュニケーションサイトが既に作成されている組織に対してスタンドアロンの手動による web パーツのセットアップを提供しています。これは、自分のコミュニケーションサイト。 手動セットアップでは、Windows PowerShell および SharePoint Online 管理シェルの操作が必要です。 ラーニングの Web パーツを手動でセットアップする手順は、次のとおりです。

- すべての前提条件を満たしていることを確認します。
- SharePoint テナントのアプリカタログに customlearning ファイルをインストールします。
- Microsoft 365 learning ・経路のホームサイトとして機能するモダンコミュニケーションサイトをプロビジョニング/識別します。
- テナントを学習させる適切な成果物を使用してテナントを構成する PowerShell スクリプトを実行します。
- CustomLearningAdmin サイトページに移動して、管理者 web パーツを読み込んで、カスタムコンテンツ構成を初期化します。

> [!NOTE]
> 学習経路をすばやく簡単にセットアップする方法については、「 [Microsoft 365 learning の経路をプロビジョニング](custom_provision.md)する」を参照してください。

## <a name="prerequisites"></a>前提条件
ラーニングパス web パーツを手動でセットアップするには、次の前提条件を満たしている必要があります。 

- テナント全体のアプリカタログを設定して構成しておく必要があります。 「 [Office 365 テナントをセットアップ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)する」を参照して、「アプリカタログサイトを作成する」セクションに従ってください。 
- テナント全体のアプリカタログが既にプロビジョニングされている場合は、このセットアッププロセスを完了するためにパッケージをアップロードする権限を持つアカウントにアクセスする必要があります。 通常、これは SharePoint 管理者の役割を持つアカウントです。 
- その役割を持つアカウントが機能しない場合は、SharePoint 管理センターに移動して、アプリカタログサイトコレクションのサイトコレクション管理者を見つけ、いずれかのサイトコレクション管理者としてログインするか、または SharePoint 管理者アカウントを追加します。サイトコレクションの管理者に失敗しました。 
- SharePoint テナント管理者であるアカウントにもアクセスできる必要があります。

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>手順 1-GitHub から web パーツパッケージを取得し、スクリプトをセットアップする
セットアッププロセスの一環として、Microsoft 365 learning の経路の Web パーツパッケージと PowerShell セットアップスクリプトが必要になります。

- [ラーニング経路 GitHub リポジトリ](https://github.com/pnp/custom-learning-office-365)に移動します。
- [**ダウンロード**] をクリックして、web パーツパッケージとスクリプトをローカルドライブに保存します。 このプロセスの後の手順で、スクリプトと web パーツパッケージを使用します。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>手順 2-テナントのアプリカタログに web パーツをアップロードする
Microsoft 365 learning の経路を設定するには、customlearning ファイルをテナント全体のアプリカタログにアップロードして展開します。 アプリカタログにアプリを追加する方法の詳細については[、「アプリカタログを使用してカスタムビジネスアプリを SharePoint Online 環境で利用できるようにする」を](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)参照してください。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>手順 3-モダンコミュニケーションサイトをプロビジョニング/識別する
既存の SharePoint コミュニケーションサイトを識別するか、SharePoint Online テナントで新しいサイトをプロビジョニングします。 コミュニケーションサイトのプロビジョニング方法の詳細については、「 [SharePoint Online でコミュニケーションサイトを作成](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)する」を参照し、手順に従ってコミュニケーションサイトを作成してください。

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>手順 4-サイトに Microsoft 365 learning パスアプリを追加する

1. SharePoint サイトで、[システム] メニューの [アプリの**追加**] をクリックします。 
2. **ご使用のアプリ**の下で、[**組織**内] をクリックし、[ **Office 365 のラーニング経路**] をクリックします。 

## <a name="step-5---set-permissions-for-the-site"></a>手順 5-サイトのアクセス許可を設定する
サイトに対して次のアクセス許可が設定されていることを確認します。
- **サイトコレクションの管理者または所有者のグループ**権限。最初に使用するために、学習経路を設定する customconfig リストアイテムを初期化するために必要です。 
- **メンバーグループ**-permissons コンテンツの表示と表示、カスタムプレイリストの管理など、学習経路を管理するために必要です。
- **閲覧者グループ**-サイトコンテンツを表示するために必要なアクセス許可。 

## <a name="step-6--execute-powershell-configuration-script"></a>手順 6-PowerShell 構成スクリプトを実行する
ソリューションで使用`CustomLearningConfiguration.ps1`する3つの[テナントプロパティ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)を作成するために実行する必要がある PowerShell スクリプトが含まれています。 さらに、スクリプトは、管理者とユーザーの web パーツを既知の場所にホストするために、サイトページライブラリに2つの[単一パーツアプリページ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)を作成します。

1. SharePoint Online 管理シェルをまだダウンロードしていない場合は、今すぐダウンロードしてください。 「 [SharePoint Online 管理シェルのダウンロード](https://go.microsoft.com/fwlink/p/?LinkId=255251)」を参照してください。
2. スクリプトを実行するには、PowerShell の実行ポリシーを設定する必要がある場合があります。 詳細については、「[実行ポリシーについ](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)て」を参照してください。
3. スクリプトを`CustomLearningConfiguration.ps1`実行します。 テナント管理者の資格情報に加えて、スクリプトによってテナント名とサイト名の入力を求められます。 サイトの URL `https://contoso.sharepoint.com/sites/O365CL`と`contoso` `O365CL`して次の例を検討してください。は、テナント名で、はサイト名です。 

### <a name="disabling-telemetry-collection"></a>テレメトリコレクションの無効化
このソリューションの一部には、既定でオンに設定されている匿名化テレメトリトラッキングオプトインが含まれています。 手動によるインストールを実行していて、テレメトリの追跡をオフにしたい場合`CustomlearningConfiguration.ps1`は、スクリプトを変更して $optInTelemetry 変数を $false に設定し、スクリプトを実行してください。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>プロビジョニングが成功したことを検証し、CustomConfig リストを初期化する

PowerShell スクリプトが正常に実行されたら、サイトに移動し、最初に使用するために学習経路を設定する**Customconfig**リストアイテムを初期化して、サイトが動作していることを確認します。

- `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` に移動します。 **CustomLearningAdmin**を開くと、最初に使用するための学習経路を設定する**customconfig**リストアイテムが初期化されます。 次のようなページが表示されます。

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>サイトに所有者を追加する
テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトにいくつかの所有者を割り当てる必要があります。 所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。 また、ラーニングパス Web パーツを通じて配信されるコンテンツを非表示にし、表示することもできます。 さらに、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることができます。  

1. [SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。
2. [**高度なアクセス許可の設定**] をクリックします。
3. [ **Office 365 所有者のための教育経路] を**クリックします。
4. [**新しい** > **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加します。 
5. 共有メッセージ内の[サイトを探索](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore)するためのリンクを追加し、[**共有**] をクリックします。

### <a name="next-steps"></a>次のステップ
- 組織のトレーニング環境を[カスタマイズ](custom_overview.md)します。

