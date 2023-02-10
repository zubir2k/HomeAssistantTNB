# HomeAssistantTNB  ![visitors](https://visitor-badge.glitch.me/badge?page_id=zubir2k.homeassistanttnb.visitor-badge)
Home Assistant template for Energy consumption based on TNB (Tenaga Nasional Berhad) Malaysia \
This template only supports for single phase user. Will add for 3 phase soon inshaAllah

## Requirements
1. Energy Sensor Integration (via CT Clamp, Smart RCCB and others) -> refer [here](https://www.home-assistant.io/docs/energy/electricity-grid/) \
(Highly recommended - Shelly EM or 3EM with CT Clamp)

- Shelly EM - [link](https://s.lazada.com.my/s.U1C72)
- Shelly 3EM - [link](https://s.lazada.com.my/s.U1wAX)

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

![image](https://user-images.githubusercontent.com/1905339/217669869-c0092f49-cdd1-46ff-8834-6a3bd126c1fb.png)


## Visual
### Main Dashboard
![image](https://user-images.githubusercontent.com/1905339/217555443-7a651f27-6bb5-45e8-b282-c9b732661038.png)

### Daily Notification
![image](https://user-images.githubusercontent.com/1905339/217663962-4c3985ca-d57c-4438-8bd9-be8216d49fcc.png)

### Home Assistant Energy Dashboard
![image](https://user-images.githubusercontent.com/1905339/217665698-619f90dd-3055-4b35-8b9c-ca99a180b1a1.png)

## Special Thanks
- [Bro Ishak](https://github.com/ishakmuhamad) for initial template 
- [Bro Hannan](https://www.lazada.com.my/shop/nh-smart-home)
- [HomeAssistantMalaysia](https://www.facebook.com/groups/homeassistantmalaysia)

## Disclaimer
This template uses TNB bill calculation method to calculate energy consumption only, and does not include other charges such as 1% late payment, 1.6% Kumpulan Wang Tenaga Boleh Baharu (RE Fund), Power Factor surcharge, Connected Load Charge (CLC) penalty etc.

More info from TNB [here](https://www.mytnb.com.my/residential/understand-your-bill/bill-calculator)
