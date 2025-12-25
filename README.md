# Push-Pull-SSTC-mini
This SSTC circuit was originate from @skoriweb and was later revision by @tefatronix. But this circuit is improved with Protection circuit  which make them more versatile for DIY builds. In this design we will cover the detials for building this amazing and genius design for our modern Solid-State Tesla Coil. Still an on going project
# Materials
* N-Mosfet (Ex. IRF540n) x2
* Zener 12V 1W (IN4742A) x4
 * Zener V<Vds x2
 * 10K pull-down resistor x2
 * 100R 1W resistor
 * 400v 10nf MKP Cap x2
 * 7812 x1
 * 60V 2200uf x2 (optional)
 * 10uh common choke x2
 * 10k Potentiometer x1
 * 1uf MKP Cap x1
 * Ferrite Core 1x
 * 2 Servo wire 1.5m of lenght(m) x2
# N-Mosfet spec
Choose a common N-Channel Mosfet with low Rds(on state resistance) for better performance and low heat dissipation = low power loss.
# Capacitor BUS
Use capacitor with higher voltage rating than the supply circuit to the circuit.The more the capacitiance the more straight and longer the ARC gets(But no branch of ARC in the case of Continuous Wave operation).Unless it get interrupted by pulling down both gate with a N-channel mosfet to keep the gate of both N-Mosfet low, therefore the capacitors can charge up and deliver a huge current spike at once.
#Zener 12V Gate protection
The zener is tuned perfectly for protecting our N-channel Mosfet gate from high votlage spikes above the N-Mosfet gate rating which is Vgs = +20V/-20V Max. 12V is enough to drive the our N-Mosfet to the fullest for Lowest Rds as possible.The zener are facing eachother to protect overvoltage bias bidirectional meaning both directions. Since we are driving them isolated from a GDT(gate drive transformer) feedback with sine-wave signal which already know that sinusoidal wave can go up and down to +V and -V.