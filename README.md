# IoT-DoS-defense
A demonstration of DoS defense methods for IoT

## Hardware
- Raspberry Pi Pico W
- MPL 3115A2 Altitude Sensor

## Base System
- Personal computer will act as a simple webserver
  - designed to receive data.
  - occasionally query Arduino for sensor data
  - measure response time
- Arduino will act as a web client (simulating an IoT device).
  - send barometric sensor data via WiFi to preconfigured target
  - data sent using both TCP and UDP
  - send data only when queried

  ## Attack
  - Third party attacker will use DoS attack on the Arduino