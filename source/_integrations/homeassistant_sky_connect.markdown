---
title: Home Assistant Connect ZBT-1
description: Home Assistant Connect ZBT-1 provides hardware information for the hardware configuration page.
ha_release: 2022.9
ha_category:
  - Other
  - Update
ha_codeowners:
  - '@home-assistant/core'
ha_domain: homeassistant_sky_connect
ha_integration_type: hardware
ha_config_flow: true
ha_platforms:
  - update
related:
  - url: https://support.nabucasa.com/hc/en-us/categories/24734620813469-Home-Assistant-Connect-ZBT-1
    title: Home Assistant Connect ZBT-1 documentation
  - docs: /connectzbt1/
    title: Home Assistant Connect ZBT-1 product page

---

The Home Assistant Connect ZBT-1 integration provides hardware information for the hardware configuration page.

For documentation on the Home Assistant Connect ZBT-1, please visit the [documentation page](https://support.nabucasa.com/hc/en-us/categories/24734620813469-Home-Assistant-Connect-ZBT-1).
If you are looking to buy one, please visit the [product page](/connectzbt1)

## Configuration

This integration is not user configurable.

## Re-installing the firmware using the Silicon Labs Web Flasher

The Home Assistant Connect ZBT-1 ships with a full-fledged Zigbee firmware. At this point, there are no known issues with the factory-flashed firmware.

Normally, there is no need to re-install the firmware. Firmware updates for the Connect ZBT-1 are natively supported in Home Assistant 2025.4 and newer if you are running the ZHA integration or OTBR.

If you are not using ZHA or OTBR, you can use the web flasher below to install the latest firmware version for Home Assistant Connect&nbsp;ZBT-1 directly from your browser over USB.

### Prerequisites

- Firmware update through web flasher is only available for Home Assistant SkyConnect devices and for Home Assistant Connect&nbsp;ZBT-1 devices purchased after October 20, 2024.

### To re-install the firmware

1. Plug in your Connect&nbsp;ZBT-1 to your computer.
2. Select the **Connect** button below.

    <script type="module" src="https://unpkg.com/@nabucasa/sl-web-tools@0.10.1/dist/web/nabucasa-zigbee-flasher.js?module"></script>
    <nabucasa-zigbee-flasher manifest="/static/firmware/connect-zbt-1/manifest.json"></nabucasa-zigbee-flasher>

3. Select the firmware version you want to install.

To read more about the SL Web Tools, refer to this [blog post](https://www.home-assistant.io/blog/2023/02/08/state-of-matter-and-thread/#silabs-multi-flasher--sl-web-tools).
