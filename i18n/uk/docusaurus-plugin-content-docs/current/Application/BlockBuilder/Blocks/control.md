---
id: Control
title: Керування
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Керування

Блоки керування відповідають за потік виконання: очікування, цикли, розгалуження та зупинку скриптів.

## Блоки очікування

### `Чекати` (Початківець) {#block_control_wait_for}

<img src={useBaseUrl('/img/blocks/block_control_wait_for.svg')} alt="block_control_wait_for.svg" />

Призупиняє поточний скрипт на вказаний час.

### `Чекати до` (Просунутий) {#block_control_wait_until}

<img src={useBaseUrl('/img/blocks/block_control_wait_until.svg')} alt="block_control_wait_until.svg" />

Призупиняє поточний скрипт, доки умова не стане істинною.

## Блоки циклів

### `Повторити` (Просунутий) {#block_control_repeat_for}

<img src={useBaseUrl('/img/blocks/block_control_repeat_for.svg')} alt="block_control_repeat_for.svg" />

Виконує вкладені блоки фіксовану кількість разів.

### `Повторювати до` (Просунутий) {#block_control_repeat_until}

<img src={useBaseUrl('/img/blocks/block_control_repeat_until.svg')} alt="block_control_repeat_until.svg" />

Повторює вкладені блоки, доки умова не стане істинною.

### `Завжди` (Просунутий) {#block_control_repeat_forever}

<img src={useBaseUrl('/img/blocks/block_control_repeat_forever.svg')} alt="block_control_repeat_forever.svg" />

Виконує вкладені блоки безперервно, доки програма або скрипт не буде зупинений.

## Блоки розгалуження

### `Якщо` (Початківець) {#block_control_if}

<img src={useBaseUrl('/img/blocks/block_control_if.svg')} alt="block_control_if.svg" />

Виконує вкладені блоки лише тоді, коли умова істинна.

### `Якщо / Інакше` (Просунутий) {#block_control_if_else}

<img src={useBaseUrl('/img/blocks/block_control_if_else.svg')} alt="block_control_if_else.svg" />

Виконує одну гілку, коли умова істинна, інакше виконує альтернативну гілку.

### `Зробити це і це` (Гуру) {#block_control_do_this_and_this}

<img src={useBaseUrl('/img/blocks/block_control_do_this_and_this.svg')} alt="block_control_do_this_and_this.svg" />

Виконує два стеки блоків послідовно в межах однієї операції керування потоком.

## Блоки зупинки

### `Зупинити` (Початківець) {#block_control_stop}

<img src={useBaseUrl('/img/blocks/block_control_stop.svg')} alt="block_control_stop.svg" />

Зупиняє виконання скрипта (область зупинки залежить від вибраного режиму).

- Варіанти зупинки: `all`, `this stack`, `and exit program`

### `Зупинити інші стеки` (Гуру) {#block_control_stop_other_stacks}

<img src={useBaseUrl('/img/blocks/block_control_stop_other_stacks.svg')} alt="block_control_stop_other_stacks.svg" />

Зупиняє всі інші запущені стеки, залишаючи поточний стек активним.

## Допоміжні блоки хаба/керування

### `Встановити підключення` (Початківець) {#block_hubs_control_set_connect}

<img src={useBaseUrl('/img/blocks/block_hubs_control_set_connect.svg')} alt="block_hubs_control_set_connect.svg" />

Керує станом підключення хаба з логіки керування.

- Варіанти дії: `підключити`, `відключити`

### `Установити конфігурацію хаба` (Просунутий) {#block_hubs_set_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_set_hub_config.svg')} alt="block_hubs_set_hub_config.svg" />
Установлює вибраний хаб на один із підтримуваних профілів конфігурації.

- Доступно лише для хабів, які надають параметри конфігурації.
- Типове використання: перемкнути налаштовуваний хаб, наприклад Technic Move Hub, на іншу збережену конфігурацію перед запуском наступних блоків.

### `Конфігурація хаба` (Просунутий) {#block_hubs_all_control_hub_config}
<img src={useBaseUrl('/img/blocks/block_hubs_all_control_hub_config.svg')} alt="block_hubs_all_control_hub_config.svg" />
Повертає поточну конфігурацію вибраного хаба.

- Тип: блок-репортер
- Варіанти формату виводу: `text`, `index`
- Доступно лише для хабів, які надають параметри конфігурації.
- Повертає `NaN`, якщо вибраний хаб не підключено або конфігурація недоступна.

### `Підключено?` (Початківець) {#block_hubs_all_sensors_is_connected}

<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_connected.svg')} alt="block_hubs_all_sensors_is_connected.svg" />

Повертає, чи хаб зараз підключений.

- Тип: логічний репортер-блок

### `BuWizz 2: встановити режим потужності` (Початківець) {#block_hubs_buwizz_sensors_set_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_set_power_mode.svg')} alt="block_hubs_buwizz_sensors_set_power_mode.svg" />

Встановлює режим потужності хаба BuWizz 2.

- Варіанти режиму: `Slow`, `Normal`, `Fast`, `Ludicrous`

### `BuWizz 2: отримати режим потужності` (Гуру) {#block_hubs_buwizz_sensors_get_power_mode}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_power_mode.svg')} alt="block_hubs_buwizz_sensors_get_power_mode.svg" />

Повертає поточний активний режим потужності BuWizz 2.

- Варіанти формату виводу: `текст`, `індекс`

### `MouldKing: встановити канал керування` (Просунутий) {#block_hubs_mouldking_control_set_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_set_control_channel.svg')} alt="block_hubs_mouldking_control_set_control_channel.svg" />

Встановлює активний канал керування для підтримуваного хаба/контролера MouldKing.

- Варіанти каналу: `A`, `B`, `C`

### `MouldKing: отримати канал керування` (Просунутий) {#block_hubs_mouldking_control_get_control_channel}

<img src={useBaseUrl('/img/blocks/block_hubs_mouldking_control_get_control_channel.svg')} alt="block_hubs_mouldking_control_get_control_channel.svg" />

Повертає поточний активний канал керування для підтримуваного хаба/контролера MouldKing.

- Варіанти формату виводу: `текст`, `індекс`