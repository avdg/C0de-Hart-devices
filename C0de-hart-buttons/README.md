## Install commands through arduino-cli

```sh
arduino-cli core update-index

arduino-cli lib install OSC

arduino-cli core install esp32:esp32

# Find the board name (linux: /dev/ttyUSB0, windows: COM3)
arduino-cli board list

# -p -> port, -u -> upload after compile, -v -> verbose (optional)
arduino-cli compile -b esp32:esp32:esp32 .\C0de-hart-buttons\ -p <port from `arduino-cli board list`> -u

# Debug
arduino-cli debug .\C0de-hart-buttons\ -p <port from `arduino-cli board list`>
```