---
id: AboutApp
title: About MOCPilot
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# MOCPilot - Build It. Drive It. Control Everything.

**MOCPilot** is an app for building custom control profiles for LEGO® and compatible Bluetooth-powered creations.

It gives builders one place to connect hubs, control motors, read sensors, design dashboards, and create visual programs for models, mechanisms, cars, trucks, trains, robots, and custom MOCs.

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(260px, 1fr))', gap: '20px', alignItems: 'center', margin: '24px 0'}}>
  <div>
    <img src={useBaseUrl('/img/app_phone.png')} alt="MOCPilot app running on a phone" style={{maxWidth: '320px', width: '100%'}} />
  </div>
  <div>
    <h2>What MOCPilot gives you</h2>
    <ul>
      <li>Custom profiles for your own models.</li>
      <li>Ready-made profiles for supported official sets.</li>
      <li>Bluetooth hub connection and management.</li>
      <li>Visual block programming for automation and logic.</li>
      <li>Dashboard controls for driving and operating models.</li>
      <li>Support for LEGO® Powered Up, Technic, BuWizz, SBrick, Mould King, motors, sensors, and compatible Bluetooth devices.</li>
    </ul>
  </div>
</div>

## The idea

Most motorized builds need more than a simple remote. A car may need steering, throttle, lights, battery monitoring, a gearbox sequence, or a special startup routine. A robot may need sensors, events, conditional logic, and several hubs working together.

MOCPilot is designed for that middle space between a basic remote control and a full programming environment. You can start by driving a model from an on-screen dashboard, then add logic, sensors, and automation when the build becomes more advanced.

## Profiles

A **profile** is the control center for one model.

Inside a profile, you can choose which hubs belong to the model, create the program that runs the model, and design the dashboard used to control it.

<img src={useBaseUrl('/img/quick-start/my-profiles.png')} alt="MOCPilot profiles page" width="420" />

<details>
<summary>Prebuilt profiles</summary>

Prebuilt profiles are ready-made examples for supported official sets. They are useful when you want to start quickly or study how a working profile is assembled.

<img src={useBaseUrl('/img/quick-start/prebuilt-profiles.png')} alt="MOCPilot prebuilt profiles" width="420" />

<img src={useBaseUrl('/img/quick-start/prebuilt-blocks.png')} alt="Prebuilt MOCPilot block program" width="1100" />

</details>

<details>
<summary>Custom profiles</summary>

Custom profiles are for your own MOCs and experiments. You can create a profile, add hubs, connect motors and sensors, build a program, and design a control dashboard that matches the exact model.

<img src={useBaseUrl('/img/quick-start/user-create-page.png')} alt="Create a custom MOCPilot profile" width="420" />

</details>

## Connect hubs and devices

MOCPilot can connect to supported Bluetooth hubs and compatible devices, then make them available inside your profile.

You can use a profile with one hub for a simple build, or connect multiple hubs when your model needs more ports, separate power systems, or independent modules.

<img src={useBaseUrl('/img/quick-start/user-hubs-page.png')} alt="My Bluetooth hubs page in MOCPilot" width="1100" />

<img src={useBaseUrl('/img/quick-start/hubs-connected.png')} alt="Connected Bluetooth hubs in MOCPilot" width="1100" />

<details>
<summary>Examples of supported hardware</summary>

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

See the [supported hubs, motors, and sensors](/docs/Introducing/SupportedDevices/) page for the full list.

</details>

## Build logic with blocks

MOCPilot includes a visual block builder. You can create programs by connecting blocks instead of writing code.

Blocks can react to events, control motors, read sensors, work with variables, use gamepad input, update dashboard controllers, and coordinate several actions together.

MOCPilot fully supports connected physical gamepads. Gamepad blocks let you read buttons, triggers, D-pad directions, and thumbsticks, so you can map a real controller to your model when physical controls feel better than using the touchscreen.

<img src={useBaseUrl('/img/quick-start/user-program-blocks.png')} alt="MOCPilot user program built with blocks" width="1100" />

<div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(240px, 1fr))', gap: '16px', alignItems: 'center', margin: '20px 0'}}>
  <img src={useBaseUrl('/img/blocks/block_event_when_program_started.svg')} alt="When program starts block" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_motors_port_start_motor_at_speed.svg')} alt="Start motor at speed block" />
  <img src={useBaseUrl('/img/blocks/block_hubs_all_sensors_battery_level.svg')} alt="Hub battery level block" />
  <img src={useBaseUrl('/img/blocks/block_dashboard_controller_steering_wheel_value_float.svg')} alt="Steering wheel value block" />
</div>

<details>
<summary>What you can do with block programs</summary>

- Start, stop, and steer motors.
- Read battery level, voltage, tilt, orientation, temperature, and sensor values.
- Configure physical gamepad controls for steering, throttle, triggers, actions, and mode switching.
- React when buttons, sensors, timers, or dashboard controls change.
- Create startup checks before the model begins moving.
- Add custom logic for lights, steering calibration, power modes, and hub configuration.
- Use variables, lists, conditions, loops, broadcasts, and custom blocks to organize complex behavior.

</details>

## Design a driving dashboard

The dashboard is the screen you use while controlling the model. It can include steering wheels, joysticks, sliders, buttons, switches, pedals, monitors, and other controllers.

You can connect dashboard controls and physical gamepad inputs to blocks and hub actions, so the interface matches the model instead of forcing every build into the same remote layout.

<img src={useBaseUrl('/img/quick-start/user-dashboard-controllers.png')} alt="MOCPilot dashboard controllers" width="1100" />

<img src={useBaseUrl('/img/quick-start/control-screen.png')} alt="MOCPilot control screen with steering and pedals" width="1100" />

<details>
<summary>Dashboard examples</summary>

- Use a steering wheel and pedals for cars.
- Use sliders for cranes, lifts, and linear actuators.
- Use buttons for lights, horns, gear changes, or scripted actions.
- Use monitors to show battery, speed, sensor values, or custom program state.
- Use a connected gamepad when you prefer physical buttons, sticks, and triggers instead of touchscreen controls.

</details>

## Keep advanced builds manageable

As a model grows, the profile can grow with it. MOCPilot supports reusable logic with **My Blocks**, profile-specific hub setup, multiple controllers, and program flows that combine manual control with automation.

<img src={useBaseUrl('/img/my-blocks/my-blocks-usage-example.png')} alt="MOCPilot My Blocks usage example" width="1100" />

This helps keep large programs readable. For example, a profile can have one custom block for battery updates, another for steering calibration, and another for a special driving mode.

## Typical workflow

1. Create or open a profile.
2. Add the Bluetooth hubs and devices used by the model.
3. Build the program with blocks.
4. Design a dashboard for driving and interaction.
5. Press **Play**.
6. Test, tune, and improve the profile until the model behaves the way you want.

<img src={useBaseUrl('/img/quick-start/connect-hub-flow.png')} alt="Connect hub flow in MOCPilot" width="1100" />

## Who MOCPilot is for

MOCPilot is useful for builders who want:

- A better remote control for motorized LEGO® models.
- A way to control third-party compatible Bluetooth hubs.
- A visual programming environment for mechanisms and robots.
- Prebuilt profiles for supported official sets.
- Custom dashboards for cars, trucks, trains, crawlers, cranes, and other MOCs.
- A single app that can combine hubs, motors, sensors, gamepads, and on-screen controls.

## Start exploring

- Follow the [quick start tutorial](/docs/Introducing/QuickStart/) to build your first profile.
- Check [supported devices](/docs/Introducing/SupportedDevices/) before choosing hardware.
- Explore the [BlockBuilder documentation](/docs/Application/BlockBuilder/Blocks/BlocksIntroducing/) when you are ready to add logic.
- Review [hub firmware updating](/docs/Application/Hubs/FirmwareUpdating/) if a hub requires a supported firmware version.
