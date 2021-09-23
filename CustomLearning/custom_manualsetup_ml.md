---
author: pkrebs
ms.author: pkrebs
title: ラーニング ml の手動セットアップ
ms.date: 02/10/2019
description: ラーニング経路の手動セットアップ
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 89693e3020baa46f86b51b97c54240f12fec2d3a
ms.sourcegitcommit: a93cae8ea6e3c1141d7266d04131b69f2c2498cb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2021
ms.locfileid: "59485168"
---
# <a name="learning-pathways-manual-setup-for-multilingual"></a>ラーニングを手動でセットアップする方法

Microsoft 365学習経路は、次のいずれかのシナリオのサポートが必要な組織向け手動セットアップを提供します。

- 組織には、トレーニング専用SharePointオンラインモダンコミュニケーションサイトが確立され、そのサイトに学習経路を追加する必要があります。 このシナリオでは、Web パーツの学習経路がサイトに設定されていない。

- 組織のコミュニケーション サイトの 1 つで多言語サポート用の学習経路をSharePointします。 このサイトは、英語ではない既定の言語を持ち、学習経路でサポートされる言語の 1 つになります。 学習経路でサポートされている言語を次に示します。

- 英語
- 中国語 (簡体字)
- フランス語
- ドイツ語
- イタリア語 (イタリア)
- 日本語 (日本)
- ポルトガル語 (ブラジル)
- ロシア語 (ロシア語)
- スペイン語

学習経路の手動セットアップには、オンライン管理シェルWindows PowerShell操作SharePoint必要があります。 学習経路の手動セットアップの手順の概要を次に示します。 

- すべての前提条件を満たしていることを検証します。
- サイトの既定の言語設定を確認します。 [OK] の場合は、手動インストールを続行します。 別の既定の言語設定が必要な場合は、新しいサイトを作成する必要があります。 
- テナント アプリ カタログに customlearning.sppkg ファイルSharePointインストールします。
- 学習経路ホーム サイトとして機能する最新のMicrosoft 365を準備/識別します。
- 学習経路が依存する成果物を使用してテナントを構成する PowerShell スクリプトを実行します。
- CustomLearningAdmin.aspx サイト ページに移動して管理 Web パーツを読み込み、カスタム コンテンツ構成を初期化します。

## <a name="prerequisites"></a>前提条件
学習経路 Web パーツの手動セットアップを成功させるには、次の前提条件を満たす必要があります。 

- テナント全体のアプリ カタログをセットアップして構成している必要があります。 「[テナントをセットアップするOffice 365」を参照](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)し、「アプリ カタログの作成」サイトセクションに従います。 
- テナント全体のアプリ カタログが既にプロビジョニングされている場合は、パッケージをアップロードする権限を持つアカウントにアクセスする必要があります。 通常、このアカウントには管理者SharePointがあります。 
- その役割を持つアカウントが機能しない場合は、SharePoint 管理センターに移動し、App Catalog サイト コレクションのサイト コレクション管理者を探し、サイト コレクション管理者の 1 人としてログインするか、サイト コレクション管理者に失敗した SharePoint 管理者アカウントを追加します。 
- また、テナント管理者の管理者であるアカウントSharePoint必要があります。

## <a name="step-1---check-your-language-settings"></a>手順 1 - 言語設定を確認する
手動インストール プロセスの最初の手順として、サイトの言語設定を確認します。 次に、可能なオプションを示します。

### <a name="option-1---you-dont-want-multilingual-support"></a>オプション 1 - 多言語サポートが必要ない
サイトの多言語サポートが必要ない場合は、サイトがオフになっていることを確認します。
1.  [通信サイトSharePoint] で、[サイト **設定**  >  **すべての** サイト設定を表示  >  **する言語の設定**]  >  **を選択します**。 
2.  [複数の **言語に翻訳するページ** とニュースを有効にする] スイッチを [オフ] に **設定します**。
3.  **[保存]** をクリックします。 
4.  手順 2 に進みます。

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>オプション 2 - 多言語サポートが必要で、既定の言語でOK
通信SharePointは既定の言語です。 既定の言語では、[学習経路の管理] ページなど、学習経路を表示する言語が決めます。 既定の言語設定は、サイトが最初に作成された場合に設定され、後で変更することはできません。 手動セットアップを続行する前に、ターゲット サイトの既定の言語でOKを確認してください。

1.  [通信サイトSharePoint] で、[サイト **設定**  >  **すべての** サイト設定を表示  >  **する言語の設定**]  >  **を選択します**。 
2.  [複数の **言語に翻訳するページ** とニュースを有効にする] スイッチを [オン] に **設定します**。
    - [言語] の一覧の上部に表示される言語で問題ない場合は、追加の言語を追加し、[保存] をクリック **します**。 手順 2 に進みます。
    - サイトで選択されている言語とは異なる既定の言語が必要な場合は、必要な言語で新しい SharePoint コミュニケーション サイトを作成する必要があります。 オプション 3 に進む。 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>オプション #3 - 多言語サポートが必要ですが、サイトに別の既定の言語が必要です
このオプションを使用して、必要な既定SharePointを使用して新しいオンライン通信サイトを作成し、サイトの言語設定を設定します。 
1.  新しい通信サイトをSharePointするには、「オンラインで通信サイトを作成する[」をSharePointしてください](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)。 サイトを作成する場合は、学習経路に必要な既定の言語に言語を設定してください。 
2. 作成したサイトで、[サイト情報設定  >    >  **すべてのサイト設定を表示する 言語の設定**  >  **] を選択します**。 
2.  [複数の **言語に翻訳するページ** とニュースを有効にする] スイッチを [オン] に **設定します**。
3. 必要に応じて言語を追加し、[保存] を **クリックします**。 
4. 手順 2 に進みます。 

>![メモ]カスタム コンテンツをサイトから新しく作成されたサイトに移行する必要がある場合は、このドキュメントの「カスタム コンテンツの移行」セクションを参照してください。 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>手順 2 - Web パーツ パッケージとセットアップ スクリプトを次の手順から取得GitHub
セットアップ プロセスの一環として、Web パーツ パッケージMicrosoft 365 PowerShell セットアップ スクリプトを使用する必要があります。

- リポジトリの[学習経路GitHub移動します](https://github.com/pnp/custom-learning-office-365)。
- [ **ダウンロード] を** クリックして、Web パーツ パッケージとスクリプトをローカル ドライブに保存します。 このプロセスの後の手順で、スクリプトと Web パーツ パッケージを使用します。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>手順 2 - アップロード Web パーツをテナント アプリ カタログに追加する
ラーニング パスMicrosoft 365設定するには、customlearning.sppkg ファイルをテナント全体のアプリ カタログにアップロードして展開します。 アプリ[カタログにアプリを](/sharepoint/use-app-catalog)追加する方法の詳細については、「アプリ カタログを使用して、SharePoint Online 環境でカスタム ビジネス アプリを使用する」を参照してください。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>手順 3 - 最新の通信サイトをプロビジョニング/識別する
既存の通信サイトをSharePointするか、オンライン テナントに新しい通信サイトをSharePointします。 通信サイトを準備する方法の詳細については、「SharePoint Online で通信サイトを作成する」を参照し[、](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)手順に従って通信サイトを作成します。

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>手順 4 - サイトにMicrosoft 365パス アプリを追加する

1. このサイトSharePoint、[システム] メニューをクリックし、[アプリの追加 **] をクリックします**。 
2. [**アプリ] の** 下の [**組織から**] をクリックし、[組織の学習経路] をクリック **Office 365。** 

## <a name="step-5---set-permissions-for-the-site"></a>手順 5 - サイトのアクセス許可を設定する
サイトに対して次のアクセス許可が設定されている必要があります。
- **サイト コレクション管理者または** 所有者グループの一部 - 最初に使用する学習経路を設定する CustomConfig リスト アイテムを初期化するために必要なアクセス許可。 
- **メンバー グループ** - コンテンツの非表示と表示、カスタム プレイリストの管理など、学習経路の管理に必要なアクセス許可
- **[訪問者] グループ** - サイト コンテンツを表示するために必要なアクセス許可。 

## <a name="step-6--execute-powershell-configuration-script"></a>手順 6- PowerShell 構成スクリプトの実行
PowerShell スクリプトが含まれているので、ソリューションで使用する 3 つのテナント プロパティを作成するために実行 `CustomLearningConfiguration.ps1` する必要があります。 [](/sharepoint/dev/spfx/tenant-properties) さらに、このスクリプトはサイト ページ[](/sharepoint/dev/spfx/web-parts/single-part-app-pages)ライブラリに 2 つの単一パーツ アプリ ページを作成し、管理者とユーザーの Web パーツを既知の場所でホストします。

1. オンライン管理シェルのダウンロードがまだSharePoint場合は、今すぐダウンロードしてください。 [「SharePoint管理シェルのダウンロード」を参照してください](https://go.microsoft.com/fwlink/p/?LinkId=255251)。
2. スクリプトを実行するには、PowerShell 実行ポリシーを設定する必要がある場合があります。 詳細については、「実行ポリシー [について」を参照してください](/powershell/module/microsoft.powershell.core/about/about_execution_policies)。
3. スクリプトを実行 `CustomLearningConfiguration.ps1` します。 テナント管理者の資格情報に加えて、スクリプトによってテナント名とサイト名の入力を求めるメッセージが表示されます。 サイト URL の次の例を考慮すると、テナント名は、 `https://contoso.sharepoint.com/sites/O365CL` `contoso` サイト `O365CL` 名です。 

### <a name="disabling-telemetry-collection"></a>テレメトリ コレクションの無効化
このソリューションの一部には、匿名化されたテレメトリ追跡オプトインが含まれます。既定ではオンに設定されています。 手動インストールを行い、テレメトリ追跡をオフにする場合は、スクリプトを変更して $optInTelemetry 変数を $falseに設定し `CustomlearningConfiguration.ps1` 、スクリプトを実行します。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>プロビジョニングの成功を検証し、CustomConfig リストを初期化する

PowerShell スクリプトが正常に実行されると、サイトに移動し、最初に使用する学習経路を設定する **CustomConfig** リスト アイテムを初期化し、サイトが動作している検証を行います。

- `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`に移動します。 **CustomLearningAdmin.aspx** を開くと、初めて使用するためのラーニング パスを設定する **CustomConfig** リスト アイテムが初期化されます。 次のようなページが表示されます。

![管理者アプリのpage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>サイトに所有者を追加する
テナント管理者として、サイトをカスタマイズするユーザーになる可能性は低いので、少数の所有者をサイトに割り当てる必要があります。 所有者はサイトに対する管理者権限を持ち、サイト ページを変更したり、サイトのブランドを変更したりすることができます。 また、学習経路 Web パーツを通じて配信されるコンテンツを非表示にし、表示する機能も備っています。 さらに、カスタム プレイリストを作成し、カスタム サブカテゴリに割り当てる機能も備えます。  

1. [アクセス許可 **SharePoint設定]** メニューの [**サイトのアクセス許可] をクリックします**。
2. [**高度なアクセス許可] 設定 をクリックします**。
3. [**所有者] の [ラーニング パスOffice 365クリックします**。
4. [**新**  >  **しいユーザーをこのグループに追加** する] をクリックし、所有者になるユーザーを追加します。 
5. [共有] メッセージで [[サイトの](custom_exploresite.md) 探索] へのリンクを追加し、[共有] を **クリックします**。

## <a name="migrate-custom-content"></a>カスタム コンテンツの移行
上記の手順に従って学習パス サイトを再確立した後 **、CustomPlaylists** リストと CustomAssets リストの内容を **移動する必要** があります。 また、必要に応じて、カスタム アセットを構成する実際のカスタム ページを、既存の学習経路サイトに住んでいる場合に移動し、そのページを削除する目的で移動することもできます。 **CustomPlaylists** リスト内のすべてのアイテムに対して **、CustomAssets** リスト内のリスト アイテムの ID が各プレイリスト リスト アイテムの JSONData フィールドに埋もれているため、タスクが困難になる可能性があります。 そのため **、CustomPlaylists** リストのコンテンツをあるサイトから別のサイトに移動するだけでは十分ではありません。 さらに **、CustomAssets リスト** には、リスト アイテムの JSONData フィールドにあるカスタム アセットのページへの絶対 URL が含まれる。 アセットが移動され、サイトの名前が変更されない場合 (したがって、絶対 URL をアセットのページに変更 **)、CustomAssets はそのまま** 残ります。 ただし、エントリを手動で修正する必要があります。 移行のこの種類の複雑さを考えると、この移行を支援するために、学習経路パートナーの 1 つを参加させる方法を検討してください。 

### <a name="next-steps"></a>次の手順
- 「学習 [経路のカスタマイズ」を参照してください](custom_overview.md)。 
- 「サイト [ページの翻訳」を参照してください](custom_translate_page_ml.md)。