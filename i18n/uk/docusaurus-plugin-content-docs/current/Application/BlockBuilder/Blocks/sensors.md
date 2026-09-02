---
id: Sensors
title: Датчики
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Датчики

Блоки датчиків читають стан хаба/пристрою та надають дані для умов, подій і керувальної логіки.

## Датчики пристрою та хаба

### `Рівень батареї хаба` (Початківець) {#block_hubs_all_sensors_battery_level}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="block_hubs_all_sensors_battery_level.svg" />
Повертає поточний рівень заряду батареї хаба.

### `Напруга батареї хаба` (Просунутий) {#block_hubs_all_sensors_battery_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_voltage.svg')} alt="block_hubs_all_sensors_battery_voltage.svg" />
Повертає напругу батареї вибраного хаба у вольтах.

- Тип: числовий блок-репортер
- Доступно лише для хабів, які повідомляють напругу батареї.
- Повертає `NaN`, коли вибраний хаб не підключено.

### `Батарея пристрою %` (Початківець) {#block_sensors_device_battery_level}
<img src={useBaseUrl('/img/blocks/block_sensors_device_battery_level.svg')} alt="block_sensors_device_battery_level.svg" />
Повертає поточний рівень заряду батареї телефону/планшета з MOCPilot (у відсотках).

### `Температура плати` (Просунутий) {#block_hubs_all_sensors_board_temp}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_board_temp.svg')} alt="block_hubs_all_sensors_board_temp.svg" />
Повертає температуру плати хаба.

- Доступно лише для `BuWizz 2` і `BuWizz 3`.

### `Акселерометр хаба` (Гуру) {#block_hubs_all_sensors_accelerometer}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_accelerometer.svg')} alt="block_hubs_all_sensors_accelerometer.svg" />
Повертає необроблені дані акселерометра, які повідомляє вибраний хаб.

- Осі: `x`, `y`, `z`

### `Прискорення хаба` (Гуру) {#block_hubs_all_sensors_acceleration}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_acceleration.svg')} alt="block_hubs_all_sensors_acceleration.svg" />
Повертає дані прискорення, які повідомляє вибраний хаб.

- Осі: `x`, `y`, `z`

### `Кнопка натиснута` (Початківець) {#block_hubs_all_sensors_button_pressed}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_button_pressed.svg?v=20260409-2258')} alt="block_hubs_all_sensors_button_pressed.svg" />
Перевіряє, чи вибрана кнопка хаба відповідає вибраному стану.

- Варіанти стану: `натиснуто`, `відпущено`
- Типовий варіант кнопки: `center` (залежить від хаба)
- Примітка: доступні варіанти кнопок можуть відрізнятися залежно від моделі хаба.

### `Тип пристрою` (Початківець) {#block_hubs_all_motors_port_device_type}
<img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_device_type.svg')} alt="block_hubs_all_motors_port_device_type.svg" />
Повертає тип підключеного пристрою для вибраного порту.

- Тип: репортер-блок
- Типове використання: визначити, що саме підключено, перед запуском логіки для конкретного пристрою

### `Акселерометр пристрою` (Гуру) {#block_sensors_device_accelerometer_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_accelerometer_sensor_data.svg')} alt="block_sensors_device_accelerometer_sensor_data.svg" />
Повертає сирі значення акселерометра з датчиків пристрою.

- Варіанти осей: `x`, `y`, `z`

### `Прискорення пристрою` (Гуру) {#block_sensors_device_acceleration_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_acceleration_sensor_data.svg')} alt="block_sensors_device_acceleration_sensor_data.svg" />
Повертає дані прискорення з датчиків пристрою.

- Варіанти осей: `x`, `y`, `z`

## Датчики орієнтації та нахилу

### `Нахил пристрою` (Просунутий) {#block_sensors_device_tilt_sensor_data}
<img src={useBaseUrl('/img/blocks/block_sensors_device_tilt_sensor_data.svg')} alt="block_sensors_device_tilt_sensor_data.svg" />
Повертає дані нахилу телефона/планшета, на якому працює MOCPilot.

- Осі: `pitch`, `roll`

### `Нахил` (Початківець) {#block_hubs_all_sensors_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_tilt.svg')} alt="block_hubs_all_sensors_tilt.svg" />
Повертає кут нахилу для вибраної осі.

- Варіанти осей: `тангаж`, `крен`, `рискання`
- Примітка: `рискання` доступне лише на хабах, які надають дані рискання.

### `Отримати орієнтацію` (Початківець) {#block_hubs_sensors_get_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_get_orientation.svg')} alt="block_hubs_sensors_get_orientation.svg" />
Повертає поточний стан орієнтації хаба.

- Варіанти формату виводу: `текст`, `індекс`
- Значення орієнтації: `Перед`, `Верх`, `Праворуч`, `Зад`, `Низ`, `Ліворуч`

### `Орієнтація вгору?` (Початківець) {#block_hubs_all_sensors_is_orientation_up}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_is_orientation_up.svg')} alt="block_hubs_all_sensors_is_orientation_up.svg" />
Перевіряє, чи орієнтація хаба відповідає вибраному напрямку «вгору».

- Варіанти орієнтації: `Перед`, `Верх`, `Праворуч`, `Зад`, `Низ`, `Ліворуч`

### `Встановити орієнтацію нахилу` (Просунутий) {#block_hubs_sensors_set_tilt_orientation}
<img src={useBaseUrl('/img/blocks/block_hubs_sensors_set_tilt_orientation.svg')} alt="block_hubs_sensors_set_tilt_orientation.svg" />
Налаштовує опорну орієнтацію для блоків, пов’язаних із нахилом/орієнтацією.

- Варіанти орієнтації: `Перед`, `Верх`, `Праворуч`, `Зад`, `Низ`, `Ліворуч`

## Таймер і датчики руху пристрою

### `Таймер` (Просунутий) {#block_sensors_timer_value_float}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_value_float.svg')} alt="block_sensors_timer_value_float.svg" />
Повертає значення таймера в секундах.

### `Скинути таймер` (Просунутий) {#block_sensors_timer_reset}
<img src={useBaseUrl('/img/blocks/block_sensors_timer_reset.svg')} alt="block_sensors_timer_reset.svg" />
Скидає таймер до нуля.

## Портові блоки датчиків

### `Датчик відстані Technic` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_distance.svg')} alt="block_hubs_all_sensors_port_technic_sensor_distance.svg" />
Повертає значення відстані з датчика відстані Technic.

- Варіанти одиниць: `мм`, `см`, `дюйм`, `відсоток`

### `Technic: коли відстань` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_when_distance_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_distance_is.svg" />
Спрацьовує/перевіряє умову відстані для датчика відстані Technic.

- Варіанти порівняння: `ближче ніж`, `далі ніж`, `точно на`
- Варіанти одиниць: `мм`, `см`, `дюйм`, `відсоток`

### `Technic встановити режим датчика кольору` (Просунутий) {#block_hubs_all_sensors_port_technic_sensor_set_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_set_mode.svg')} alt="block_hubs_all_sensors_port_technic_sensor_set_mode.svg" />
Цей блок встановлює датчик кольору Technic у вибраний режим.

- Примітка: Зміна режиму датчика кольору може неочікувано вплинути на вашу програму. Наприклад, датчик кольору Technic не може зчитувати кольори або відбите світло, коли він у режимі `"довкілля"`.

### `Значення кольору Technic` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_color.svg" />
Повертає визначене значення кольору з датчика відстані Technic.

- Варіанти виводу: `значення`, `рядок`

### `Technic: коли колір` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_when_color_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_color_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_color_is.svg" />
Спрацьовує/перевіряє, коли визначений колір збігається з вибраним.

### `Відбите світло Technic` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_reflected_light.svg" />
Повертає інтенсивність відбитого світла.

### `Technic: коли відбите світло` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_reflected_light_is.svg" />
Спрацьовує/перевіряє порогову умову відбитого світла.

- Варіанти порівняння: `<`, `=`, `>`

### `Навколишнє світло Technic` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_ambient_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_ambient_light.svg')} alt="block_hubs_all_sensors_port_technic_sensor_ambient_light.svg" />
Повертає інтенсивність навколишнього світла.

### `Technic: коли навколишнє світло` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg')} alt="block_hubs_all_sensors_port_technic_sensor_when_ambient_light_is.svg" />
Спрацьовує/перевіряє порогову умову навколишнього світла.

- Варіанти порівняння: `<`, `=`, `>`

### `Сирий колір Technic` (Початківець) {#block_hubs_all_sensors_port_technic_sensor_raw_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_technic_sensor_raw_color.svg')} alt="block_hubs_all_sensors_port_technic_sensor_raw_color.svg" />
Повертає сире значення каналу кольору з датчика Technic.

- Варіанти каналу: `червоний`, `зелений`, `синій`

### `Відстань датчика BOOST` (Початківець) {#block_hubs_all_sensors_port_boost_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_distance.svg" />
Повертає відстань з датчика відстані BOOST.

- Варіанти одиниць: `відсоток`, `см`, `дюйм`

### `BOOST: коли відстань` (Початківець) {#block_hubs_all_sensors_port_boost_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_distance.svg" />
Спрацьовує/перевіряє умову відстані для датчика відстані BOOST.

- Варіанти порівняння: `ближче ніж`, `далі ніж`, `точно на`
- Варіанти одиниць: `відсоток`, `см`, `дюйм`

### `Колір датчика BOOST` (Початківець) {#block_hubs_all_sensors_port_boost_sensor_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_color.svg" />
Повертає колір, визначений датчиком BOOST.

- Варіанти виводу: `значення`, `рядок`

### `BOOST: це колір` (Початківець) {#block_hubs_all_sensors_port_boost_sensor_is_color}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_is_color.svg')} alt="block_hubs_all_sensors_port_boost_sensor_is_color.svg" />
Перевіряє, чи датчик BOOST зараз визначає вибраний колір.

### `Відбите світло BOOST` (Початківець) {#block_hubs_all_sensors_port_boost_sensor_reflected_light}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_reflected_light.svg')} alt="block_hubs_all_sensors_port_boost_sensor_reflected_light.svg" />
Повертає значення відбитого світла з датчика BOOST.

### `BOOST: коли відбите світло` (Початківець) {#block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg')} alt="block_hubs_all_sensors_port_boost_sensor_when_reflected_light_is.svg" />
Спрацьовує/перевіряє порогову умову відбитого світла для датчика BOOST.

- Варіанти порівняння: `<`, `=`, `>`

### `Technic Move: встановити режим потужності` (Початківець) {#block_hubs_technicmove_sensors_set_power_mode}
<img src={useBaseUrl('/img/blocks/block_hubs_technicmove_sensors_set_power_mode.svg')} alt="block_hubs_technicmove_sensors_set_power_mode.svg" />
Встановлює режим потужності Technic Move.

- Варіанти режиму: `звичайний`, `буст`

### `Вихідна напруга BuWizz` (Гуру) {#block_hubs_buwizz_sensors_get_output_voltage}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_get_output_voltage.svg')} alt="block_hubs_buwizz_sensors_get_output_voltage.svg" />
Повертає поточну вихідну напругу, яку повідомляє хаб BuWizz.

- Доступно лише для підтримуваних хабів BuWizz.

### `Струм порту BuWizz` (Гуру) {#block_hubs_buwizz_sensors_port_get_current}
<img src={useBaseUrl('/img/blocks/block_hubs_buwizz_sensors_port_get_current.svg')} alt="block_hubs_buwizz_sensors_port_get_current.svg" />
Повертає споживаний струм, повідомлений для вибраного порту хаба BuWizz.

- Доступно лише для підтримуваних хабів і портів BuWizz.

### `Відстань WeDo 2` (Початківець) {#block_hubs_all_sensors_port_wedo2_sensor_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_distance.svg" />
Повертає відстань із датчика відстані WeDo 2.

- Варіанти одиниць: `відсоток`, `см`, `дюйм`

### `WeDo 2 коли відстань` (Початківець) {#block_hubs_all_sensors_port_wedo2_sensor_when_distance}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg')} alt="block_hubs_all_sensors_port_wedo2_sensor_when_distance.svg" />
Запускає/перевіряє умову відстані для датчика відстані WeDo 2.

- Варіанти порівняння: `closer than`, `farther than`, `exactly at`
- Одиниці: `%`, `cm`, `inch`

### `Нахил WeDo 2` (Початківець) {#block_hubs_all_sensors_port_wedo2_tilt}
<img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_port_wedo2_tilt.svg')} alt="block_hubs_all_sensors_port_wedo2_tilt.svg" />
Повертає значення нахилу з датчика нахилу WeDo 2.

- Варіанти осі: `тангаж`, `крен`