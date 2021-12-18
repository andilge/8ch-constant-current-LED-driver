# 8ch-constant-current-LED-driver
Constant current driver with esp32 MCU made for esphome


## Preamble
We are planning our new house. A seemingly endless process full of technical plans and proposed solutions. Among the proposals there are good ones, bad ones but also too expensive or immature ones.

In the field of automated lighting, the negatives outweigh the good in professional installations. I don’t need sinfully expensive lighting on closed and proprietary systems. Besides, I’ve been using Home Assistant for years and have learned to use ESPHome and want to build up on this.

With this starting position, the desire arose to do all the lighting in the new house myself and to rely on open source. Of course, in 2021 I will be using LED lights and I know that LEDs are best operated with constant current. After discussions with interested experts around the world, I arrived at the module LD24AJTA, which allows DC voltage and dimming with pwm at the input and offers a suitable constant current at the output.

Sweet, I can do nice pwm easily with an ESP32, the first prototype board was soon built up with it. If only all this could be done even faster and easier, without breadboard and soldering connections individually… you know what came next: I built up my own board with the essentials of the module LD24AJTA and an ESP32 on it.

## Where to find things
The board revisions are accessible in the folder "revisions". Check CHANGELOG.md for detailed revision history.

An example esphome yaml file is located in the folder "esphome".

## Where to go
I know some additional information is needed to get going. I'm planning to build up a wiki here with a step by step procedure, but I got no time to roll this off swiftly :-(
