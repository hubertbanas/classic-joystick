
Arduino Micro PRO

				TX (1)	USB		RAW
				RX (0)			GND		-> GND
				GND				RST
				GND				VCC		-> Joy1/Joy2 VCC
				SDA (2)			(A3)	-> Joy2 poty
				SCL (3)			(A2)	-> Joy2 potx
J2up		<- (4)				(A1)	-> Joy1 poty
J2down		<- (5)				(A0)	-> Joy1 potx
J2left		<- (6)				(15)	-> J1up
J2right		<- (7)				(14)	-> J1down
J2fire		<- (8)				(16)	-> J1left
J1fire		<- (9)				(10)	-> J1right

Na USB serial otworzy� menu z informacj�:
1. joy1 usb config (kbd:WSAD/strza�ki i/lub joy1)
2. joy2 usb config (kbd:WSAD/strza�ki i/lub joy2)
3. joy1 hw config (multisystemowe? mapowanie 2 i 3 fire; co z potx/y?)
4. joy2 hw config (multisystemowe? mapowanie 2 i 3 fire; co z potx/y?)
5. zapis konf. do eeprom
stopka i info �eby otworzy� w 1200baud do resetu
datadump ruch�w na serial ca�y czas

joysticki sprawdzane co max 20ms, ze 2-4 razy cz�ciej lepiej 

potxy
https://hackaday.io/project/7941-avercade/log/26877-rewiring-for-dual-atari-controller
(nie takie �atwe - trzeba dobra� kondensator i mierzy� czas �adowania - potrzebny pin z zasilaniem,
 zostawi� - i tak nie mam nic do paddles)

DB9 pinout
1	up
2	down
3	left
4	right
5	poty
6	fire
7	vcc
8	gnd
9	potx

patrz�c na kabel od przodu, wida� otwory
54321
9876

patrz�c na port od przodu wida� szpilki
12345
6789
