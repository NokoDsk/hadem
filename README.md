![HADEM Logo](https://raw.githubusercontent.com/NokoDsk/hadem/refs/heads/main/1789223024879.png)

# Home Assistant Device & Entity Migration ("HADEM")

[![Version](https://img.shields.io/badge/version-0.0.1__dev-orange?style=for-the-badge)](https://github.com/NokoDsk/hadem)
[![GitHub Stars](https://img.shields.io/github/stars/NokoDsk/hadem?style=for-the-badge)](https://github.com/NokoDsk/hadem)
[![Contributors](https://img.shields.io/github/contributors/NokoDsk/hadem?style=for-the-badge)](https://github.com/NokoDsk/hadem/graphs/contributors)
[![License](https://img.shields.io/github/license/NokoDsk/hadem?style=for-the-badge)](https://github.com/NokoDsk/hadem/blob/main/LICENSE)

Do you remember the first time you replaced your phone, installed the Companion App and added it to Home Assistant. It wasn't until that moment when you realised what you had just done...

**New device. New entities. New sensors. Broken automations. And... spouse approval ratings somewhere below 1-star, and threats to rip the whole thing out.**

And it was somewhere around that point that you probably thought: **_"Well... there goes my weekend."_**

**Replacing a device shouldn't mean rebuilding Home Assistant. Now you can without rebuilding the configuration that depends on it.**

So I started developing **HADEM**. It's designed to make replacing devices in Home Assistant painless.

When a device is replaced, Home Assistant often creates a new device and a new set of entities. Your existing automations, scripts, dashboards, scenes, and other configuration may still depend on the entities from the old device.

HADEM analyses the old and replacement devices **(notice I didn't say "uses A.I." 🤣)**, matches their entities, and helps sync the replacement with your existing Home Assistant setup while preserving the Entity IDs your configuration already relies on.

It also identifies missing entities, checks which entities are actually being used, and can recommend sensors, capabilities, and permissions that may need to be enabled or configured on the replacement device.

## Our Primary Focus

While this concept is applicable to any device that may have reached end of life and needs to be replaced or is being upgraded, the **Home Assistant Companion App** is HADEM's primary use case.

Replacing a phone or tablet can create an entirely new device and, along with it, a large number of new sensors and entities. Differences in hardware, permissions, and available sensors can make it difficult to reproduce the functionality of the old device and restore the configuration that depends on it.

**New device. Same Home Assistant. No rebuilding from scratch. Enjoy your weekend.**

## Contributing

HADEM is an open-source project, and contributions are welcome.

If you've ever replaced a device and had to rebuild part of your Home Assistant configuration, you already understand the problem HADEM is trying to solve.

Whether you can help with development, testing, documentation, entity matching, device compatibility, or simply report an issue you've encountered, your contribution can help make device replacement easier for everyone.

[Open an Issue](https://github.com/NokoDsk/hadem/issues) · [View Contributors](https://github.com/NokoDsk/hadem/graphs/contributors)