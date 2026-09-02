---
id: Light
title: ライト
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# ライト

このページでは、対応するハブのLEDやライト出力を制御するためのライトカテゴリブロックについて説明します。

## 共通ライトブロック

### `LEDの色を設定` (初級) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

事前定義された色を使用してハブのLEDカラーを設定します。

- タイプ: コマンドブロック
- 使用例: 状態表示（待機中、動作中、警告、エラー）

### `ライトを〜にする` (初級) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

選択したライト出力を指定した明るさ／値に設定します。

- タイプ: コマンドブロック
- 使用例: ヘッドライトの明るさ調整、状態の強度表示

### `ライトをオフ` (初級) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

選択したライト出力をオフにします。

- タイプ: コマンドブロック
- 使用例: シャットダウン処理、省電力動作

### `Technic Move ライトを〜にする` (初級) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

Technic Moveハブ用の `ライトを〜にする` のバリエーションです。

- タイプ: コマンドブロック
- 使用例: Moveハブのライト出力レベル設定

## 内蔵LEDマトリクスブロック

### `ライトマトリクスをオンにする` (上級) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

選択した画像をハブの内蔵LEDマトリクスに表示し、スタック内の次のブロックへすぐに進みます。画像は、別のブロックが内蔵LEDマトリクスを変更するか、プログラムが停止するまで表示されます。

- 種類: コマンドブロック
- 注意: 選択したハブには内蔵LEDマトリクスが必要です。

### `ライトマトリクスに書き込む` (初級) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

1文字ずつスクロールして、ハブの内蔵LEDマトリクスにテキスト文字列を表示します。

- 種類: コマンドブロック
- 注意: 選択したハブには内蔵LEDマトリクスが必要です。

### `マトリクスのピクセルをオフにする` (初級) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

ハブの内蔵LEDマトリクス上のすべてのライトを消します。

- 種類: コマンドブロック
- 注意: 選択したハブには内蔵LEDマトリクスが必要です。

### `マトリクスのピクセルを設定` (上級) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

ハブの内蔵LEDマトリクス上の1つのピクセルの明るさを設定します。選択したピクセルだけが更新され、残りの表示は変わりません。ピクセル位置のフィールドは列と行の値を使い、ピクセル `1, 1` は左上隅です。

- 種類: コマンドブロック
- 注意: 選択したハブには内蔵LEDマトリクスが必要です。

### `マトリクスの向きを回転` (上級) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

ハブの内蔵LEDマトリクスに表示されている内容の向きを時計回りまたは反時計回りに回転します。各回転で表示方向が90度変わり、その後に実行されるライトブロックに影響します。

- 種類: コマンドブロック
- 注意: 選択したハブには内蔵LEDマトリクスが必要です。

### `マトリクスの向きを設定` (上級) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

ハブの内蔵LEDマトリクスに表示される内容の向きを設定します。既定の向きは直立で、選択した向きはその後に実行されるライトブロックに影響します。

- 種類: コマンドブロック
- 向きオプション: `直立`, `左`, `右`, `上下反転`
- 注意: 選択したハブには内蔵LEDマトリクスが必要です。

## 距離センサーライトブロック

### `距離センサーを点灯` (初級) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

選択した距離センサーのライトを設定します。このブロックは個々のセンサーライトをオンまたはオフにでき、リストのレポーターブロックを使って各ライトの明るさを制御できます。

- 種類: コマンドブロック
- 注意: MINDSTORMS Robot Inventor ハブでのみ使用できます。

## BuWizz 3 ライトブロック

### `BuWizz 3 LEDの色を設定` (初級) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

選択したBuWizz 3ポートのLEDカラーを設定します（内蔵カラーパレット）。

- タイプ: コマンドブロック

### `BuWizz 3 LEDの色を設定（テキスト）` (達人) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

テキストによる色指定でBuWizz 3のLEDカラーを設定します。

- タイプ: コマンドブロック
- 使用例: 変数による動的な色指定

### `BuWizz 3 LEDの色を設定（RGB）` (上級) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

RGB値を使用してBuWizz 3のLEDカラーを設定します。

- タイプ: コマンドブロック
- 使用例: カスタムカラーやグラデーション制御
