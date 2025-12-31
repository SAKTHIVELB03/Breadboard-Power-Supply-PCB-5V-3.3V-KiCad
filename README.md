# Breadboard-Power-Supply-PCB-5V-3.3V-KiCad
This breadboard power supply circuit is designed to generate stable and regulated 5V and 3.3V DC outputs from an external DC power source, making it suitable for embedded systems development and electronics prototyping.

The input power is supplied through a DC barrel jack, typically from a 7V–12V adapter. A power switch is placed in series with the input to allow controlled power ON/OFF operation, ensuring safe isolation of the circuit when not in use. A power flag is included in the schematic to properly indicate the presence of a power source during electrical rule checks.

The 5V regulation stage is implemented using a LM7805 linear voltage regulator. This regulator converts the unregulated input voltage into a fixed 5V output by internally dissipating excess voltage as heat. Input and output decoupling capacitors are placed close to the regulator pins to suppress noise, prevent oscillations, and improve transient response. The regulated 5V rail can be used directly to power external circuits and also serves as the input supply for the 3.3V regulation stage.

The 3.3V output is generated using an LM317 adjustable linear regulator, configured with a resistor divider network to set the output voltage to 3.3V according to the standard LM317 voltage equation. Additional output capacitance is used to enhance stability and reduce ripple. Deriving the 3.3V rail from the regulated 5V supply improves overall noise performance and ensures consistent voltage regulation.

An LED indicator with a current-limiting resistor is included to provide a visual indication of power availability. This allows quick verification that the board is powered correctly during use.

The regulated 5V, 3.3V, and GND outputs are routed to breadboard-compatible pin headers, enabling easy insertion into standard breadboards and flexible power distribution to multiple prototyping circuits. A hatched ground copper pour is implemented on the PCB to provide a low-impedance return path, improve noise performance, and maintain good grounding practices while ensuring manufacturability and solderability.

Overall, the circuit provides a simple, reliable, and compact power solution for breadboard-based prototyping, demonstrating practical application of linear voltage regulation, filtering, grounding, and PCB layout best practices.

#BOM 
<img width="962" height="309" alt="image" src="https://github.com/user-attachments/assets/e67e5ff4-5e4d-4f4b-bbdc-4a1801c81fde" />

#Schematic
<img width="1919" height="1079" alt="schematic" src="https://github.com/user-attachments/assets/ce674dbe-4f99-47b5-8a61-d2a3c6ac647b" />

#pcb layout
<img width="1919" height="1079" alt="pcb layout" src="https://github.com/user-attachments/assets/342f9a38-1248-45ff-8bf1-d9284fefec42" />

#Top view
<img width="1919" height="1079" alt="Top" src="https://github.com/user-attachments/assets/4c309bd8-d4b5-48ae-962a-82d7802e7d34" />

#Bottom view
<img width="1919" height="1079" alt="bottom" src="https://github.com/user-attachments/assets/61e89156-caf5-42ac-9bcb-988e24a58c8b" />
