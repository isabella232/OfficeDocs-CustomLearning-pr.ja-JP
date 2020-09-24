---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学習経路のトラブルシューティング
ms.date: 02/10/2019
description: Microsoft 365 学習経路のトラブルシューティング方法について説明します。
ms.service: sharepoint online
ms.openlocfilehash: 8d8b418c7a4b2c025391eb4527af86b02738c532
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233869"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Microsoft 365 学習経路のトラブルシューティング

ここでは、Microsoft 365 の学習経路または SharePoint Online プロビジョニングサービスで発生する可能性のある問題のトラブルシューティングのヒントを示します。

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>テナント管理者のアクセス許可があるかどうかを確認する方法

SharePoint Online プロビジョニングサービスにサインインし、カスタム学習を準備するには、テナント管理者のアクセス許可が必要です。 SharePoint Online プロビジョニングサービスでサインインに関する問題が発生している場合は、全体管理者の役割が割り当てられていることを確認してください。 カスタム学習ソリューションには、テナント管理者のアクセス許可が必要です。それ以外の場合は、Office 365 のグローバル管理者ロールと呼ばれます。 グローバル管理者の役割が割り当てられているかどうかを確認する方法は次のとおりです。

1.  Office.com にサインインします。
2.  [**管理**] をクリックします。
3.  [**ユーザー**] で、[**アクティブなユーザー** ] を選択します。
4.  自分の名前を検索する
5.  [検索結果] で自分の名前をクリックします。 役割の全体管理者が表示します。

![cg-globaladminrole.png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>グローバル管理者の役割を持っていない場合
- 組織内のグローバル管理者を検索して、そのユーザーがサービスにサインインしたり、グローバル管理者の役割を割り当てたりするようにします。

## <a name="tenant-app-catalog-troubleshooting"></a>テナントのアプリカタログのトラブルシューティング
カスタム学習では、ターゲットテナントにアプリカタログをプロビジョニングする必要があります。 アプリカタログを作成するには、グローバル管理者のアクセス許可が必要です。 一般的なアプリカタログの問題のトラブルシューティング手順を以下に示します。

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>テナントアプリカタログがあるかどうかを確認する方法 
手始めとして、全体管理者のアクセス許可があることを確認します。 前述のテナント管理者権限の手順を参照してください。

1. Office 365 で、[**管理者**] をクリックし > [展開] の矢印をクリックし、[すべての**Show all**  >  **管理センター**  >  の**SharePoint**を表示] をクリックします。
2. [**従来の管理者 SharePoint センター**  >  **アプリ**  >  の**アプリカタログ**] をクリックします。
3. [ **アプリ**] の下に、[ **SharePoint 用アプリの配布**] というタイトルのタイルが表示します。 タイルが表示されている場合は、テナントのアプリカタログがあります。 下記の「サイトの詳細を **確認する方法** 」セクションを参照してください。 タイルが表示されない場合は、テナントのテナントアプリカタログを作成する必要があります。 「 **How to create a Tenant App Catalog** 」セクションを参照してください。

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>テナントアプリカタログのサイトコレクションの所有者であることを確認する方法 
Microsoft 365 learning の経路をプロビジョニングするには、テナントのアプリカタログのサイトコレクションの所有者である必要があります。 所有者であるかどうかを判断する方法は次のとおりです。

1. Office 365 で、[**管理者**] をクリックし > [展開] の矢印をクリックし、[すべての**Show all**  >  **管理センター**  >  の**SharePoint**を表示] をクリックします。
2. [ **従来の管理者 SharePoint センター**] をクリックし、 **アプリカタログ**を選択します。
3. [ **所有者**] を選択し、サイトコレクションの所有者であることを確認します。 これは次のようなものになります。
 
![cg-sitecollectionowner.png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>テナントのアプリカタログを作成する方法 (存在しない場合) 
1. SharePoint Online 管理者アカウントを使用して、Office 365 にサインインします。
2. **[管理者]** をクリックします。
3. [ **管理センター**] で、[ **SharePoint**] をクリックします。 
4. [**アプリ**  >  **アプリカタログ**] をクリックします。
5. [ **新しいアプリカタログサイトを作成する**] をクリックし、[ **OK**] をクリックします。 
6.  アプリカタログの情報を入力します。 複数の管理者を含めることができます。 次に例を示します。  

![cg-appcatalogfinish.png](media/cg-appcatalogfinish.png)

7.  これで完了です。 完了しました。 ただし、カスタム学習のプロビジョニングに移行する前に、アプリカタログの作成が完了したことを確認するために、少なくとも30分待機する必要があります。 

> [!IMPORTANT]
> テナントのアプリカタログを作成した後、少なくとも30分待ってから、カスタム学習をプロビジョニングします。 これにより、アプリカタログのプロビジョニングプロセスが SharePoint 内で完了するようになります。 