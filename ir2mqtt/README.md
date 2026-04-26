# IR2MQTT

Web UI for IR Bridges with Learning and MQTT Auto-Discovery for Home Assistant.

![IR2MQTT Demo](https://raw.githubusercontent.com/steelcuts/ir2mqtt/main/.github/assets/showcase.gif)

## What it does

IR2MQTT bridges physical infrared devices with your smart home. Instead of writing YAML, you use a modern Web UI to:

- **Manage IR bridges** that connect via MQTT (e.g. ESPHome-based devices)
- **Learn IR codes** directly from your remotes
- **Browse IR databases** (Flipper-IRDB, Probono IRDB) to find codes without a remote
- **Create automations** that trigger IR commands based on MQTT messages
- **Auto-discover devices** in Home Assistant via MQTT Discovery

## Configuration

| Option | Description | Default |
|--------|-------------|---------|
| `mqtt_broker` | Hostname or IP of your MQTT broker | `core-mosquitto` |
| `mqtt_port` | MQTT broker port | `1883` |
| `mqtt_user` | MQTT username | *(empty)* |
| `mqtt_pass` | MQTT password | *(empty)* |

## Hardware

Requires one or more IR bridges running the IR2MQTT ESPHome firmware. The bridges connect to your MQTT broker and are **auto-discovered** by IR2MQTT — no serial/USB connection to the host is needed.

See the [ir2mqtt_bridge](https://github.com/steelcuts/ir2mqtt_bridge) repository for firmware and wiring instructions (IR receiver + IR LED on an ESP32).

## Documentation

Full documentation is available at [steelcuts.github.io/ir2mqtt](https://steelcuts.github.io/ir2mqtt/).

## Support

- [Report an issue](https://github.com/steelcuts/ir2mqtt/issues)
