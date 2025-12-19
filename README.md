# EKS Better Vehicles

A lightweight realism driving script for FiveM that adds **smooth launch control**, **realistic engine on/off**, **handbrake logic**, **indicator & hazards controls**, and **natural hill rolling** — all via **pause-menu changeable keybinds**.

## Features

- **Smooth Launch (Hold Key)**

  - Hold your configured key to pull away smoothly
  - Prevents burnouts / harsh wheelspin for realistic takeoffs

- **Smooth Braking**

  - Braking ramps in smoothly for a more realistic stop

- **Realistic Engine Control (Keybind)**

  - Engine does **not** auto-start when entering the vehicle
  - Engine can be toggled on/off via keybind
  - When turned off, the engine is forced **fully off** (no idle/ticking)

- **Handbrake System (Keybind)**

  - Handbrake can only be applied when the vehicle is **stationary**
  - While handbrake is on, the vehicle cannot move

- **Hill Rolling**

  - If the engine is on and the handbrake is off, the vehicle will roll only on **actual hills**
  - Rolling starts slowly and builds up naturally
  - Rolling is cancelled while holding the brake (S) or handbrake (SPACE)

- **Indicators & Hazards (Keybinds)**

  - Left indicator keybind
  - Right indicator keybind
  - Hazards require holding the key:
    - Hold **2 seconds** to enable hazards
    - Hold **3 seconds** to disable hazards
  - Auto-cancel indicators only when you turn in the same direction indicated

## Keybinds (Pause Menu)

All controls are registered with `RegisterKeyMapping`, meaning players can change them in:

**ESC > Settings > Key Bindings > FiveM**

Keybinds include:
- Smooth Launch (Hold)
- Engine On/Off
- Handbrake
- Left Indicator
- Right Indicator
- Hazards (Hold)

## Installation

1. Drag the resource into your server `resources` folder  
2. Add to your `server.cfg`:

   ensure EKS_SmoothDrive

3. Restart the server (or `restart EKS_BetterVehicle`)

## Configuration

Edit `config.lua` to adjust:

- Speed units (MPH/KMH)
- Smooth launch torque ramp and no-smoke tuning
- Braking ramp settings
- Hill-roll realism (slope sensitivity / max roll speed / ramp-in feel)
- Hold durations for hazards
- Allowed vehicle classes

## Notes

- If you run other handling/driving scripts, disable overlapping features to prevent conflicts.
- For best results, keep this as the only script modifying traction/torque behaviour.

## Support

For help or bug reports, join our Discord and open a support ticket:  
https://discord.gg/busQ9w6dqa
