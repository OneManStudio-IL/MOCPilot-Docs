---
id: AboutApp
title: MOCPilot について
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - 作る。走らせる。すべてを操る。

**MOCPilot** は、LEGO® と互換 Bluetooth 駆動作品向けのカスタム制御プロファイルを作成するアプリです。

ハブの接続、モーター制御、センサー読み取り、ダッシュボード設計、モデル、機構、車、トラック、列車、ロボット、独自 MOC 用のビジュアルプログラム作成を、ひとつの場所で行えます。

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="スマートフォンで動作する MOCPilot アプリ" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>MOCPilot でできること</h2>
    <ul>
      <li>自分のモデル用のカスタムプロファイル。</li>
      <li>対応する公式セット用の既製プロファイル。</li>
      <li>Bluetooth ハブの接続と管理。</li>
      <li>自動化とロジックのためのビジュアルブロックプログラミング。</li>
      <li>モデルを走らせたり操作したりするためのダッシュボードコントロール。</li>
      <li>LEGO® Powered Up、Technic、BuWizz、SBrick、Mould King、モーター、センサー、互換 Bluetooth デバイスのサポート。</li>
    </ul>
  </div>
</div>

## 考え方

多くの電動モデルには、単純なリモコン以上のものが必要です。車にはステアリング、スロットル、ライト、バッテリー監視、ギアボックスの順序、特別な起動手順が必要になることがあります。ロボットにはセンサー、イベント、条件ロジック、複数ハブの連携が必要になることがあります。

MOCPilot は、基本的なリモコンと本格的なプログラミング環境の中間にある用途のために設計されています。画面上のダッシュボードでモデルを走らせるところから始め、モデルが高度になったらロジック、センサー、自動化を追加できます。

## プロファイル

**プロファイル** は、1 つのモデルの制御センターです。

プロファイル内では、モデルに属するハブを選び、モデルを動かすプログラムを作成し、制御に使うダッシュボードを設計できます。

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilot のプロファイルページ" width="420" />

<details>
<summary>組み込みプロファイル</summary>

組み込みプロファイルは、対応する公式セット向けの既製サンプルです。すばやく始めたいときや、動作するプロファイルの構成を学びたいときに便利です。

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="MOCPilot の組み込みプロファイル" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="MOCPilot の組み込みブロックプログラム" width="1100" />

</details>

<details>
<summary>カスタムプロファイル</summary>

カスタムプロファイルは、自分の MOC や実験向けです。プロファイルを作成し、ハブを追加し、モーターとセンサーを接続し、プログラムを作り、実際のモデルに合った制御ダッシュボードを設計できます。

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="MOCPilot のカスタムプロファイルを作成" width="420" />

</details>

## ハブとデバイスを接続する

MOCPilot は対応する Bluetooth ハブと互換デバイスに接続し、それらをプロファイル内で利用できるようにします。

シンプルなモデルでは 1 つのハブを使えます。より多くのポート、別電源、独立モジュールが必要な場合は複数のハブを接続できます。

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="MOCPilot の 自分の Bluetooth ハブ ページ" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="MOCPilot で接続済みの Bluetooth ハブ" width="1100" />

<details>
<summary>対応ハードウェアの例</summary>

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(140px, 1fr))', gap: '16px', alignItems: 'end', margin: '16px 0'}}>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_hub_p.webp')} alt="LEGO Technic Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/technic_move_hub_p.webp')} alt="LEGO Technic Move Hub" style={{maxWidth: '130px'}} />
    <div><strong>Technic Move Hub</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/buwizz3_hub_p.webp')} alt="BuWizz 3.0 Pro Hub" style={{maxWidth: '130px'}} />
    <div><strong>BuWizz 3.0</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/sbrick_hub_p.webp')} alt="SBrick Hub" style={{maxWidth: '130px'}} />
    <div><strong>SBrick</strong></div>
  </div>
  <div style={{textAlign: 'center'}}>
    <img src={useBaseUrl('/img/devices/mould_king_4_p.webp')} alt="Mould King Hub" style={{maxWidth: '130px'}} />
    <div><strong>Mould King</strong></div>
  </div>
</div>

完全な一覧は[対応ハブ、モーター、センサー](/docs/Introducing/SupportedDevices/)ページを参照してください。

</details>

## ブロックでロジックを作る

MOCPilot にはビジュアルブロックビルダーが含まれています。コードを書く代わりにブロックをつないでプログラムを作成できます。

ブロックはイベントへの反応、モーター制御、センサー読み取り、変数の利用、ゲームパッド入力、ダッシュボードコントローラー更新、複数アクションの連携に使えます。

MOCPilot は接続された物理ゲームパッドを完全にサポートします。ゲームパッドブロックはボタン、トリガー、D-pad 方向、スティックを読み取れるため、タッチスクリーンより物理操作が合う場合に実コントローラーをモデルへ割り当てられます。

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="ブロックで作成された MOCPilot ユーザープログラム" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="プログラム開始ブロック" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="速度指定でモーターを開始するブロック" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="ハブのバッテリーレベルブロック" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="ステアリングホイール値ブロック" />
</div>

<details>
<summary>ブロックプログラムでできること</summary>

- モーターを開始、停止、操舵する。
- バッテリーレベル、電圧、傾き、向き、温度、センサー値を読み取る。
- ステアリング、スロットル、トリガー、アクション、モード切り替え用に物理ゲームパッドを設定する。
- ボタン、センサー、タイマー、ダッシュボードコントローラーの変化に反応する。
- モデルが動き始める前の起動チェックを作成する。
- ライト、ステアリング調整、パワーモード、ハブ設定の独自ロジックを追加する。
- 変数、リスト、条件、ループ、ブロードキャスト、カスタムブロックで複雑な動作を整理する。

</details>

## 走行ダッシュボードを設計する

ダッシュボードは、モデルを制御するときに使う画面です。ステアリングホイール、ジョイスティック、スライダー、ボタン、スイッチ、ペダル、モニター、その他のコントローラーを配置できます。

ダッシュボードのコントロールや物理ゲームパッド入力をブロックやハブのアクションにつなげることで、インターフェースをモデルに合わせられます。

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot のダッシュボードコントローラー" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="ステアリングとペダルを備えた MOCPilot の制御画面" width="1100" />

<details>
<summary>ダッシュボード例</summary>

- 車にはステアリングホイールとペダルを使う。
- クレーン、リフト、リニアアクチュエーターにはスライダーを使う。
- ライト、ホーン、ギア変更、スクリプト動作にはボタンを使う。
- バッテリー、速度、センサー値、独自プログラム状態の表示にはモニターを使う。
- タッチ操作より物理ボタン、スティック、トリガーが好みなら接続ゲームパッドを使う。

</details>

## 高度な作品を扱いやすく保つ

モデルが大きくなるにつれて、プロファイルも一緒に拡張できます。MOCPilot は **My Blocks** による再利用可能なロジック、プロファイル固有のハブ設定、複数コントローラー、手動制御と自動化を組み合わせるプログラムフローをサポートします。

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="MOCPilot での My Blocks 使用例" width="1100" />

これにより大きなプログラムを読みやすく保てます。たとえば、バッテリー更新用、ステアリング調整用、特別な走行モード用にそれぞれカスタムブロックを持てます。

## 基本的な流れ

1. プロファイルを作成または開きます。
2. モデルで使う Bluetooth ハブとデバイスを追加します。
3. ブロックでプログラムを作成します。
4. 走行と操作用のダッシュボードを設計します。
5. **Play** を押します。
6. モデルが望む動きをするまで、テスト、調整、改善します。

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="MOCPilot のハブ接続フロー" width="1100" />

## MOCPilot が向いている人

MOCPilot は次のようなビルダーに役立ちます。

- 電動 LEGO® モデル用のより良いリモコンが欲しい。
- サードパーティ互換 Bluetooth ハブを制御したい。
- 機構やロボット向けのビジュアルプログラミング環境が欲しい。
- 対応する公式セット用の組み込みプロファイルを使いたい。
- 車、トラック、列車、クローラー、クレーン、その他 MOC 用のカスタムダッシュボードを作りたい。
- ハブ、モーター、センサー、ゲームパッド、画面コントロールを 1 つのアプリで組み合わせたい。

## 探索を始める

- [クイックスタートチュートリアル](/docs/Introducing/QuickStart/)に従って最初のプロファイルを作成します。
- ハードウェアを選ぶ前に[対応デバイス](/docs/Introducing/SupportedDevices/)を確認します。
- ロジックを追加する準備ができたら [BlockBuilder ドキュメント](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/)を確認します。
- ハブに対応ファームウェア版が必要な場合は、[ハブファームウェア更新](/docs/Application/Hubs/FirmwareUpdating/)を確認します。
