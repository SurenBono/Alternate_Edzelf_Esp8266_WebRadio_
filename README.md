# Edzelf-Esp8266-WebRadio-Alternate-Module
D1R1+VS1053B

Advantage:
-	Wire Free ( Plug’n’Play )
-	Cheap and Smoother than Esp32
-	Stronger Signal on vs1053b
-	Unlimited Data Copper Broadband 24/7 run Tested 
-	Simple & Compatible
-	Windows Xp capable with some effort
-	Wifi with LED indicator (if usetft defined)

Disadvantage
-	Not Effortless
-	Bare Minimum Setup
-	Not Localhost SD File player yet ( TF card )
-	Needs 2wire vs1053b hard solder modification
( conflicting with redundant D1 SPI )
-	Only runs smoothly when (usetft) defined
-	radio.ini needs re-upload in some case
-	Exposed Wifi password

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
