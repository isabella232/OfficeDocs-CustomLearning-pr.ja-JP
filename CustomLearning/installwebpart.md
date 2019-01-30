# <a name="installing-the-custom-learning-solution-webpart"></a>学習ソリューションの web パーツ、カスタムのインストール

## <a name="prerequisites-for-a-tenant-wide-installation"></a>テナント全体のインストールの前提条件

- 全体のテナントの学習のカスタム web パーツをインストールするのには、Office 365 の管理者権限を持っている必要があります。 場合は、Office 365 の管理者で作業するか、個々 のサイト コレクションの web パーツをインストールするには、これらのアクセス許可がありません。
- か、Office 365 の管理者のセットアップが必要し、テナント全体にわたる[アプリケーションのカタログ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)または[サイト コレクションのアプリケーション カタログ](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)は、web パーツが表示されるように構成します。]
- SharePoint Online 機能だけをサポートします。Web パーツは、社内設置型の SharePoint のすべてのバージョンにインストールするためのサポートではありません。

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>テナントに学習のカスタム web パーツを追加します。 

1. 学習のカスタム web パーツをダウンロードし、ローカル ドライブに保存します。 このファイルを「ms ・ カスタム ・ learning.sppkg」といいます。 名またはファイルのサフィックスは変更されません。 
2. テナントの[Office 365 管理ポータル](https://admin.microsoft.com/AdminPortal/Home#/homepage)に移動します。
3. 左側のナビゲーションから、管理センターでは、SharePoint を選択します。SharePoint 管理センターで [アプリケーション、アプリケーションのカタログ、SharePoint のアプリケーション、新しいタブに表示されます。 
4. 選択は、web パーツをアップロードするファイルを選択して「ms ・ カスタム ・ learning.sppkg」をダウンロードしました。
5. テナント全体のインストール] チェック ボックス」にこのソリューションを組織内のすべての位置を使用」  

![ソリューションを導入します。](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a>お客様のラーニングの web パーツを SharePoint オンライン ページに追加します。

カスタムの学習は、テナントのインストール後は、SharePoint ページに Web パーツを追加できます。実行すると、突然 Office 365 のトレーニングが利用できます。 

1. 全体の幅の列のレイアウトでは、学習のカスタム web パーツを追加します。

![SharePoint ページのレイアウト](media/clo365fullcolumnwidth.png)

2. SharePoint ページでの追加」を選択して全体の幅の列を選択し。 次のプロンプトが表示されます。

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. Microsoft ラーニングを選択します。 次が今すぐ表示されます。 

![カスタムの web パーツを学習します。](media/clo365addwebpart.png)

 ソリューションに含まれている既定のコンテンツを表示するタイルをクリックします。  

## <a name="next-steps"></a>次のステップ
- Web パーツに含まれる[既定のコンテンツ](webpartcontent.md)を表示します。
- [ユーザー設定](customization.md)、組織のトレーニング経験します。
- トレーニング ソリューションの[採用を推進](driveadoption.md)をします。

