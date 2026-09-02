---
id: TechnicMoveHubConfigurations
title: Technic Move Hub の設定
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Technic Move Hub の設定

## 概要

Technic Move Hub は、LEGO Powered Up ハブ ファミリーに独自の機能を導入しました。現在適用されている設定に応じて、ハブの動作を変更できます。

MOCPilot では Technic Move Hub の設定を変更し、操作したい公式 LEGO セットの動作に合わせることができます。

## 対応設定

現在、次の Technic Move Hub 設定が知られています。

- **Porsche GT4 e-Performance**
- **Lamborghini Revuelto**
- **Batmobile™ Tumbler**

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_4.png')} alt="Technic Move Hub の設定オプション" />

## 自分の Bluetooth ハブから設定を変更する

設定は **自分の Bluetooth ハブ** ページから変更できます。

1. **自分の Bluetooth ハブ** を開きます。
2. Technic Move Hub を探します。
3. ハブのコンテキストメニューを開きます。
4. **設定を選択** を選択します。
5. 必要な設定を選択します。
6. 再設定ダイアログを確認します。

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_0.png')} alt="Technic Move Hub のコンテキストメニュー" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_1.png')} alt="Technic Move Hub の設定サブメニュー" />

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_3.png')} alt="Technic Move Hub の再設定確認ダイアログ" />

:::warning 重要
ハブ設定の変更では、サブプログラムをハブに書き込みます。この処理はファームウェア更新に似ています。

処理中はハブの電源を入れたままにしてください。Bluetooth 接続を安定させるため、スマートフォン、タブレット、またはコンピューターの電源を入れ、ハブの近くに置いてください。設定変更中に MOCPilot を閉じたり、Bluetooth をオフにしたり、ハブの電源を切ったりしないでください。

設定変更を中断すると、ハブのファームウェアが破損する可能性があります。その場合、再び使用する前にファームウェア復旧が必要になることがあります。復旧が必要な場合は、[ハブ ファームウェア復旧](/docs/Application/Hubs/RecoveryHubFirmware/) ガイドに従ってください。
:::

再設定中、ハブは通常のコマンドに応答しません。処理が完了するまで、LED が段階的なカラー表示で点滅します。新しい設定が適用されると、ハブは再初期化されます。

## 設定ブロック

MOCPilot には、プログラム中に Technic Move Hub の設定を読み取り、変更するためのブロックも含まれています。

### ハブ設定をセット

<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="ハブ設定をセット ブロック" />

**ハブ設定をセット** ブロックは、選択したハブを対応している設定プロファイルのいずれかに変更します。

- ハブ選択: 再設定するハブを選択します。
- 設定選択: 目標設定を選択します。
- Technic Move Hub で利用できる設定: **Porsche GT4 e-Performance**、**Lamborghini Revuelto**、**Batmobile™ Tumbler**。

[ハブ設定をセット ブロックのドキュメント](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_set_hub_config)を参照してください。

### ハブ設定

<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="ハブ設定 ブロック" />

**ハブ設定** ブロックは、選択したハブの現在の設定を報告します。

- ハブ選択: 読み取るハブを選択します。
- 出力形式: **テキスト** は設定名を返します。
- 出力形式: **インデックス** は設定インデックスを返し、条件での比較に便利です。

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_5.png')} alt="ハブ設定 ブロックの出力形式オプション" />

[ハブ設定 ブロックのドキュメント](/docs/Application/BlockBuilder/Blocks/Control/#block_hubs_all_control_hub_config)を参照してください。

### パワーパルス

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_motors_power_pulse.svg')} alt="パワーパルス ブロック" />

**パワーパルス** ブロックは、選択した Technic Move Hub にパワーパルスコマンドを送信します。このブロックは Technic Move Hub が **Batmobile™ Tumbler** に設定されている場合のみ動作します。

実行すると、ハブは利用可能な最大出力と速度で短時間モーターを動かします。通常は約 1-2 秒です。

[パワーパルス ブロックのドキュメント](/docs/Application/BlockBuilder/Blocks/Motors/#block_hubs_technicmove_motors_power_pulse)を参照してください。

## プログラム実行中に設定を変更する

プログラム実行中に Technic Move Hub の設定を変更することもできます。

一般的な方法は次のとおりです。

1. 現在のハブ設定を読み取ります。
2. プロファイルで必要な設定と比較します。
3. 設定が異なる場合は、必要な設定を適用します。
4. 再設定後に設定をもう一度読み取ります。
5. ハブが期待する設定を報告した場合のみ続行します。
6. 必要な設定が適用されなかった場合は、切断するかプログラムを停止します。

このハブを使用する組み込みプロファイルを、この実装方法の参考にできます。

<img src={useBaseUrl('/img/hubs/technic-move-hub-configurations/cfg_6.png')} alt="実行中に Technic Move Hub の設定を変更するブロック例" />
