# Edzelf-Esp8266-WebRadio-Alternate-Module
D1R1+VS1053B

Advantage:
-	Less Wires ( Plug’n’Play )
-	Cheap and Simpler than Esp32
-	Hi Sound clarity vs1053b
-	Tested 24/7 run once on Unlimited Data Cable Broadband  
-	Simple & Forced Compatible
-	Windows Xp programmed.
-	Wifi with LED indicator 
- Buttonless Touch Preset +

Disadvantage
-	Not Effortless
-	Bare Minimum Setup
-	Not Localhost SD File read radio.ini yet ( TF card )
-	Needs 2wire vs1053b hard solder modification
( conflicting with redundant D1 SPI )
-	Only runs smoothly when (usetft) defined
-	radio.ini needs to be uploaded via wifi to spiff.
-	Exposed Wifi password on webinterface setup page .
- Security Advice: Enable Router aceess control (Whitelist).Only registered MAC gets access.

// Pins for VS1053 module
#define VS1053_DCS  3  
#define VS1053_CS   1  
#define VS1053_DREQ 16 
 
// Pins CS and DC for TFT module (if used, see definition of "USETFT")
#define TFT_CS 15
#define TFT_DC 2 //blinks inbuilt LED when wifi on

// Control button (GPIO) for controlling station
#define BUTTON1 4 // SDA
#define BUTTON2 17 //A0
#define BUTTON3 5 // SCL

Note x: 
-	A0 can be programmed with resistors to work more than one button.
-	SDA & SCL can be reserved for i2c OLED display
-	CS_SD of vs1053b can be used for LOCALHOST play
-	“USETFT” should be defined for smooth play on bare minimum else returns choppy streaming.
- Dont hesitate to re-devolope the sketch to your liking (OpenSourced D.I.Y Concept )

Re-Figured using Arduino ver 1.8.9 , esp8266 ver 2.5.0 on XP SP3 by Sroto & Gargees trials & errors.
Based on Original OpenSourced Author Edzelf.
