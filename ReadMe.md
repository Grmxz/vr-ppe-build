<span style="color:yellow">**WARNING**</span> This project is only compatible with the HP Omnicept reverb G2 VR Headset.

<span style="color:yellow">**WARNING**</span> If you are using a different device the data from the sensors will not be recorded and the controllers may not be recognized.

This project aims to develop a virtual reality application to register, verify and validate the sensors' data of the HP Omnicept Reverb G2 VR Headset.

The Headset has four sensors:

- Eye Tracking
- Pupillometry
- Heart rate
- Cognitive Load

The Cognitive Load Sensor has the premise to calculate the mental effort of the user through an artificial intelligence based on the user's physiological data acquired by the other sensors when executing tasks. Therefore, the project is mainly focused on analyzing the data from this sensor.

The virtual reality application was developed using Unity. Three scenes was developed, each one with different tasks to stimulate the Cognitive Load Sensor.

For each played session the sensors' data are saved in a csv file. A python application was developped to read the csv file, manipulate the data and plot charts, facilitating data analysis.


<span style="color:red">**IMPORTANT**</span>
To configure the environment to use the headset, go check: [Setup](./Instructions/setup.md)

For more informations of how to configure and play the scenes, go check:
[Instruction](./Instructions/instructions.md)

In order to understand the sensors'data and the python application go check:
[Sensors](./Instructions/sensors.md)