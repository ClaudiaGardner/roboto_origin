# atom01_firmware - ROBOTO_ORIGIN Firmware Module

Firmware and build systems for the ROBOTO_ORIGIN humanoid robot.

## Overview

This module contains firmware components and board image build systems required for the robot's embedded systems.

## Submodules

| Module | Description |
|--------|-------------|
| [roboto_usb2can](./roboto_usb2can) | USB to CAN adapter firmware - provides communication interface between host computer and robot's CAN bus |
| [orangepi-build](./orangepi-build) | OrangePi board image build system - compiles custom Linux images for RK series boards |
| [x5-rdk-gen](./x5-rdk-gen) | RP0 X5 image build system - generates firmware images for X5 platforms |

## Quick Start

```bash
# Clone repository with submodules
git clone --recursive https://github.com/Roboparty/atom01_firmware.git

# Or initialize submodules after cloning
git submodule update --init --recursive
```

## Directory Structure

```
atom01_firmware/
├── roboto_usb2can/      # USB2CAN firmware source
├── orangepi-build/      # OrangePi build system
│   └── external/cache/sources/bms_daemon/  # BMS daemon (nested)
├── x5-rdk-gen/          # X5 RDK generator
├── readme.md            # This file
└── readme_cn.md         # Chinese documentation
```

## Related Repositories

- **[Atom01_hardware](https://github.com/Roboparty/Atom01_hardware)** - Hardware design files
- **[atom01_deploy](https://github.com/Roboparty/atom01_deploy)** - ROS2 deployment framework
- **[atom01_train](https://github.com/Roboparty/atom01_train)** - RL training environment
- **[atom01_description](https://github.com/Roboparty/atom01_description)** - URDF model files

## License

This project is licensed under the GNU General Public License Version 3 (GPLv3).

## Contributing

See the main [roboto_origin](https://github.com/Roboparty/roboto_origin) repository for contribution guidelines.
