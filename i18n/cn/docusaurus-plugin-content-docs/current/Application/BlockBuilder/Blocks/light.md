---
id: Light
title: 灯光
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# 灯光

本页介绍“灯光”分类中的积木，用于控制受支持主控上的 LED 与灯光输出。

## 常用灯光积木

### `设置 LED 颜色` (初级) {#block_hubs_all_light_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_led_color.svg')} alt="block_hubs_all_light_set_led_color.svg" />

使用预设颜色选项设置主控 LED 颜色。

- 类型：命令积木
- 常见用途：显示状态（就绪、运行中、警告、错误）

### `灯光调到` (初级) {#block_hubs_all_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_to.svg')} alt="block_hubs_all_light_light_turn_to.svg" />

将所选灯光输出设置为目标亮度/数值。

- 类型：命令积木
- 常见用途：前灯亮度、状态灯强度

### `关闭灯光` (初级) {#block_hubs_all_light_light_turn_off}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_light_turn_off.svg')} alt="block_hubs_all_light_light_turn_off.svg" />

关闭所选灯光输出。

- 类型：命令积木
- 常见用途：关机流程、省电行为

### `Technic Move 灯光调到` (初级) {#block_hubs_technicmove_light_light_turn_to}

<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_light_light_turn_to.svg')} alt="block_hubs_technicmove_light_light_turn_to.svg" />

`Light turn to` 的 Technic Move 主控/灯光目标版本。

- 类型：命令积木
- 常见用途：设置 Move 主控的灯光输出级别

## 内置 LED 矩阵积木

### `打开灯光矩阵` (高级) {#block_hubs_all_light_set_internal_led_matrix_image}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_image.svg')} alt="block_hubs_all_light_set_internal_led_matrix_image.svg" />

在 Hub 的内置 LED 矩阵上显示所选图像，并立即继续执行堆栈中的下一个积木。该图像会一直保留在显示屏上，直到另一个积木更改内置 LED 矩阵，或程序停止。

- 类型：命令积木
- 注意：所选 Hub 必须有内置 LED 矩阵。

### `在灯光矩阵上写入` (初级) {#block_hubs_all_light_set_internal_led_matrix_text}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_text.svg')} alt="block_hubs_all_light_set_internal_led_matrix_text.svg" />

通过逐个滚动字母，在 Hub 的内置 LED 矩阵上显示文本字符串。

- 类型：命令积木
- 注意：所选 Hub 必须有内置 LED 矩阵。

### `关闭矩阵像素` (初级) {#block_hubs_all_light_turn_off_internal_led_matrix_pixels}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg')} alt="block_hubs_all_light_turn_off_internal_led_matrix_pixels.svg" />

关闭 Hub 内置 LED 矩阵上的所有灯光。

- 类型：命令积木
- 注意：所选 Hub 必须有内置 LED 矩阵。

### `设置矩阵像素` (高级) {#block_hubs_all_light_set_internal_led_matrix_pixel}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_pixel.svg')} alt="block_hubs_all_light_set_internal_led_matrix_pixel.svg" />

设置 Hub 内置 LED 矩阵上单个像素的亮度。只会更新所选像素，显示屏的其余部分保持不变。像素位置字段使用列和行，像素 `1, 1` 位于左上角。

- 类型：命令积木
- 注意：所选 Hub 必须有内置 LED 矩阵。

### `旋转矩阵方向` (高级) {#block_hubs_all_light_rotate_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_rotate_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_rotate_internal_led_matrix_orientation.svg" />

顺时针或逆时针旋转 Hub 内置 LED 矩阵上显示内容的方向。每次旋转都会将显示方向改变 90 度，并影响之后运行的灯光积木。

- 类型：命令积木
- 注意：所选 Hub 必须有内置 LED 矩阵。

### `设置矩阵方向` (高级) {#block_hubs_all_light_set_internal_led_matrix_orientation}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_set_internal_led_matrix_orientation.svg')} alt="block_hubs_all_light_set_internal_led_matrix_orientation.svg" />

设置 Hub 内置 LED 矩阵上显示内容的方向。默认方向为正向，所选方向会影响之后运行的灯光积木。

- 类型：命令积木
- 朝向选项：`正向`、`左`、`右`、`倒置`
- 注意：所选 Hub 必须有内置 LED 矩阵。

## 距离传感器灯光积木

### `距离传感器点亮` (初级) {#block_hubs_all_light_port_distance_sensor_light_up}

<img src={useBaseUrl('/img/blocks/block_hubs_all_light_port_distance_sensor_light_up.svg')} alt="block_hubs_all_light_port_distance_sensor_light_up.svg" />

设置所选距离传感器上的灯光。该积木可以打开或关闭单个传感器灯，也可以使用列表报告积木控制每个灯的亮度。

- 类型：命令积木
- 注意：仅适用于 MINDSTORMS Robot Inventor Hub。

## BuWizz 3 灯光积木

### `BuWizz 3 设置 LED 颜色` (初级) {#block_hubs_buwizz3_light_port_set_led_color}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color.svg')} alt="block_hubs_buwizz3_light_port_set_led_color.svg" />

使用内置颜色选项设置所选 BuWizz 3 端口上的 LED 颜色。

- 类型：命令积木

### `BuWizz 3 设置 LED 颜色（字符串）` (专家) {#block_hubs_buwizz3_light_port_set_led_color_string}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_string.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_string.svg" />

使用文本颜色值设置 BuWizz 3 的 LED 颜色。

- 类型：命令积木
- 常见用途：从变量动态读取颜色名称

### `BuWizz 3 设置 LED 颜色（RGB）` (高级) {#block_hubs_buwizz3_light_port_set_led_color_rgb}

<img src={useBaseUrl('/img/blocks/block_hubs_buwizz3_light_port_set_led_color_rgb.svg')} alt="block_hubs_buwizz3_light_port_set_led_color_rgb.svg" />

使用明确的 RGB 通道值设置 BuWizz 3 的 LED 颜色。

- 类型：命令积木
- 常见用途：完全自定义颜色控制与渐变效果
