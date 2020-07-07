---
author: pkrebs
ms.author: pkrebs
title: 経路の手動セットアップの学習
ms.date: 07/06/2020
description: Microsoft 365 学習経路手動セットアップ
ms.openlocfilehash: f980722fed48b5f92fb595cf8286604b3fa6d409
ms.sourcegitcommit: ba0cddd12dd8687ec4b97c26174fdda09de83b05
ms.contentlocale: ja-JP
ms.lasthandoff: 07/06/2020
ms.locfileid: "45043269"
---
# <a name="learning-pathways-manual-setup"></a>経路の手動セットアップの学習

Microsoft 365 の学習経路は、次のいずれかのシナリオのサポートを必要とする組織のために手動によるセットアップを提供します。 

- 組織には、トレーニング専用の SharePoint Online モダンコミュニケーションサイトが確立されており、そのサイトにラーニング経路を追加する必要があります。 このシナリオでは、ラーニングパス web パーツはサイトにセットアップされていません。

- 組織の SharePoint コミュニケーションサイトで多言語サポートのための学習経路をインストールする必要がある。 サイトに英語以外の既定の言語が設定されているか、または、学習経路でサポートされている言語のいずれかである。 ラーニング経路でサポートされている言語は次のとおりです。

- English
- 簡体字中国語
- フランス語
- ドイツ語
- イタリア語 (イタリア)
- 日本語 (日本)
- ポルトガル語 (ブラジル)
- ロシア語 (ロシア)
- スペイン語

学習経路を手動でセットアップするには、Windows PowerShell および SharePoint Online 管理シェルを使用した経験が必要です。 学習経路を手動でセットアップする手順の概要を次に示します。 

- すべての前提条件を満たしていることを確認します。
- サイトの既定の言語設定を確認します。 OK の場合は、手動インストールを続行します。 既定の言語設定が異なる場合は、新しいサイトを作成する必要があります。 
- SharePoint テナントのアプリカタログに customlearning ファイルをインストールします。
- Microsoft 365 learning ・経路のホームサイトとして機能するモダンコミュニケーションサイトをプロビジョニング/識別します。
- テナントを学習する成果物を使用してテナントを構成する PowerShell スクリプトを実行します。
- CustomLearningAdmin サイトページに移動して、管理者 web パーツを読み込んで、カスタムコンテンツ構成を初期化します。

## <a name="prerequisites"></a>前提条件
ラーニングパス web パーツを手動でセットアップするには、次の前提条件を満たしている必要があります。 

- テナント全体のアプリカタログを設定して構成しておく必要があります。 「 [Office 365 テナントをセットアップする](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)」および「アプリカタログの作成」のセクションに従ってください。 
- テナント全体のアプリカタログが既にプロビジョニングされている場合は、パッケージをアップロードする権限を持つアカウントにアクセスする必要があります。 通常、このアカウントには SharePoint 管理者の役割があります。 
- その役割を持つアカウントが機能しない場合は、SharePoint 管理センターに移動して、アプリカタログサイトコレクションのサイトコレクション管理者を検索し、いずれかのサイトコレクション管理者としてログインするか、またはサイトコレクション管理者に失敗した SharePoint 管理者アカウントを追加します。 
- SharePoint テナント管理者であるアカウントにもアクセスできる必要があります。

## <a name="step-1---check-your-language-settings"></a>手順 1-言語設定を確認する
手動インストールプロセスの最初の手順として、サイトの言語設定を確認します。 可能なオプションは次のとおりです。

### <a name="option-1---you-dont-want-multilingual-support"></a>オプション 1-多言語のサポートを必要としません
サイトで多言語サポートを使用しない場合は、オフにします。
1.  SharePoint コミュニケーションサイトで、[**設定**] [  >  **サイト情報**]、[  >  **すべてのサイト設定**  >  の**言語設定**] のいずれかを選択します。 
2.  [**ページとニュースを複数言語に翻訳する**] スイッチを [**オフ**] に設定します。
3.  [**保存**] をクリックします。 
4.  手順2に進みます。

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>オプション 2-多言語のサポートが必要で、既定の言語で OK
SharePoint コミュニケーションサイトには、既定の言語があります。 [ラーニングパス] 管理ページを含む、学習経路の表示に使用する言語は、既定の言語によって決まります。 既定の言語の設定は、サイトが初めて作成されたときに設定され、後から変更することはできません。 手動セットアップを続行する前に、ターゲットサイトの既定の言語を使用していることを確認してください。

1.  SharePoint コミュニケーションサイトで、[**設定**] [  >  **サイト情報**]、[  >  **すべてのサイト設定**  >  の**言語設定**] のいずれかを選択します。 
2.  [**ページとニュースを複数言語に翻訳する**] スイッチを **[オン**] に設定します。
    - [**言語**] の下にある一覧の一番上に表示されている言語を使用している場合は、追加の言語を追加して、[**保存**] をクリックします。 手順2に進みます。
    - サイトで選択されている言語とは異なる既定の言語を使用する場合は、必要な言語の新しい SharePoint コミュニケーションサイトを作成する必要があります。 オプション3に進みます。 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>オプション #3-多言語のサポートを必要としますが、サイトの既定の言語とは異なるものを使用します。
このオプションを使用して、使用する既定の言語で新しい SharePoint Online コミュニケーションサイトを作成し、サイトの言語設定を設定します。 
1.  新しい SharePoint コミュニケーションサイトを作成するには、「 [Sharepoint Online でコミュニケーションサイトを作成](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)する」を参照してください。 サイトを作成するときは、必ず言語を学習するための既定の言語に設定してください。 
2. 作成したサイトから、[**設定**] [  >  **サイト情報**]、[  >  **すべてのサイト設定**  >  の**言語設定**] のいずれかを選択します。 
2.  [**ページとニュースを複数言語に翻訳する**] スイッチを **[オン**] に設定します。
3. 必要に応じて追加の言語を追加し、[**保存**] をクリックします。 
4. 手順2に進みます。 

>!ことサイトから新しく作成したサイトにカスタムコンテンツを移行する必要がある場合は、後述の「カスタムコンテンツを移行する」セクションを参照してください。 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>手順 2-GitHub から web パーツパッケージとセットアップスクリプトを取得する
セットアッププロセスの一環として、Microsoft 365 learning の経路の Web パーツパッケージと PowerShell セットアップスクリプトが必要になります。

- [学習経路 GitHub リポジトリ](https://github.com/pnp/custom-learning-office-365)に移動します。
- [**ダウンロード**] をクリックして、web パーツパッケージとスクリプトをローカルドライブに保存します。 このプロセスの後の手順で、スクリプトと web パーツパッケージを使用します。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>手順 2-テナントのアプリカタログに web パーツをアップロードする
Microsoft 365 learning の経路を設定するには、customlearning ファイルをテナント全体のアプリカタログにアップロードして展開します。 アプリカタログにアプリを追加する詳細な手順については[、「アプリカタログを使用してカスタムビジネスアプリを SharePoint Online 環境で利用できるようにする」を](https://docs.microsoft.com/sharepoint/use-app-catalog)参照してください。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>手順 3-モダンコミュニケーションサイトをプロビジョニング/識別する
既存の SharePoint コミュニケーションサイトを識別するか、SharePoint Online テナントで新しいサイトをプロビジョニングします。 コミュニケーションサイトのプロビジョニング方法の詳細については、「 [SharePoint Online でコミュニケーションサイトを作成](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)する」を参照し、手順に従ってコミュニケーションサイトを作成してください。

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>手順 4-サイトに Microsoft 365 learning パスアプリを追加する

1. SharePoint サイトで、[システム] メニューの [アプリの**追加**] をクリックします。 
2. **ご使用のアプリ**の下で、[**組織**内] をクリックし、[ **Office 365 のラーニング経路**] をクリックします。 

## <a name="step-5---set-permissions-for-the-site"></a>手順 5-サイトのアクセス許可を設定する
サイトに対して次のアクセス許可が設定されていることを確認します。
- **サイトコレクションの管理者または所有者のグループ**権限。最初に使用するために、学習経路を設定する customconfig リストアイテムを初期化するために必要です。 
- **メンバーグループ**-学習経路を管理するために必要なアクセス許可 (コンテンツの表示/非表示、カスタムプレイリストの管理など)
- **閲覧者グループ**-サイトコンテンツを表示するために必要なアクセス許可。 

## <a name="step-6--execute-powershell-configuration-script"></a>手順 6-PowerShell 構成スクリプトを実行する
`CustomLearningConfiguration.ps1`ソリューションで使用する3つの[テナントプロパティ](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties)を作成するために実行する必要がある PowerShell スクリプトが含まれています。 さらに、このスクリプトは、管理者とユーザーの web パーツを既知の場所にホストするために、サイトページライブラリに2つの[単一パーツアプリページ](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages)を作成します。

1. SharePoint Online 管理シェルをまだダウンロードしていない場合は、今すぐダウンロードしてください。 「 [SharePoint Online 管理シェルのダウンロード](https://go.microsoft.com/fwlink/p/?LinkId=255251)」を参照してください。
2. スクリプトを実行するには、PowerShell の実行ポリシーを設定する必要がある場合があります。 詳細については、「[実行ポリシーについ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)て」を参照してください。
3. スクリプトを実行 `CustomLearningConfiguration.ps1` します。 テナント管理者の資格情報に加えて、スクリプトによってテナント名とサイト名の入力を求められます。 サイトの URL として次の例を検討して `https://contoso.sharepoint.com/sites/O365CL` `contoso` ください。は、テナント名で、 `O365CL` はサイト名です。 

### <a name="disabling-telemetry-collection"></a>テレメトリコレクションの無効化
このソリューションの一部には、既定でオンに設定されている匿名化テレメトリトラッキングオプトインが含まれています。 手動によるインストールを実行していて、テレメトリの追跡をオフにする場合は、 `CustomlearningConfiguration.ps1` $optInTelemetry 変数を $false に設定し、スクリプトを実行するようにスクリプトを変更します。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>プロビジョニングが成功したことを検証し、CustomConfig リストを初期化する

PowerShell スクリプトが正常に実行されたら、サイトに移動し、最初に使用するために学習経路を設定する**Customconfig**リストアイテムを初期化して、サイトが動作していることを確認します。

- `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` に移動します。 **CustomLearningAdmin**を開くと、最初に使用するための学習経路を設定する**customconfig**リストアイテムが初期化されます。 次のようなページが表示されます。

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>サイトに所有者を追加する
テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトにいくつかの所有者を割り当てる必要があります。 所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。 また、ラーニングパス Web パーツを通じて配信されるコンテンツを非表示にし、表示することもできます。 さらに、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることができます。  

1. [SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。
2. [**高度なアクセス許可の設定**] をクリックします。
3. [ **Office 365 所有者のための教育経路] を**クリックします。
4. [**新しい**  >  **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加します。 
5. 共有メッセージ内の[サイトを探索](https://docs.microsoft.com/Office365/CustomLearning/custom_explore)するためのリンクを追加し、[**共有**] をクリックします。

## <a name="migrate-custom-content"></a>カスタムコンテンツを移行する
上記の手順に従って学習機のサイトを再確立した後、 **Customplaylists**リストのリストと**customplaylists**リストの内容を移動する必要があります。 また、必要に応じて、カスタムアセットを構成する実際のカスタムページを既存の学習機能サイトにある場合は、それらを削除することもできます。 **Customplaylists**リスト内のすべてのアイテムに対して、 **customplaylists**リスト内のリストアイテムの ID が、各再生リストのリストアイテムの jsondata フィールドに埋め込まれているため、タスクが困難になることがあります。 そのため、あるサイトから別のサイトに**Customplaylists**リストのコンテンツを移動するだけでは不十分です。 さらに、 **Customassets**リストには、リストアイテムの jsondata フィールドにカスタムアセットのページへの絶対 URL が含まれています。 アセットが移動されず、サイトの名前が変更されない (つまり、絶対 URL がアセットのページに変更される) 場合、 **Customassets**を残すことができます。 ただし、エントリを手動で修正する必要があります。 この種類の移行の複雑さを考慮して、この移行を支援するために、ラーニング経路パートナーの1つを参加させることをお勧めします。 

### <a name="next-steps"></a>次の手順
- 「[学習経路をカスタマイズ](custom_overview.md)する」を参照してください。 
- 「[サイトページの翻訳](custom_translate_page_ml.md)」を参照してください。


