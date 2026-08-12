# English version below
# Progress PI1310 Geschirrspüler: Steuerplatine defekt, keine Anzeige, lässt sich nicht einschalten (Reparaturanleitung)

Reparaturanleitung für eine defekte Steuerplatine (Elektronikplatine) im **Progress PI1310 Geschirrspüler**. Blitron-Platine, Bestückungsdruck **15003261-01**.

## Symptome

- Geschirrspüler reagiert nicht mehr auf Tastendruck
- Keine LEDs / keine Anzeige am Bedienfeld
- Gerät lässt sich nicht einschalten
- Netzspannung (230V) liegt nachweislich an der Platine an, das Gerät bleibt trotzdem komplett "tot"
- Betroffene Platinen-Bezeichnung: **15003261-01** (Aufdruck "Blitron")

## Mögliche Ursache

In meinem Fall waren mehrere Bauteile im Netzteilbereich der Platine beschädigt. Die Netzspannung kommt zwar noch an, aber die interne Kleinspannungsversorgung für den Mikrocontroller und die Steuerlogik bricht zusammen. Dadurch fehlt jede Reaktion, jede Anzeige, jedes Licht.

## Benötigte Ersatzteile

Alle Bauteile sind Standard-Elektronikbauteile und günstig bei jedem gängigen Elektronikversand (z.B. Reichelt, Conrad, Mouser, Digikey) erhältlich. Gesamtkosten typischerweise unter 5€.

Nummern beziehen sich auf die Positionen im beigefügten Foto der Platine:

1. **Funkentstörkondensator, X2-Klasse, 22nF, 305V, RM 10mm, 105°C**
   Suchbegriff: `X2 Kondensator 22nF 305V`

2. **Elko, radial, 4,7µF, 450V, RM 5mm, 105°C**
   Suchbegriff: `Elko 4,7µF 450V`

3. **Elko, radial, 4,7µF, 450V, RM 5mm, 105°C** (baugleich zu Nr. 2, zweimal auf der Platine verbaut)

4. **Widerstand, Metalloxid, 1,0kΩ, Bauform 0207, 1W, 5%**
   Suchbegriff: `Widerstand 1k 1W Metalloxid`

5. **AC/DC-Offline-Schalter (Schaltnetzteil-Controller), 85-265VAC, 280mA, SMD-8B**
   Bauteilbezeichnung: **LNK305GN** (Hersteller: Power Integrations)

6. **Elko, radial, 47µF, 35V, RM 2mm, 105°C**
   Suchbegriff: `Elko 47µF 35V` (zweimal auf der Platine verbaut)

7. **Elko, radial, 220µF, 35V, RM 3,5mm, 105°C**
   Suchbegriff: `Elko 220µF 35V`

8. **Varistor, 275V, RM 7,5mm**
   Bauteilbezeichnung: **S10K275** oder gleichwertig

9. **Varistor, 275V, RM 5mm**
   Bauteilbezeichnung: **S07K275** (zweimal auf der Platine verbaut)

![15003261-01](loeten.png?raw=true "15003261-01")

## Vorgehen

1. Platine ausbauen und die genannten Bauteile mit einem Multimeter prüfen.
2. Wenn möglich, verdächtige Bauteile auslöten und frei (nicht in-circuit) messen. In-circuit-Messungen können durch parallel liegende Bauteile verfälscht werden und einen falschen Wert anzeigen.
3. Auffällige Bauteile identifizieren: falscher Widerstands-/Kapazitätswert, Kurzschluss, oder fehlender Durchgang, wo einer erwartet wird.
4. Defekte Bauteile austauschen. Bei Elkos unbedingt auf korrekte Polung achten (Minus-Kennzeichnung am Gehäuse beachten).
5. Nach dem Löten die Platine optisch auf kalte Lötstellen und Lötbrücken prüfen.
6. Erst danach die Platine wieder an die Netzspannung anschließen.

## Voraussetzungen

Diese Reparatur erfordert Löterfahrung und einen sicheren Umgang mit Netzspannung (230V). Bauteile in diesem Bereich der Platine stehen unter Netzspannung. Bei Unsicherheit sollte die Reparatur einer Fachkraft überlassen werden.

## Haftungsausschluss

Diese Anleitung dient ausschließlich der Information und basiert auf einem konkreten Einzelfall. Keine Garantie auf Vollständigkeit oder Übertragbarkeit auf andere Geräte oder Fehlerbilder. Arbeiten an Netzspannung führenden Bauteilen erfolgen auf eigene Gefahr.

## Stichworte / Keywords

Progress PI1310, Geschirrspüler defekt, Geschirrspüler keine Anzeige, Geschirrspüler lässt sich nicht einschalten, Steuerplatine defekt, Elektronikplatine Reparatur, Blitron Platine 15003261-01, LNK305GN defekt, Varistor S07K275, Varistor S10K275, Schaltnetzteil Geschirrspüler, Geschirrspüler Elektronik Reparatur, Progress Electrolux AEG Zanussi Platine


# Progress PI1310 Dishwasher: Faulty Control Board, No Display, Won't Power On (Repair Guide)

Repair guide for a defective control board (electronics PCB) in the **Progress PI1310 dishwasher**. Blitron board, assembly designation **15003261-01**.

## Symptoms

- Dishwasher no longer responds to button presses
- No LEDs / no display on the control panel
- Appliance cannot be switched on
- Mains voltage (230V) is confirmed present at the board, yet the appliance remains completely "dead"
- Affected board designation: **15003261-01** (labeled "Blitron")

## Possible Cause

In my case, several components in the power supply section of the board were damaged. Mains voltage still arrives, but the internal low-voltage supply for the microcontroller and control logic collapses. As a result, there is no reaction, no display, no lights at all.

## Required Spare Parts

All components are standard electronic parts and are inexpensive from any common electronics supplier (e.g., Reichelt, Conrad, Mouser, Digikey). Typical total cost under €5.

Numbers refer to the positions in the attached photo of the board:

1. **Interference suppression capacitor, X2 class, 22nF, 305V, RM 10mm, 105°C**
   Search term: `X2 capacitor 22nF 305V`

2. **Electrolytic capacitor, radial, 4.7µF, 450V, RM 5mm, 105°C**
   Search term: `Elko 4.7µF 450V`

3. **Electrolytic capacitor, radial, 4.7µF, 450V, RM 5mm, 105°C** (identical to No. 2, installed twice on the board)

4. **Resistor, metal oxide, 1.0kΩ, 0207 package, 1W, 5%**
   Search term: `resistor 1k 1W metal oxide`

5. **AC/DC off-line switcher (SMPS controller), 85-265VAC, 280mA, SMD-8B**
   Part designation: **LNK305GN** (manufacturer: Power Integrations)

6. **Electrolytic capacitor, radial, 47µF, 35V, RM 2mm, 105°C**
   Search term: `Elko 47µF 35V` (installed twice on the board)

7. **Electrolytic capacitor, radial, 220µF, 35V, RM 3.5mm, 105°C**
   Search term: `Elko 220µF 35V`

8. **Varistor, 275V, RM 7.5mm**
   Part designation: **S10K275** or equivalent

9. **Varistor, 275V, RM 5mm**
   Part designation: **S07K275** (installed twice on the board)

![15003261-01](loeten.png?raw=true "15003261-01")

## Procedure

1. Remove the board and check the listed components with a multimeter.
2. If possible, desolder suspicious components and measure them out of circuit (not in-circuit). In-circuit measurements can be skewed by parallel components and show incorrect values.
3. Identify faulty components: wrong resistance/capacitance value, short circuit, or missing continuity where continuity is expected.
4. Replace defective components. With electrolytic capacitors, be sure to observe correct polarity (note the minus marking on the housing).
5. After soldering, visually inspect the board for cold solder joints and solder bridges.
6. Only then reconnect the board to mains voltage.

## Prerequisites

This repair requires soldering experience and safe handling of mains voltage (230V). Components in this section of the board are at mains potential. If unsure, the repair should be left to a qualified professional.

## Disclaimer

This guide is for informational purposes only and is based on one specific case. No guarantee of completeness or transferability to other appliances or fault patterns. Work on components carrying mains voltage is performed at your own risk.

## Keywords

Progress PI1310, dishwasher defective, dishwasher no display, dishwasher won't power on, control board faulty, electronics board repair, Blitron board 15003261-01, LNK305GN defective, varistor S07K275, varistor S10K275, dishwasher switch-mode power supply, dishwasher electronics repair, Progress Electrolux AEG Zanussi board
