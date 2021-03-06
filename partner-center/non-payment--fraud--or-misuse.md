---
title: 未払い、詐欺、不正使用の管理
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: オンライントランザクションに関連するさまざまなリスクと、それらのリスクを管理して軽減するためのベストプラクティスについて理解することが重要です。
keywords: 詐欺, 不正使用, 使用条件, 利用規約, 未払い, 顧客が料金を支払わない, オンライン リスク, サービスの盗用, サービスの不正使用, サブスクリプションの一時停止,
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f8ca1461ed8b71ea2e6c82603672f4029599b4cc
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991896"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>パートナー センターでの未払い、詐欺、不正使用の管理

適用対象:

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

**適切なロール**
- グローバル管理者
- ユーザー管理者
- 管理エージェント
- 課金管理者

パートナーは、顧客による不正購入や、購入サービスの料金未払いについて、金銭的な責任を負います。 したがって、*不正行為の防止と検出のリスク軽減のための制御*を行うことを強くお勧めします。

不正行為や不正使用を回避したり、これらに対処するには、潜在的なリスクを理解して、リスクへの露出を軽減するためのポリシーとプラクティスを作成することが重要です。

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Microsoft による利用規約の適用

許容される使用ポリシーに違反しているかどうかを確認するパートナーまたは顧客のアクティビティを Microsoft が検出した場合は、実施手順を実行します。 顧客はすぐに中断される可能性があります。 Microsoft からの要求に対して、実施アクションまたは更新が通知されます。

## <a name="abuse-of-service-risks"></a>サービスリスクの悪用

**サービスのリスクを悪用**すると、クラウドサービスを使用するお客様は、マイクロソフトの利用規約に違反することになります。

### <a name="examples-of-abuse-of-service"></a>サービスの悪用の例

Microsoft の利用規約に違反する例として、次のようなものがあります。

- スパム
- ハッキング
- 分散型サービス拒否 (DDoS) 攻撃
- ビットコイン マイニング
- マルウェアの配布
- 偽造されたサブスクリプションの再販

## <a name="theft-of-service-risks"></a>サービスリスクの盗難

**サービスリスクの盗難**は、消費されたサービスに対して支払いを行うことがないお客様を意味します。 この盗難には、盗まれた支払い方法の使用、誤請求情報の提供、または未払い残高の既定値の使用が含まれる場合があります。

### <a name="examples-of-service-theft"></a>サービスの盗難の例

オンライントランザクションのリスクの例としては、次のようなものがあります。

- 担当者では発生しないトランザクション ("クレジットカードが存在しません" トランザクション)
- ID の不正使用
- 初回の支払い前にプロビジョニングおよび使用されたサービス
- オンライン不正アクセスのための新たな市場や危険度の高いリージョン
- 不正なアクターによるアカウントの作成と購入を自動化する

## <a name="managing-online-risk"></a>オンラインリスクの管理

次の推奨事項を使用すると、顧客関係のライフサイクルにおいてオンライントランザクションのリスクにさらされるリスクを軽減するためのポリシーとプラクティスを開発できます。

### <a name="onboarding-new-customers"></a>新しい顧客をオンボードする

新しい顧客をオンボードするときにオンラインリスクを軽減するための推奨事項は次のとおりです。

- 可能な場合は、顧客との個人関係を確立します (たとえば、電話で顧客に連絡します)。
- お客様の資格情報とバックグラウンドをより適切な方法 (クレジット機関やビジネスコマーシャルレポート機関を使用するなど) で検証します。
- サインアップ時に multi-factor authentication (SMS の検証など) を使用して、ロボットアカウントの作成と購入の危険性を最小限に抑えます。
- サービス (デジタル id サービスなど) を使用して id を管理および追跡します。
- クレジットカード詐欺検出システムを使用して、顧客の財務力を評価します。
- コレクションのクリアポリシーを確立します。 コレクションのプロセスを詳しく説明します。サブスクリプションへのアクセスは、支払いが行われないことによって影響を受けます。 (アクセスを無効にしたり[、顧客のサブスクリプション](suspend-a-subscription.md)の支払いを中断したりすることができます)。

### <a name="managing-customer-accounts"></a>顧客アカウントの管理

購入後に顧客アカウントを管理するための推奨事項は次のとおりです。

- Microsoft 通知を迅速に受信、確認、操作、および対応するプロセスを実装します。
- お客様と協力して、クラウドの使用状況に関するビジネスニーズを把握し、設定に適切な監視しきい値を設定します。 (たとえば、パートナーセンターで[月単位の Azure 支出予算を設定](set-an-azure-spending-budget-for-your-customers.md)できます。 これにより、1か月の間に顧客の使用状況を監視し、顧客が予算に近づいたときに通知を受けることができます。)
- [顧客のアクティビティログ](activity-logs.md)を定期的に監視して、不正行為を早期に検出できるようにします。
- 疑わしいアクティビティが検出されたときにクイックアクションを実行します。
- 最初にリスク軽減制御を実装することなく、サブスクリプションへの完全な管理アクセス権を顧客に付与しないようにします。

### <a name="managing-customer-billing"></a>顧客の請求の管理

購入後のお客様の課金を管理するための推奨事項は次のとおりです。

- 初期のトランザクションと課金の前に、前払いを要求します。
- 高リスクの支払い方法 (プリペイドカードや格納済みの値のカードなど) は受け入れないでください。
- 顧客の支払いと経時勘定科目の売掛金を監視します。 遅延支払いまたは非支払いのために標準化された催促プロセスを積極的に適用します。

オンライン リスクを軽減するための詳しい方法については、[オンライン トランザクション リスクの管理ガイド](https://assets.windowsphone.com/7d885238-e13b-4f10-a682-3d5adacd2859/CSP-PartnerRiskGuide-APSFinal_InvariantCulture_Default.zip)をご覧ください。
