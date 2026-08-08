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
| GPIO16       | PWM LED Output        | D6       |
| GPIO17       | Fan Relay - Sleep     | D7       |
| GPIO19       | Fan Relay - Speed 1   | D8       |
| GPIO20       | Fan Relay - Speed 2   | D9       |
| GPIO18       | Fan Relay - Speed 3   | D10      |

Capacitive buttons

| MPR121 Channel | Function             |
|----------------|----------------------|
| 3              | Lock                 |
| 4              | Sleep                |
| 5              | Timer                |
| 6              | Filter Reset         |
| 7              | Lights Toggle        |
| 8              | Power                |
| 9              | Fan Speed            |

LED addresses. LEDs are chained together, controlled by a single ESP32 pin.

| Segment ID          | LED Index | Purpose            |
|---------------------|----------:|--------------------|
| power_led           | 0         | Power button       |
| lock_led            | 1         | Lock indicator     |
| sleep_led           | 2         | Sleep mode         |
| timer_led           | 3         | Timer indicator    |
| filter_reset_led    | 4         | Filter reset       |
| lights_led          | 5         | Lights button      |
| fan_low_led         | 6         | Fan speed low      |
| fan_medium_led      | 7         | Fan speed medium   |
| fan_high_led        | 8         | Fan speed high     |

 - [ESPHome Configuration File](esphome.yaml)

### Configuration:
...

### Purchase:
For purchasing information, please visit our [Product Page](https://shop.silocitylabs.com/products/esp32-button).
