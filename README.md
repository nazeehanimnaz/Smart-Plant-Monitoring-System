 <div align="justify"> 

## __WHAT IT DOES__
This is a smart plant monitoring system. <br>
 - It detects the moisture levels of the soil.
 - When the soil is dry, the red LED switches on and water is pumped into the soil for 2 seconds.
 - Then checks again if the soil is still dry.
 - If it is still dry, the red LED stays switched on and water is pumped again for 2 seconds.
 - If the soil is wet enough, the red LED switches off and the green LED switches on, indicating there is enough water and the water is not pumped.

<br>

## __COMPONENTS USED__

1. Arduino UNO x1.
2. Small Breadboard x1.
3. 3.7V 3500mA 18650 Li-ion Rechargeable Battery x1.
4. Switch x1.
5. 5V Relay Module x1.
6. 9V Battery x1.
7. 3-6V DC Motor Submersible Pump x1.
8. Jumper wires (as needed).
9. Red LED x1.
10. Green LED x1.
11. Resistive soil moisture sensor with module x1.

## __EXTRA COMPONENTS NEEDED__

15. Battery chargers.
16. Battery holders, brackets, protective case, etc. (if needed).
17. Water container to fill water needed for spraying.
18. Long tube to spray water.
19. Two flower pot, one with dry soil and the other with wet soil.
20. Cardboards, color papers, etc. (for props and decorations).

<br><br>

_IMPORTANT NOTE: There are 2 types of soil moisture sensor widely available for simple demostrations. The resistive soil moisture sensor is widely used, but it could get corroded easily and also give faulty readings in certain cases. For example, if fertilizer is added to the soil, the resistance of the soil decreases. Since the resistive soil moisture sensors detect moisture using the resistance, the readings change even without the involvement of water. Therefore this method is not sufficient for instances where highly accurate readings are required. In contrast, capacitive soil moisture sensors measure the amount of ions present in the soil to indicate if the soil is wet or dry, hence provide more accurate readings. It is also marketed as rust-resistance. The type of sensor can be selected depending on your demonstration. If it is for a simple school project and does not require highly accurate values, go with a resistive soil moisture sensor. If the readings must be highly accurate in every soil condition, then go with capacitive soil moisture sensor. It is also important to remember that capacitive sensors are not perfect and more sensitive and powerful soil moisture sensors exist, but with high cost._

<br>

## __THE THEORY BEHIND__

1. _How is everything powered up?_ <br>
   - The rechargeable battery powers up the Arduino. Then through the 5V pin of the Arduino, the soil moisture sensor and the relay module are powered up. The submersible water pump is powered up by the 9v battery.<br>
  
2. _How does the resistive soil moisture sensor detect the moisture levels in the soil?_ <br>
   - A resistive soil moisture sensor consists of a probe which has a fork-like structure. This probe is made out of resistive material, hence it acts as a variable resistor. The resistance of the probes varies according to the wetness of the soil. When the soil is wet, it has water, which induces a small amount of current. According to Ohm's law, resistance and current are inversely proportional to each other. Hence due to this formation of current, the resistance of the probes would decrease. Alternatively, when the soil is dry and no or less water is detected in the soil, then the resistance of the probes would increase. Therefore, it is important to note that the output collected from the sensor is the resistance of the probe and not directly the amount of moisture in the soil. <br>
  
3. _How does the water get sprayed?_ <br>
   - The soil moisture sensor detects and gives the readings of the amount of resistance. Once the reading goes above the threshold value, the soil is considered dry and a signal is sent to the Arduino. Arduino sends a signal to the red LED to light up and the green LED to go off. Arduino also sends a signal to the relay module. The relay closes the switch, turning on the motor pump for 2 seconds according to the program.

<br>

## __TIPS__

1. Use high quality batteries for efficiency.
2. Remove the wire connected to the VIN pin of Arduino before connecting the Arduino to the PC/laptop to upload the code. Once the code is uploaded, disconnect the Arduino from the PC/laptop and connect the wire back to the VIN pin of the Arduino. This is to prevent too much voltage flowing into the Arduino via the laptop and the batteries.
3. Always check the readings given by the soil moisture sensor via the Serial Monitor and change the threshold value accordingly.
4. The most common issue while making robotics projects is that the wires break too soon. Either better wires instead of jumper wires should be used, or use a multimeter to constantly check if the jumper wires are in good condition.

<br>

## __PROBLEMS FACED AND SOLUTIONS__

1. _Why does my relay keep switching on even when the soil is wet?_ <br>
   There are 2 main reasons for this; <br>
      - The wires of the soil moisture sensor are loose, making the sensor switch on and off. This would give lower and higher values simultaneously, causing the relay to switch on. Secure the wires with strong tape or by soldering.<br>
      - The threshold value could be too low. Increase the threshold value in the program according to your preference. <br>

2. _Why does the motor pump not pump water even when the relay switches on?_ <br>
   - If the connections are all good and it still does not work, the issue could be with the 9V battery. There might not be enough voltage to power up the motor pump. Check the voltage of the battery with a multimeter. If it is lower than 4v, replace the battery with a new one and try again. <br>

6. _Why are my readings seem to be inaccurate?_ <br>
   There are 2 main reasons for this; <br>
   - The soil moisture sensor could be faulty <br>
   - The soil moisture sensor could have corroded. Replace the sensor and give power to the sensor only when you demostrate your project. Always wipe the sensor clean after use. This could minimize corrosion. <br>






</div>
   

   





