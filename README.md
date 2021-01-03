# goodie-box
An Arduino-based solution to preventing multiple pets from eating out of each other's food bowls

## Diagram
![Diagram shown here](https://github.com/Han-Lon/goodie-box/blob/main/img/ez-diagram.png?raw=true)

## Pin Layout (until I can find a higher rez Mifare component image)
### Mifare RFID reader connections
SDA <--> Digital 10 \n
SCK <--> Digital 13 \n
MOSI <--> Digital 11 \n
MISO <--> Digital 12 \n
IRQ -> unconnected \n
GND <--> GND (on Arduino) \n
RST <--> Digital 9 \n
3.3V <--> 3.3V (DON'T CONNECT TO 5V)
### Passive buzzer connections
Negative strip/column on breadboard <--> GND \n
Positive terminal on passive buzzer <--> Digital 8  

## Requirements
- Uses Miguel Balboa's RFID library located at https://github.com/miguelbalboa/rfid
  - You will need to download and import this library for this to function

## Roadmap
- Rewrite using ID12LA RFID reader instead of MFRC522
- Design 3D printable mounts for RFID reader and Arduino components
- Build the dang box
- Use cheaper Arduino Nano boards instead of an Uno R3
