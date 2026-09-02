---
id: Control
title: コントロール
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# コントロール

コントロールブロックは実行フローを管理します：待機、ループ、分岐、およびスクリプトの停止。

## 待機ブロック

### `待機` (初級) {#block_control_wait_for}

<img src={useBaseUrl('/img/blocks/block_control_wait_for.svg')} alt="block_control_wait_for.svg" />

現在のスクリプトを指定した時間だけ一時停止します。

### `〜まで待機` (上級) {#block_control_wait_until}

<img src={useBaseUrl('/img/blocks/block_control_wait_until.svg')} alt="block_control_wait_until.svg" />

条件が真になるまで現在のスクリプトを一時停止します。

## ループブロック

### `繰り返し` (上級) {#block_control_repeat_for}

<img src={useBaseUrl('/img/blocks/block_control_repeat_for.svg')} alt="block_control_repeat_for.svg" />

ネストされたブロックを指定回数実行します。

### `〜まで繰り返し` (上級) {#block_control_repeat_until}

<img src={useBaseUrl('/img/blocks/block_control_repeat_until.svg')} alt="block_control_repeat_until.svg" />

条件が真になるまでブロックを繰り返し実行します。

### `ずっと` (上級) {#block_control_repeat_forever}

<img src={useBaseUrl('/img/blocks/block_control_repeat_forever.svg')} alt="block_control_repeat_forever.svg" />

プログラムまたはスクリプトが停止されるまで継続的に実行します。

## 分岐ブロック

### `もし` (初級) {#block_control_if}

<img src={useBaseUrl('/img/blocks/block_control_if.svg')} alt="block_control_if.svg" />

条件が真のときのみブロックを実行します。

### `もし / そうでなければ` (上級) {#block_control_if_else}

<img src={useBaseUrl('/img/blocks/block_control_if_else.svg')} alt="block_control_if_else.svg" />

条件が真の場合は一方を、そうでない場合は別のブランチを実行します。

### `これとこれを実行` (達人) {#block_control_do_this_and_this}

<img src={useBaseUrl('/img/blocks/block_control_do_this_and_this.svg')} alt="block_control_do_this_and_this.svg" />

2つのブロックスタックを順番に実行します。

## 停止ブロック

### `停止` (初級) {#block_control_stop}

<img src={useBaseUrl('/img/blocks/block_control_stop.svg')} alt="block_control_stop.svg" />

スクリプトの実行を停止します（範囲は選択されたオプションによる）。

- 停止オプション: `すべて`, `このスタック`, `プログラムを終了`

### `他のスタックを停止` (達人) {#block_control_stop_other_stacks}

<img src={useBaseUrl('/img/blocks/block_control_stop_other_stacks.svg')} alt="block_control_stop_other_stacks.svg" />

現在のスタックを継続したまま、他のすべてのスタックを停止します。

## ハブ／制御ユーティリティブロック

### `接続を設定` (初級) {#block_hubs_control_set_connect}

<img src={useBaseUrl('/img/blocks/block_hubs_control_set_connect.svg')} alt="block_hubs_control_set_connect.svg" />

制御フローからハブの接続状態を変更します。

- アクションオプション: `接続`, `切断`

### `ハブ設定をセット` (上級) {#block_hubs_set_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="block_hubs_set_hub_config.svg" />
選択したハブを、対応している設定プロファイルのいずれかに切り替えます。

- ハブ設定オプションを提供するハブでのみ使用できます。
- 主な用途: Technic Move Hub などの設定可能なハブを、次のブロックを実行する前に別の保存済み設定へ切り替えます。

### `ハブ設定` (上級) {#block_hubs_all_control_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="block_hubs_all_control_hub_config.svg" />
選択したハブの現在の設定を返します。

- タイプ: レポーターブロック
- 出力形式オプション: `text`, `index`
- ハブ設定オプションを提供するハブでのみ使用できます。
- 選択したハブが接続されていない場合、または設定が利用できない場合は `NaN` を返します。

### `接続されているか` (初級) {#block_hubs_all_sensors_is_connected}

<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_connected.svg')} alt="block_hubs_all_sensors_is_connected.svg" />

ハブが接続されているかどうかを返します。

- タイプ: ブール値レポーターブロック

### `BuWizz 2 電力モードを設定` (初級) {#block_hubs_buwizz_sensors_set_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_set_power_mode.svg')} alt="block_hubs_buwizz_sensors_set_power_mode.svg" />

BuWizz 2 ハブの電力モードを設定します。

- モードオプション: `Slow`, `Normal`, `Fast`, `Ludicrous`

### `BuWizz 2 電力モードを取得` (達人) {#block_hubs_buwizz_sensors_get_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_power_mode.svg')} alt="block_hubs_buwizz_sensors_get_power_mode.svg" />

現在の電力モードを返します。

- 出力形式: `テキスト`, `インデックス`

### `MouldKing 制御チャンネルを設定` (上級) {#block_hubs_mouldking_control_set_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_set_control_channel.svg')} alt="block_hubs_mouldking_control_set_control_channel.svg" />

MouldKing ハブの制御チャンネルを設定します。

- チャンネル: `A`, `B`, `C`

### `MouldKing 制御チャンネルを取得` (上級) {#block_hubs_mouldking_control_get_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_get_control_channel.svg')} alt="block_hubs_mouldking_control_get_control_channel.svg" />

現在の制御チャンネルを返します。

- 出力形式: `テキスト`, `インデックス`