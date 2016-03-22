# Zev 7 and 8 Digit Nixie Clocks
Arduino ATmega 1284P based Nixie clock with GPS, PIR, automatic daylight saving time setting, and many additional features.

Zev-1-7 Seven digit clock uses a variety of small tubes. 
Zev-2-7 Seven digit clock using the IN-18 tube.
Zev 1-8 & Zev-2-8 are Eight digit versions that also include nRF24L01+.

Features of the clocks include:

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

Software:
Seven digit clocks use Z7 hex file
Eight digit clocks use Z8 hex file
Use AVRDude or similar to program the Atmel 1284P chip. Sorry, I cannot help with this.

Files with the extension .ai are the designs for the acrylic tube reflectors. They can be ordered in the USA from Pololu, and at lower cost but obviously longer delivery times from Asian supplies such as Seeed Studio.

Sabina, a fifteen digit replica of the Metronome clock at Union Square, is also here on Github.

Mitch Feig 
2/28/16
