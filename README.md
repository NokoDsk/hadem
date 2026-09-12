# Home Assistant Device & Entity Migration ("HADEM")

[![Version](https://img.shields.io/badge/version-0.0.1__dev-orange?style=for-the-badge)](https://github.com/NokoDsk/hadem) [![GitHub Stars](https://img.shields.io/github/stars/NokoDsk/hadem?style=for-the-badge)](https://github.com/NokoDsk/hadem) [![Contributors](https://img.shields.io/github/contributors/NokoDsk/hadem?style=for-the-badge)](https://github.com/NokoDsk/hadem/graphs/contributors) [![License](https://img.shields.io/github/license/NokoDsk/hadem?style=for-the-badge)](https://github.com/NokoDsk/hadem/blob/main/LICENSE)

**Replacing a device shouldn't mean rebuilding Home Assistant.** 

> **Now you can replacing your device without rebuilding the Home Assistant configuration that depends on it.**

HADEM is designed to make replacing devices in Home Assistant painless.

When a device is replaced, Home Assistant often creates a new device and a new set of entities. Your existing automations, scripts, dashboards, scenes, and other configuration may still depend on the entities from the old device.

HADEM analyses the old and replacement devices, matches their entities, and helps sync the replacement with your existing Home Assistant setup while preserving the Entity IDs your configuration already relies on.

It also identifies missing entities, checks which entities are actually being used, and can recommend sensors, capabilities, and permissions that may need to be enabled or configured on the replacement device.

### Our Primary Focus

The **Home Assistant Companion App** is HADEM's primary use case.

Replacing a phone or tablet can create an entirely new device and, along with it, a large number of new sensors and entities. Differences in hardware, permissions, and available sensors can make it difficult to reproduce the functionality of the old device and restore the configuration that depends on it.

HADEM is designed to make that process easier by identifying what changed, matching what can be migrated, highlighting what is missing, and helping you restore the configuration your Home Assistant setup already depends on.

**New Device. Same Home Assistant. No Rebuilding from Scratch.**

## Contributing

HADEM is an open-source project, and contributions are welcome.

If you've ever replaced a device and had to rebuild part of your Home Assistant configuration, you already understand the problem HADEM is trying to solve.

Whether you can help with development, testing, documentation, entity matching, device compatibility, or simply report an issue you've encountered, your contribution can help make device replacement easier for everyone.

[Open an issue](https://github.com/NokoDsk/hadem/issues) · [View contributors](https://github.com/NokoDsk/hadem/graphs/contributors)