---
title: 支払いと収益の問題のトラブルシューティング
ms.topic: article
ms.date: 06/29/2020
description: 収益の不足や不適切な利益、適格性の問題、インセンティブ収益の調整方法などの問題を解決する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 352499e96c69e9f59190aaf6fa1c43d2d0f8ed59
ms.sourcegitcommit: bea864212edc90c5f851566505deef6623f79723
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2020
ms.locfileid: "85719361"
---
# <a name="troubleshooting-payments-and-earnings-issues"></a>支払いと収益の問題のトラブルシューティング

適用対象:

- パートナー センター

この記事は、インセンティブプログラムの利益や支払いの問題を解決するのに役立ちます。 記載されているトピックには、支払いのタイミング、収益の適格性の確認、支払いと税金のプロファイルを適切に設定することの重要性が含まれます。

適切なロール:

- インセンティブ管理者

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>組織の支払いと税金のプロファイルを作成または更新できるのはだれですか?

パートナーセンターで、関連するインセンティブプログラムと MPN の場所のインセンティブ管理者ロールを持つユーザーは、組織の支払いと税金のプロファイルを更新して表示できます。

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>保留中の支払い/税務プロファイルの承認には、どのくらい時間がかかりますか?

検証には最大 48 時間かかることがあります。 その間、[概要] ページのプロファイルの状態は "登録の検証中" になります。 プロセスが完了すると、状態は [成功した場合は**登録**済み]、または必要に応じて [**アクションが必要]** と表示されます。

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>支払いおよび税務プロファイルが正しく完了しているかどうかを確認するには、どうすればよいですか?

登録の状態は [概要] ページに表示されます。 プロファイルの作成が完了すると、状態が [**登録の検証**中] になります。 情報が検証されると、状態が [**登録**済み] に変わります。 これは、支払いおよび税務プロファイルの登録が正常に完了したことを示しています。

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>税務プロファイルを更新しないと、そのプロファイルを新しいインセンティブ プログラムで使用できないのはなぜですか?

インセンティブの支払いは、インセンティブの種類に応じて、さまざまな場所から行われます。 適切な処理を実行するには、場所によってはインセンティブ プログラム ルールに基づいて、追加の税務情報が必要になる場合があります。

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>支払い/税務プロファイルを削除するには、どうすればよいですか?

現在、既存の支払いおよび税務プロファイルを削除するオプションはサポートされていません。

## <a name="my-payment-is-missing-or-incorrect"></a>支払いが不足しているか、正しくありません

支払いが見つからないか正しくない場合、次のいずれかが原因であることがよくあります。

- **資格がない可能性があります。**  収益は、運用資格の要件を満たしている場合、またはそれぞれのプログラムの使用期間に登録されている場合にのみ利用できます。
- **要件を満たしていない可能性があります。**  探しているインセンティブの資格と適格な収益ルールが満たされているかどうかを確認します。

  **資格を確認するには**

  1. パートナーセンターにサインインします。[パートナーインセンティブ](https://partner.microsoft.com/membership/partner-incentives)。
  
  2. プログラムのドキュメントまで下にスクロールします。
  
  3. 目的のドキュメントリンクを選択し、「**パートナーの資格**と適格な**収益ルール**」セクションを確認します。

- **支払いプロファイルが不完全である可能性があります。** インセンティブの利益の開始日は、支払いと税金の詳細を含むオンボードを含む、すべての資格要件を完了した月の最初の日になります。 収益は、支払いと税金の完了前の月には使用できません。 たとえば、2020年4月にすべての要件を完了すると、収益の開始日は2020年4月1日になります。
- **未処理のアクションがある可能性があり**ます。  未処理のアクションが保留中になっているため、インセンティブが処理されていない可能性があります。

  **未処理のアクションを表示するには**

  1. パートナーセンターにサインインします。[パートナーインセンティブ](https://partner.microsoft.com/membership/partner-incentives)。
  2. [**トランザクションの履歴**] ページを開きます。 このページのフィールドを確認して、**保留中の税プロファイル**、**保留中の支払いプロファイル**、または**保留中の税金請求書の送信**など、未処理のアクションを実行します。

これらのアクションが役に立ちませんが、支払いがまだ見つからないか間違っている場合は、[サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>協力申請の支払いが 2 つの異なる通貨で行われるのはなぜですか?

さまざまな Microsoft エンティティから協力ファンドが取得されるとき、エンティティごとに現地通貨で支払いが行われます。  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>協力申請の通貨以外で支払いが行われたのはなぜですか?

すべてのインセンティブ プログラムに、セットアップ中に作成された銀行プロファイルがあります。 そのプロファイルで指定された通貨は、支払いが行われる通貨です。

## <a name="i-dont-see-earnings-for-a-certain-period"></a>特定の期間の収益が表示されない

予想される期間の収益が表示されない場合は、通常、次のいずれかの問題が原因です。

- **資格がない可能性があります。**  収益は、運用資格の要件を満たしている場合、またはそれぞれのプログラムの使用期間に登録されている場合にのみ利用できます。

- **支払いプロファイルが不完全である可能性があります。**  インセンティブの利益の開始日は、支払いと税金の詳細を含むオンボードを含む、すべての資格要件を完了した月の最初の日になります。 収益は、支払いと税金の完了前の月には使用できません。 たとえば、2020年4月にすべての要件を完了すると、収益の開始日は2020年4月1日になります。

支払いと税金の詳細を使用したオンボードなどの有資格要件を満たしていても、収益がまだない場合は、[サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。

## <a name="my-earnings-are-missing-or-incorrect"></a>収益が不足しているか、正しくありません

次のいずれかの問題が原因で、存在しない、または正しくない収益が発生している可能性があります。

- **要件を満たしていない可能性があります。**  探しているインセンティブの[資格](#my-payment-is-missing-or-incorrect)と適格な収益ルールが満たされているかどうかを確認します。

- **不一致がある可能性があります。**  パートナーの資格と適格な収益の両方のルールを満たしていても、誤った収益が見られる場合は、すべての収益とそれぞれの取引にアクセスする手順について、 [& の支払いの不一致を特定する方法](https://support.microsoft.com/help/4534675)をご覧ください。

これらのアクションが役に立ちませんが、まだ収益を得られない場合や、収益が間違っていると思われる場合は、[サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。

## <a name="how-do-i-reconcile-my-earnings"></a>収益を調整操作方法

収益に違いがある場合は、次の手順を実行します。

1. **収益の資格があることを確認します。**  収益は、運用資格の要件を満たしている場合、またはそれぞれのプログラムの使用期間に登録されている場合にのみ利用できます。

2. **支払いプロファイルが完了していることを確認します。**  インセンティブの利益の開始日は、支払いと税金の詳細を含むオンボードを含む、すべての資格要件を完了した月の最初の日になります。 収益は、支払いと税金の完了前の月には使用できません。 たとえば、2020年4月にすべての要件を完了すると、収益の開始日は2020年4月1日になります。 

3. **要件を満たしていることを確認します。**  探しているインセンティブの[資格](#my-payment-is-missing-or-incorrect)と適格な収益ルールが満たされているかどうかを確認します。

4. **不一致があるかどうかを判断します。**  パートナーの資格と適格な収益の両方のルールを満たしていても、誤った収益が見られる場合は、すべての収益とそれぞれの取引にアクセスする手順について、 [& の支払いの不一致を特定する方法](https://support.microsoft.com/help/4534675)を参照してください。

これらのアクションが役に立ちませんが、収益がまだ調整されていない場合は、[サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。

## <a name="where-can-i-find-my-rates"></a>料金はどこで確認できますか。

1. [[Partner incentives]\(パートナー インセンティブ\)](https://partner.microsoft.com/membership/partner-incentives) に移動してサインインします。

2. サインインしたら、下にスクロールして興味のあるプログラムのドキュメントにアクセスし、該当するプログラムのドキュメント リンクをクリックします。

3. ドキュメントの「**プログラムの構造と料金**」セクションを参照してください。