# Zev-2 Seven Digit Nixie Clock
Arduino ATmega 1284P based Nixie clock with GPS, PIR, automatic daylight saving time setting, and many additional features.

Zev-2 is a seven digit Nixie tube clock that uses the large, IN-18 Nixie tube. Zev-2-8 is the eight digit version, with RF and a switching power supply

Features of the clock include:

•	RGB LED under lighting with a variety of effects

•	Three configurable heirarchical override periods with independent settings for start and end times, Nixie brightness, RGB LED brightness, RGB colors and patterns, and Neon colon patterns. Each period can be enabled for weekdays, weekends, or both. Override button restores standard settings for user selectable time period.

•	Real time clock with accuracy to approximately one second per week

•	Optional GPS receiver syncs real time clock when variance is one second or greater, Zev-2-8 optionally syncs with MOD-6 Repeater

•	Automatic timezone setting for daylight saving time and standard time

•	Scrolling date display with three selectable date formats and optional RGB LED scrolling with date

•	Scrolling temperature display and optional RGB LED scrolling with temperature

•	Ambient light sensor increases brightness at user configurable setting

•	PIR sensor optionally enables display only when motion is sensed, for selected time period

•	Configurable cathode anti-poisoning routine helps to keep tubes in good condition

• Four digit dim override option (new 12/1/15)

• Custom RGB color select menu, for each hour (new 2/22/16)

DipTrace schematic, board layouts, acrylic tube spacer .ai files, Arduino code, and operating instructions are here. Latest designs have been ordered from pcbway.com. The processor is an Atmel Atmega 1284P using the Bobuino/Skinny Bob bootloader found here on Github.

GPS - The Ublox Neo-6M and 7M commonly available on eBay for under $15 shipped, works perfectly with this clock. Adafruit Ultimate GPS also works perfectly. The cost is $39.95 plus shipping. Latest versions have a phone jack for the GPS cable, and a header compatible with Ublox and Adafruit boards so that the GPS can be mounted vertically on the clock board. These GPS boards are so sensitive that they work anywhere in the house here in South Florida, so remote placement is not necessary.

Additional Notes:

Zev-1 and Zev-2 use the same software. See Zev-1 to download Zev-1.ino. The schematic is also the same for both clocks, except substitute 10K resistors on the anodes of the tubes, for the 15k resistors used on the Zev-1. 

LEDFader library is included here because it is not easy to find. TimerThree is here too, modified to work with the 1284P and Bobuino/Skinny Bob. Other libraries are easily found. Use the original Bounce library included with Bounce2, not Bounce2. I changed the name of the MCP23017 library, to MCP23017 because it was too long for me. It's from Adafruit.

Files with the extension .ai are the designs for the acrylic tube reflectors. They can be ordered in the USA from Pololu, and at lower cost but obviously longer delivery times from Asian supplies such as Seeed Studio.

Use zev-1.ino on the Zev-1 page, for the seven digit, Zev-2 clock. The eight digit clock only, uses zev-2-8.ino, here.

Sabina-1, a fifteen digit replica of the Metronome clock at Union Square, is running. All designs are here on Github.

Mitch Feig 
2/28/16

2/22/16 - This update includes major rewrites and optimizations, throughout the program. Several new options are available including a menu to set RGB color combinations for each hour of the day. 

This is my first circuit and pc board design. Feel free to improve the hardware and software. 
