---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 learning の経路設定オプション
ms.date: 02/11/2019
description: カスタム学習設定のセットアップオプション
ms.openlocfilehash: 6906b5e70b186c106b3a9969b5bce1cbe87d7021
ms.sourcegitcommit: f4c2b6ef531d2d820c3d97871e187d0a2220d8f4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/04/2019
ms.locfileid: "37956654"
---
# <a name="learning-pathways-setup-options"></a>学習経路設定オプション
ラーニング経路を使用すると、さまざまな方法でソリューションを柔軟にセットアップできます。 次のセクションでは、使用可能なオプションの概要を示します。

> [!IMPORTANT]
> 組織内で Office 365 のカスタム学習機能を既にプロビジョニングしていて、ソリューションを更新する場合は、「 [Microsoft 365 Learning ・パスの ReadMe](https://github.com/pnp/custom-learning-office-365)」の「ソリューションを更新する」の手順に従ってください。 初めて Microsoft 365 learning の経路情報をプロビジョニングする場合は、「microsoft 365 learning の経路」のドキュメントの「 [microsoft 365 learning のラーニングをプロビジョニング]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision)する」の手順を参照してください。  


## <a name="recommended---sharepoint-online-provisioning-service-setup"></a>推奨-SharePoint Online プロビジョニングサービスのセットアップ 
SharePoint Online プロビジョニングサービスは、カスタム学習を設定するための最も高速で簡単な方法として推奨される方法を提供します。 SharePoint Online プロビジョニングサービスでは、Office 365 テナント管理者がサービスにサインインしていくつかの選択を行い、[**テナントに追加**] をクリックしてカスタム学習サイトとカスタム学習 Web パーツをプロビジョニングします。 プロビジョニングが完了すると、テナント管理者はサイトの準備が整ったことを示す電子メールを受信します。 

- SharePoint のプロビジョニングサービスを開始するには、「 [PnP プロビジョニングサービスを使用してプロビジョニング](custom_provision.md)する」にアクセスしてください。   

## <a name="stand-alone-learning-pathways-web-part-setup"></a>スタンドアロンの学習経路 web パーツのセットアップ
既に確立されている SharePoint Online のモダンコミュニケーショントレーニングポータルがある組織では、既存の SharePoint Online サイトに Microsoft 365 learning の経路の web パーツを手動でインストールするオプションがあります。 サイトは、最新の SharePoint Online サイトである必要があることに注意してください。 このメソッドには、テナント管理者のアクセス許可と、Windows PowerShell または SharePoint Online 管理シェルを使用した環境が必要です。 この方法では、SharePoint Online プロビジョニングサービスのセットアップにより多くの技術的な専門知識が必要になることに注意してください。

- 手動による web パーツのインストール手順については、「 [web パーツを手動でインストールする](custom_manualsetup.md)」を参照してください。 

## <a name="update-learning-pathways"></a>学習経路を更新する
SharePoint Online プロビジョニングサービスを使用して以前のバージョンの Microsoft 365 をインストールした組織では、ソリューションを最新バージョンに更新することができます。 ソリューションの最新バージョンに対して展開されたバージョンを確認する方法、およびソリューションを更新する方法の手順については、 [ReadMe ファイル](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)の「ソリューションを更新する」セクションを参照してください。

### <a name="next-steps---provision-microsoft-365-learning-pathwayscustom_provisionmd"></a>次のステップ- [Microsoft 365 learning の経路をプロビジョニング](custom_provision.md)する
