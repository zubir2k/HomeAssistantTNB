# HomeAssistantTNB  ![visitors](https://visitor-badge.glitch.me/badge?page_id=zubir2k.homeassistanttnb.visitor-badge)
Home Assistant template for Energy consumption based on TNB (Tenaga Nasional Berhad) Malaysia \
This template only supports for single phase user. Will add for 3 phase soon inshaAllah

## Requirements
1. Energy Sensor Integration (via CT Clamp, Smart RCCB and others) -> refer [here](https://www.home-assistant.io/docs/energy/electricity-grid/)

## Installation
1. Copy all files into your Home Assistant directory and paste all files into `\config`.
2. Enable package in [configuration.yaml](configuration.yaml) by adding the following line into the config file

```yaml
homeassistant:
  packages: !include_dir_named HAMY/
```

3. Restart Home Assistant to take effect.
4. Create new dashboard (lovelace) and copy the templates [lovelace-ui-1phase.yaml](lovelace-ui-1phase.yaml)
5. Define energy source

## Visual
![image](https://user-images.githubusercontent.com/1905339/217555443-7a651f27-6bb5-45e8-b282-c9b732661038.png)

## Special Thanks
- [Bro Ishak](https://github.com/ishakmuhamad) for initial template 
- [HomeAssistantMalaysia](https://www.facebook.com/groups/homeassistantmalaysia)
