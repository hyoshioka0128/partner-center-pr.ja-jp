---
title: パートナー セキュリティ要件の状態
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: クラウド ソリューション プロバイダー プログラムにおけるアドバイザー、コントロール パネル ベンダー、およびパートナーのセキュリティを強化する、新しい必須要件について説明します。
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, クラウド ソリューションプロバイダー, クラウド ソリューション プロバイダー プログラム, CSP, コントロール パネル ベンダー, CPV, 多要素認証, MFA, 安全なアプリケーション モデル, セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: b842566245eaf7a874535fd081da51424316d417
ms.sourcegitcommit: 3a1c0934ff337fc164bee690e7b9d69d113fdb99
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "84328183"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>パートナー セキュリティ要件の状態 - 現在の状態に関する回答を入手し、レポートを確認する

**適用対象**

- クラウド ソリューション プロバイダー プログラムのすべてのパートナー
  - 直接請求
  - 間接プロバイダー
  - 間接リセラー
- すべてのコントロール パネル ベンダー
- すべてのアドバイザー

**該当するユーザー**
- ゲスト ユーザーを含むすべての有効なユーザー

プライバシーの保護とセキュリティの強化は、マイクロソフトの最優先事項の 1 つです。 最善の防御とは予防することで、私たちの強さが、最も弱いリンクと同程度でしかないことはわかっています。 だから、エコシステムの全員が行動し、適切なセキュリティ保護を確保する必要があるのです。 パートナーと顧客を保護するために、アドバイザー、コントロール パネル ベンダー、およびクラウド ソリューション プロバイダー プログラムに参加しているパートナーを対象とした一連の必須セキュリティ要件が導入されています。

2019 年 8 月 1 日以降、すべてのパートナーが、パートナー テナントのすべてのユーザー (サービス アカウントを含む) に対して多要素認証を適用する必要があります。 新しいセキュリティ ポリシーの詳細については、「[パートナー セキュリティ要件](partner-security-requirements.md)」を参照してください。

Microsoft では、各ユーザーが 1 つの認証ごとに確実に MFA チャレンジを受けるように取り組んでいます。 このエクスペリエンスは、次のいずれかの方法で実現できます。

- Azure AD Premium を実装し、MFA が各ユーザーに確実に適用されるようにする
- [Azure AD のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)を実装する
- サードパーティ ソリューションを実装し、MFA が各ユーザーに確実に適用されるようにする

## <a name="partner-security-requirements-status"></a>パートナー セキュリティ要件の状態

このレポートを使用すると、要件を満たしていない可能性がある個所が示されるので、セキュリティ要件の状態を確認できます。 追跡は定期的に更新されます。

>[!NOTE]
>パートナー セキュリティ要件の状態レポートは、パートナー センターでのみサポートされています。 Microsoft Cloud for US Government または Microsoft Cloud Germany では使用できません。 ソブリン クラウド (21Vianet、米国政府、およびドイツ) を介して取引するすべてのパートナーには、これらの新しいセキュリティ要件を採用することを強くお勧めします。 ただし、これらのパートナーは、2019 年 8 月 1 日に開始される新しいセキュリティ要件を満たす必要はありません。 マイクロソフトでは、今後、ソブリン クラウドに対するこれらのセキュリティ要件の適用に関して、追加の詳細情報を提供する予定です。

## <a name="multi-factor-authentication-mfa-report"></a>多要素認証 ("MFA") レポート

パートナー センターの MFA レポートには、CSP テナントの MFA 構成とパートナー センターのアクティビティに基づいた 2 種類のメトリックが用意され、パートナーの MFA の実装に関する分析情報が示されます。 

### <a name="mfa-configuration-on-a-csp-tenant"></a>CSP テナントでの MFA 構成

このメトリックは、1 日単位でキャプチャおよび報告した CSP テナントの MFA 構成に関連しています。 これらの [MFA オプション](https://aka.ms/partner-mfa-get-started)のいずれかを使用して、MFA が適用された有効なユーザー アカウントの割合を測定します。 たとえば、次のように入力します。

- Contoso は、テナントに 110 個のユーザー アカウントを持つ CSP パートナーであり、そのユーザー アカウントのうち 10 個は無効になっています。 
- 残りの 100 個のユーザー アカウントのうち、90 個は、指定された [MFA オプション](https://aka.ms/partner-mfa-get-started)を使用して MFA が適用されます。 そのため、メトリックには 90% と示されます。 

### <a name="partner-center-activities-with-mfa"></a>MFA を使用したパートナー センター アクティビティ

従業員がパートナー センターにサインインして作業したり、API を介してパートナー センターからデータを取得または送信したりするたびに、セキュリティ状態のチャレンジが行われ、追跡されます。 また、セキュリティ状態の追跡には、自社のアプリケーションと、すべてのコントロール パネル ベンダー アプリケーションも含まれます。 過去 7 日間の状態が表示されます。

#### <a name="mfa-verification-completed-by-users"></a>MFA verification completed by users (ユーザーが完了した MFA 検証)

このメトリックは、パートナー センター ダッシュボード内のアクティビティに関連しています。 MFA 検証を完了したユーザーによって行われた操作の割合が測定されます。 たとえば、次のように入力します。

- Contoso は、加藤さんと田中さんという 2 人の管理者エージェントがいる CSP パートナーです。
- 初日に、加藤さんは MFA 検証を完了せずにパートナー センター ダッシュボードにログインし、3 つの操作を行いました。
- 2 日目に、田中さんは MFA 検証を完了せずにパートナー センター ダッシュボードにログインし、5 つの操作を行いました。
- 3 日目に、加藤さんは MFA 検証を完了してパートナー センター ダッシュボードにログインし、2 つの操作を行いました。
- 残りの 4 日間は、どちらのエージェントも操作を行いませんでした。
- 7 日間に実行された 10 個の操作のうち、ユーザーが MFA 検証を完了して行ったものは 2 回でした。 そのため、メトリックには 20% と示されます。

ファイル **[Portal requests without MFA]\(MFA なしのポータル要求\)** を使用すると、MFA 検証なしでパートナー センター ダッシュボードにログインしたユーザーと、レポート期間中に最後にアクセスした時刻を把握できます。

#### <a name="appuser-authentication"></a>App+User authentication (アプリ + ユーザー認証)

このメトリックは、[App+User authentication]\(アプリ + ユーザー認証\) を使用して行われたパートナー センター API 要求の使用に関連しています。 MFA 要求と共にアクセス トークンを使用して行われた API 要求の割合が測定されます。 たとえば、次のように入力します。

- Fabrikam は CSP パートナーであり、[App+User authentication]\(アプリ + ユーザー認証\) とアプリのみの認証方法を組み合わせて使用する CSP アプリケーションを持っています。
- 初日に、アプリケーションでは、MFA 検証を完了せずに、[App+User authentication]\(アプリ + ユーザー認証\) 方法を介して取得されたアクセス トークンを利用して、3 つの API 要求を作成しました。
- 2 日目に、アプリケーションでは、[App-only authentication]\(アプリのみの認証\) を介して取得されたアクセス トークンを利用して、5 つの API 要求を作成しました。
- 3 日目に、アプリケーションでは、MFA 検証を完了し、[App+User authentication]\(アプリ + ユーザー認証\) 方法を介して取得されたアクセス トークンを利用して、2 つの API 要求を作成しました。
- 残りの 4 日間は、どちらのエージェントも操作を行いませんでした。
- [App-only authentication]\(アプリのみの認証\) を介して取得されたアクセス トークンを利用した 2 日目の 5 つの API 要求は、ユーザーの資格情報を使用しないため、メトリックから除外されます。 残りの 5 つの操作のうち、2 つでは MFA 検証を完了して取得されたアクセス トークンを利用しました。 そのため、メトリックには 40% と示されます。

このメトリックで 100% の結果ではない [App+user activities]\(アプリ + ユーザー アクティビティ\) を把握するには、次のファイルを使用します。

- **[API requests summary]\(API 要求の概要\)** 。アプリケーションごとの全体的な MFA 状態を把握できます。
- **[All API requests]\(すべての API 要求\)** 。テナントのユーザーによって行われた各 API 要求の詳細を把握できます。ダウンロード エクスペリエンスを向上させるために、結果は最新の 10,000 件の要求までに制限されます。

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>MFA レポートのメトリックが 100% ではない場合の対処方法

MFA を実装しているパートナーの場合、パートナー センターの MFA レポートのメトリックが 100% ではないことがあります。 その理由を理解するために、考慮する必要がある要素を次に示します。

> [!NOTE]
> パートナー テナントの ID 管理と MFA の実装について理解している組織のユーザーと協力する必要があります。

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>パートナー テナント用に MFA を実装しましたか

それ以外の場合は、最初にパートナー テナント用に MFA を実装する必要があります。 MFA を実装する方法の詳細については、「[パートナーのセキュリティ要件](partner-security-requirements.md)」を参照してください。

### <a name="have-you-only-recently-completed-mfa-implementation"></a>最近、MFA の実装を完了したばかりですか

メトリックは日単位で計算され、過去 7 日間に実行された操作が考慮されます。 パートナー テナントの MFA 実装を最近完了したばかりの場合は、メトリックが 100% ではない可能性があります。

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>一部のユーザー アカウントが MFA 実装から除外されていますか

現在の MFA 実装の対象がすべてのユーザー アカウントか一部のみかを把握します。 一部の MFA ソリューションはポリシーベースであり、ユーザーの除外をサポートしますが、ユーザーごとに MFA を明示的に有効にすることが必要な場合もあります。 現在の MFA 実装からユーザーを除外していないことを確認します。 除外されたユーザー アカウントが、パートナー センターにログインして CSP 関連のアクティビティを実行すると、メトリックが 100% にならない可能性があります。

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>MFA は特定の条件が満たされた場合にのみ必要ですか

現在ご利用の実装では、特定の条件下でのみ MFA が適用されるかどうかを把握します。 一部の MFA ソリューションには、特定の条件が満たされた場合にのみ MFA を適用する柔軟性があります。 たとえば、ユーザーは不明なデバイスまたは不明な場所からアクセスしています。 MFA は有効ですが、パートナー センターにアクセスするときに MFA 検証を完了する必要がないユーザーがいると、メトリックが 100% にならない可能性があります。

>[!NOTE]
>Azure AD のセキュリティの既定値を使用して MFA を実装したパートナーの場合、管理者以外のユーザー アカウントにはリスクに基づいて多要素認証が適用されることに注意することが重要です。 ユーザーには、リスクの高いサインイン試行時にのみ MFA が求められます (たとえば、ユーザーが別の場所からサインインする場合など)。 さらに、ユーザーは、MFA への登録が完了するまでに最大 14 日間かかります。 MFA の登録を完了していないユーザーには、この 14 日間に MFA 検証のチャレンジが行われません。 そのため、Azure AD のセキュリティの既定値を使用して MFA を実装したパートナーの場合、メトリックが 100% にならない可能性があると予想されます。

### <a name="are-you-using-third-party-mfa-solution"></a>サードパーティの MFA ソリューションを使用している場合

サードパーティの MFA ソリューションを使用している場合は、それを Azure AD と統合する方法を確認してください。 一般に、フェデレーションとカスタム コントロールを含む 2 つの方法があります。

* **ID フェデレーション** - Azure AD が認証要求を受け取ると、Azure AD では認証のためにフェデレーション ID プロバイダーにユーザーをリダイレクトします。 認証に成功すると、フェデレーション ID プロバイダーでは、ユーザーを SAML トークンと共に Azure AD にリダイレクトします。 フェデレーション ID プロバイダーに対する認証時にユーザーが MFA 検証を完了したことを Azure AD が認識できるようにするには、SAML トークンに (値 *multipleauthn* を指定して) *authenticationmethodsreferences* 要求を含める必要があります。 フェデレーション ID プロバイダーがこのような要求の発行をサポートしているかどうかを確認してください。 その場合、この処理を実行するようにフェデレーション ID プロバイダーが構成されているかどうかを確認します。 この要求がない場合、Azure AD (およびパートナー センター) ではユーザーが MFA 検証を完了したことが認識されないため、要求がないとメトリックが 100% にならない可能性があります。

* **カスタム コントロール** - Azure AD カスタム コントロールを使用して、ユーザーがサードパーティの MFA ソリューションによる MFA 検証を完了したかどうかを特定することはできません。 その結果、カスタム コントロールを介して MFA 検証を完了したユーザーは、常に Azure AD (およびパートナー センター) からは MFA 検証を完了していないように見えます。 可能であれば、Azure AD との統合時に、カスタム コントロールではなく、ID フェデレーションの使用に切り替えることをお勧めします。

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>MFA を完了せずにパートナー センターにログインしたユーザーを特定する

MFA 検証を完了せずにパートナー センターにログインしているユーザーを特定し、現在の MFA の実装に照らして検証すると便利な場合があります。 [Azure AD サインイン レポート](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)を使用すると、ユーザーが MFA 検証を完了したかどうかを確認できます。 Azure AD サインイン レポートは、現在、Azure AD Premium、または Azure AD Premium を含む任意の O365 SKU (EMS など) にサブスクライブしているパートナーのみが利用できます。

**詳細情報**

- [パートナー センター セキュリティ ガイダンス グループ コミュニティ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [パートナー センターのセキュリティ要件](partner-security-requirements.md)
- [パートナー センターのセキュリティ要件についてよく寄せられる質問](partner-security-requirements-faq.md)
