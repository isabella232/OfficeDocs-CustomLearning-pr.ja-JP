---
author: pkrebs
ms.author: pkrebs
title: カスタム学習アップグレード
ms.date: 02/10/2019
description: Office 365 マニュアル web パーツのセットアップのカスタム学習
ms.openlocfilehash: f9729c922b374cc6b775737fa7c7c76a4719534c
ms.sourcegitcommit: b6617bbbaee0784d6216e96052c2469f97cf51e9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "30411897"
---
# <a name="manual-upgrade-for-custom-learning"></a>カスタム学習の手動アップグレード

Office 365 のカスタム学習では、以前のパイロットに参加していた組織に手動でのアップグレードプロセスが提供されます。 アップグレードプロセスでは、組織は、新しいカスタム学習 web パーツを SharePoint アプリカタログに追加してから PowerShell スクリプトを実行することによって、現在のカスタム学習サイトとアップグレードを引き続き使用できます。 アップグレードプロセスの概要を次に示します。 

- 新しい web パーツをアップロードし、Powershell スクリプトを実行する担当者が必要なアクセス許可を持っていることを確認する
- web パーツ、customlearning、sppkg ファイルを Office 365 テナントのアプリカタログにアップロードします。
- カスタム学習に必要な適切な成果物を使用してテナントを構成する PowerShell スクリプトを実行します。
- カスタムのラーニングサイトの CustomLearningAdmin ページに移動して、カスタムの ccontent 構成を初期化します。

## <a name="prerequisites"></a>前提条件
カスタム学習を正常にアップグレードするには、次の前提条件が満たされている必要があります。 

- テナント全体のアプリカタログを設定する必要があります。 テナントアプリカタログを持っていない場合は、「 [Office 365 テナントをセットアップ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)する」を参照し、「アプリカタログサイトを作成する」セクションに従ってください。 
- テナント全体のアプリカタログが既にプロビジョニングされている場合は、パッケージをアップロードする権限を持つアカウントにアクセスする必要があります。 通常、これは SharePoint 管理者の役割を持つアカウントです。 
- sharepoint 管理者の役割を持つアカウントが機能しない場合は、sharepoint 管理センターに移動し、アプリカタログを選択し、[所有者] をクリックして、サイトコレクションの管理者の1つとしてサインインするか、失敗した sharepoint 管理者アカウントをサイトに追加します。コレクション管理者リスト。 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>手順 1-GitHub から web パーツパッケージを取得し、スクリプトをセットアップする
セットアッププロセスの一環として、カスタム学習 Web パーツパッケージと PowerShell セットアップスクリプトが必要になります。

1. [カスタムラーニング GitHub リポジトリ](https://github.com/pnp/custom-learning-office-365)に移動します。
2. [**複製] または [ダウンロード**] をクリックし、[ **ZIP のダウンロード**] をクリックします。   
3. **ZIP**ファイルをローカルドライブの場所に保存します。
4. ローカルドライブで**ZIP**ファイルを抽出します。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>手順 2-テナントのアプリカタログに web パーツをアップロードする
Office 365 のカスタム学習をセットアップするには、customlearning ファイルをテナント全体のアプリカタログにアップロードして展開します。 アプリカタログにアプリを追加する方法の詳細については[、「アプリカタログを使用してカスタムビジネスアプリを SharePoint Online 環境で利用できるようにする」を](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)参照してください。

1. Office 365 で、[**管理者**] をクリックします。
2. [**管理センター**] で、[ **SharePoint**] をクリックします。
3. [**アプリ** > **アプリカタログ** > **を SharePoint 用アプリに配布] をクリックします。**
4. [**アップロード** > **ファイルの選択] を**クリックします。
5. ZIP ファイルを保存したフォルダーで、[ **webpart** ] フォルダーを選択し、[ **customlearning] [sppkg** ] を選択します。
6. [**展開**] をクリックします。

## <a name="step-5--execute-powershell-configuration-script"></a>手順 5-PowerShell 構成スクリプトを実行する
PowerShell スクリプト`CustomLearningConfiguration.ps1`は、GitHub からの ZIP ダウンロードに含まれています。 このスクリプトを実行して、ソリューションで使用される3つの[テナントプロパティ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)を作成する必要があります。 さらに、このスクリプトは、管理者とユーザーの web パーツを既知の場所にホストするために、サイトページライブラリに2つの[単一パーツアプリページ](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)を作成します。 これらのアプリページは次のとおりです。

- customadministration .aspx
- customviewer .aspx

### <a name="to-run-the-powershell-script"></a>Powershell スクリプトを実行するには
- PowerShell を使用して`CustomLearningConfiguration.ps1` 、GitHub ZIP から webpart フォルダーにあるスクリプトを実行します。 成功した場合は、コマンドウィンドウに3つのキーと値のペアと**カスタム学習管理者**が表示されます。

### <a name="disabling-telemetry-collection"></a>テレメトリコレクションの無効化
カスタム学習には、匿名化テレメトリトラッキングオプトインが含まれています。これは、既定では [オン] に設定されています。 テレメトリトラッキングをオフにしたい場合は、 `CustomlearningConfiguration.ps1` `$optInTelemetry`変数をに`$false`設定するようにスクリプトを変更してください。

## <a name="step-6---initialize-web-part-custom-configuration"></a>ステップ 6-web パーツのカスタム構成の初期化
PowerShell スクリプトが正常に実行されたら、 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`に移動します。 **CustomLearningAdmin**を開くと、カスタム学習を設定する**customconfig**リストアイテムが初期化されます。 次のようなページが表示されます。

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>サイトに所有者を追加する
テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトにいくつかの所有者を割り当てる必要があります。 所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。 また、カスタム学習 Web パーツを通じて配信されるコンテンツを非表示にしたり、表示したりすることもできます。 また、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることもできます。  

1. [SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。
2. [**高度なアクセス許可の設定**] をクリックします。
3. [ **Office 365 所有者向けのカスタム学習] を**クリックします。
4. [**新しい** > **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加して、[**共有**] をクリックします。

これでアップグレードが完了しました。 環境に合わせてカスタム学習サイトと web パーツをカスタマイズする方法の詳細については、「トレーニング環境を[カスタマイズ](custom_overview.md)する」を参照してください。

## <a name="upgrade-instructions-for-site-owners"></a>サイト所有者のアップグレード手順
office 365 のカスタム学習では、web パーツにさまざまな機能拡張が導入されています。 web パーツの作業の詳細については、「 [learning experience のカスタマイズ](custom_overview.md)」セクションを参照してください。 ここでは、サイトの所有者は次のようにする必要があります。  

- カスタム学習 Office 365 Web パーツが利用可能であることを確認します。 
- ページ上の既存の web パーツを新しい web パーツに置き換える
- 古い web パーツを指すリンクを置き換える

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>Office 365 web パーツのカスタム学習が利用可能であることを確認する
1.  カスタム学習サイトから、[**設定**] をクリックし、[***ページの追加**] をクリックします。
2.  ページの**+** アイコンをクリックして web パーツを追加し、[ **Office 365 web パーツのカスタム学習**] を選択します。 ページは次の図のようになります。

[cg-adminapppage](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>古い web パーツを新しい web パーツに置き換える
カスタム学習 web パーツを置き換えるか、サイトに変更を加える前に、新しい web パーツの使用方法について説明している「[学習環境のカスタマイズ](custom_overview.md)」のドキュメントを参照することをお勧めします。 

カスタム学習サイトをアップグレードするには、web パーツの既存のインスタンスを新しい web パーツに置き換えます。 web パーツが追加された場所を確認することはできませんが、前のパイロット向けのガイダンスでは、次のページに web パーツを追加する必要がありました。そのため、これらのページで web パーツを置換することを確認してください。

- Get-started-with-Office-365
- Get-started-with-Microsoft-Teams
- Get-started-with-OneDrive
- Get-started-with-SharePoint

### <a name="replace-existing-links-to-the-web-part"></a>既存のリンクを web パーツに置き換える
新しい web パーツの機能強化により、再生リストにリンクする方法が変更されました。 アップグレードの一環として、web パーツ (メニュー項目、ホームページ上のリンクなど) へのすべてのリンクを置き換える必要があります。 カスタム学習 web パーツを置き換えるか、サイトに変更を加える前に、新しい web パーツの使用方法について説明している「[学習環境のカスタマイズ](custom_overview.md)」のドキュメントを参照することをお勧めします。 

## <a name="recreate-existing-playlists"></a>既存の再生リストを再作成する 
再生リストが正しく動作することを確認するには、以前のバージョンの web パーツを使用して作成されたすべての再生リストを再作成する必要があります。 再生リストを削除する前に、カスタムプレイリストと関連付けられているアセットのリストを作成し、新しいカスタム学習 Web パーツを使用して簡単に再作成できるようにします。 再生リストのコピーを作成し、削除します。 jsondata フィールドを使用して、削除する前に再生リストのコンテンツのコピーを作成できます。 これにより、後で作成することが容易になります。


•カスタム学習サイトから、[設定 > サイトコンテンツ] をクリックします。 •再生リストを選択し、省略記号を選択して、[編集] を選択し、[jsondata] フィールドの内容をメモ帳に保存し、後で参照するために別のドキュメントに保存します。 [キャンセル] を選択します。
•再生リストを選択し、省略記号を選択して、[削除] を選択します。
•新しい Web パーツを使用してプレイリストを再作成する準備ができました。
Office 365 Web パーツの新しいカスタム学習を使用する方法についてhttps://docs.microsoft.com/en-us/office365/customlearning/custom_overviewは、「」を参照してください。

## <a name="step-8---chan"></a>手順 8-チャンネル

### <a name="next-steps"></a>次のステップ
- 組織のトレーニング環境を[カスタマイズ](custom_overview.md)します。

