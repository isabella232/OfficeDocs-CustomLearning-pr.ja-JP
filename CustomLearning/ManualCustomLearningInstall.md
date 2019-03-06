# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Office 365 のカスタム学習を手動でインストールおよび構成する

Microsoft カスタム学習 Web パーツは、 [SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview)バージョン1.7.1 を使用してビルドされます。

web パーツおよびサイトコレクションを手動でインストールして構成するには、次の手順を実行する必要があります。

1. すべての前提条件を満たしていることを確認します。
1. Office 365 テナントのアプリカタログに customlearning ファイルをインストールします。
1. Office 365 ホームサイト用のカスタム学習として機能するモダンコミュニケーションサイトをプロビジョニング/識別します。
1. カスタム学習が依存する適切な成果物を使用してテナントを構成する PowerShell スクリプトを実行します。
1. CustomLearningAdmin サイトページに移動して、管理者 web パーツを読み込んで、カスタムコンテンツ構成を初期化します。

## <a name="prerequisites"></a>前提条件

テナント全体のアプリカタログを設定して構成しておく必要があります。 「 [Office 365 テナントをセットアップ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)する」を参照して、「アプリカタログサイトを作成する」セクションに従ってください。 テナント全体のアプリカタログが既にプロビジョニングされている場合は、このセットアッププロセスを完了するためにパッケージをアップロードする権限を持つアカウントにアクセスする必要があります。 通常、これは SharePoint 管理者の役割を持つアカウントです。 その役割を持つアカウントが機能しない場合は、sharepoint 管理センターに移動して、アプリカタログサイトコレクションのサイトコレクション管理者を見つけ、いずれかのサイトコレクション管理者としてログインするか、または sharepoint 管理者アカウントを追加します。サイトコレクションの管理者に失敗しました。 SharePoint テナント管理者であるアカウントにもアクセスできる必要があります。

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>web パーツをテナントのアプリカタログにアップロードする

Office 365 のカスタム学習をセットアップするには、customlearning ファイルをテナント全体のアプリカタログにアップロードして展開します。 アプリカタログにアプリを追加する方法の詳細については[、「アプリカタログを使用してカスタムビジネスアプリを SharePoint Online 環境で利用できるようにする」を](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)参照してください。

## <a name="provisionidentify-modern-communication-site"></a>モダンコミュニケーションサイトのプロビジョニング/識別

既存の sharepoint コミュニケーションサイトを識別するか、sharepoint Online テナントで新しいサイトをプロビジョニングします。 コミュニケーションサイトのプロビジョニング方法の詳細については、「 [SharePoint Online でコミュニケーションサイトを作成](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)する」を参照し、手順に従ってコミュニケーションサイトを作成してください。

## <a name="set-permissions-for-the-site"></a>サイトのアクセス許可を設定する

閲覧者グループにコンテンツを表示できるようにするすべてのユーザーと、メンバーグループにカスタム再生リストを管理できる必要があるユーザーを追加する必要があります。 ユーザーが初めてサイトコレクション管理者または所有者グループの一部である必要がある場合に、カスタム学習用にサイトを構成する。

Office 365 アプリのカスタム学習機能をサイトコレクションに追加します。

## <a name="execute-powershell-configuration-script"></a>PowerShell 構成スクリプトを実行する

ソリューションで使用`CustomLearningConfiguration.ps1`する3つの[テナントプロパティ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)を作成するために実行する必要がある PowerShell スクリプトが含まれています。 さらに、スクリプトは、管理者とユーザーの web パーツを既知の場所にホストするために、サイトページライブラリに2つの[単一パーツアプリページ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)を作成します。

### <a name="disabling-telemetry-collection"></a>テレメトリコレクションの無効化

このソリューションの一部には、既定でオンに設定されている匿名化テレメトリトラッキングオプトインが含まれています。 手動によるインストールを実行していて、テレメトリの追跡をオフにする場合は`CustomlearningConfiguration.ps1` 、$optInTelemetry 変数を $false に設定するようにスクリプトを変更してください。

手動インストールを実行しておらず、テレメトリトラッキングをオフにしたい場合は、実行`TelemetryOptOut.ps1`時にテレメトリ追跡を無効にする別のスクリプトが含まれています。

## <a name="initialize-web-part-custom-configuration"></a>web パーツのカスタム構成を初期化する

PowerShell スクリプトが正常に実行されたら、 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`に移動します。 これにより、最初に使用するカスタム学習を設定する customconfig リストアイテムが初期化されます。

これで、構成は完了し、Office 365 のカスタム学習を使用することによって進めることができます。 詳細については、ユーザーマニュアルを参照してください。