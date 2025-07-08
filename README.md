# Theory behind Soil Moisture Sensor

There are a few types of soil moisture sensors. 
The one used for this project has two parts; the soil moisture probe and an electronic module.
The probe looks like a fork and acts as a variable resistor. 
It has two pins which should be connected to the two pins of the electronic module.
The resistance of the probes varies according to the wetness of the soil.
When the soil is wet, it has water, which induces a small amount of current. 
According to Ohm's law, resistance and current are inversely proportional to each other.
Hence due to this formation of current, the resistance of the probes would decrease.
Alternatively, when the soil is dry and no or less water is detected in the soil, then the resistance of the probes would increase.
Therefore, it is important to note that the value of the resistance of the probe is the output collected from the sensor and not directly the amount of moisture in the soil.

# What's done in this project?

This is a smart plant monitoring system, where it would work out if the water content in the soil in sufficient for the plant and takes actions based on the input. 
Here, we need to give a threshold value for the system to decide if the soil is dry or wet.
If the soil is dry, there is no or less current detected by the soil moisture sensor, which would in turn have a high resistance value, particularly more than the threshold value. When the resistance is high, the program would light up the red LED, indicating less water and the relay connected to the water pump opens, allowing water to flow through the pump to the plant.
If the soil is wet, there is more current detected by the soil moisture sensor, which would in turn have a low resistance value, particularly less than the threshold value. When the resistance is low, the program would light up the green LED, indicating the presence of adequate amount of water and the relay connected to the water pump closes, discontinuing the flow of water through the pump to the plant.
Hence, the plant is looked after automatially without any human intervention.
