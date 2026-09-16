# ESP32-C6 Capacitive Button

blah blah

### Features:
- button
- LEDs
-

### Quick Start Guide:

#### Pinout:

| ESP32-C6 Pin | Function              | Xiao Pin |
|--------------|-----------------------|----------|
| GPIO22       | I2C SDA (MPR121)      | D4       |
| GPIO23       | I2C SCL (MPR121)      | D5       |
| GPIO16       | LED Strip (WS2812)    | D6       |
| GPIO17       | Fan Relay - Sleep     | D7       |
| GPIO19       | Fan Relay - Low       | D8       |
| GPIO20       | Fan Relay - Medium    | D9       |
| GPIO18       | Fan Relay - High      | D10      |

Capacitive buttons

| MPR121 Channel | Function             |
|----------------|----------------------|
| 3              | Sleep                |
| 4              | Filter Reset         |
| 5              | Lights Toggle        |
| 6              | Fan Speed            |
| 7              | Timer                |
| 8              | Power                |
| 9              | Lock                 |

LED addresses. LEDs are chained together, controlled by a single ESP32 pin (14 LEDs).

| Segment ID          | LED Index | Purpose            |
|---------------------|----------:|--------------------|
| power_led           | 0         | Power indicator    |
| lock_led            | 1         | Lock indicator     |
| filter_reset_led    | 2         | Filter reset       |
| lights_led          | 3         | Lights / brightness|
| led_8h              | 4         | Timer 8h           |
| led_6h              | 5         | Timer 6h           |
| led_4h              | 6         | Timer 4h           |
| led_2h              | 7         | Timer 2h           |
| timer_led           | 8         | Timer active       |
| sleep_led           | 9         | Sleep mode         |
| fan_on_led          | 10        | Fan on             |
| fan_low_led         | 11        | Fan speed low      |
| fan_medium_led      | 12        | Fan speed medium   |
| fan_high_led        | 13        | Fan speed high     |

 - [ESPHome Configuration File](esphome.yaml)

### Configuration:
...

### Purchase:
For purchasing information, please visit our [Product Page](https://shop.silocitylabs.com/products/esp32-button).
