
# BMV080
## Ultra-mini Particulate Matter Sensor

![Image of BMV080 sensor held between fingers]

**BMV080 Ultra-mini Particulate Matter Sensor – Datasheet**

- **Document revision**: 1.3
- **Document release date**: May 2025
- **Document number**: BST-BMV080-DS000-11
- **Sales part number(s)**: 0273.017.054-1NV
- **Notes**: 
  - Data and descriptions in this document are subject to change without notice.
  - Product photos and pictures are for illustration purposes only and may differ from the real product appearance.


---


# Basic description

## Introduction

The BMV080 particulate matter sensor is an ultra-mini opto-electronic sensor capable of measuring particulate matter mass concentration. It delivers real-time measurements for particulate matter with diameters equal to or smaller than 2.5 µm (PM2.5). The sensor also offers mass concentration of particulate matter with diameters equal to or smaller than 1 µm (PM1) and equal to or smaller than 10 µm (PM10), enabling a comprehensive understanding of air quality across various particulate size ranges. The BMV080 measures naturally and freely moving particulate matter by using the ambient airflow close to the sensor. Its novel measurement principle, revolutionary small size, and low power consumption enable its integration into ultra-compact Internet of Things (IoT) devices such as air quality monitors, smart thermostats, smart air purifiers, and wearables.

The BMV080 has the following features:

- Ultra-compact form factor
- Precise particulate matter concentration measurement
- Innovative fanless design
  - Noiseless device operation
  - No inlets or channels needed – minimum industrial design impact on the host system
  - Maintenance free
  - Novel principle, measuring in free space
  - Enables dust-proof or waterproof integration

## Particulate matter and health

Air pollution is a major environmental risk to health. Studies and research on airborne particulate matter and its impact on public health consistently show evidence of adverse health effects at specific exposure levels. While the range of health effects is broad, the respiratory and cardiovascular systems are the most affected by exposure to particulate matter. Adverse health effects have been demonstrated even for relatively small increases in particulate concentration compared to clean air conditions.

While particulate matter comes in a vast range of particle sizes, the biggest impact on human health is from particulates in the PM2.5 range, which comprises all particles smaller than or equal to 2.5 µm in diameter. Due to its small size, PM2.5 particulates can easily enter deep into the human respiratory system and provoke serious health problems.

The World Health Organization (WHO) set different air quality guidelines to assess the health effects of air pollution and thresholds for health-harmful pollution levels. As exposure to PM2.5 can cause both short-term and long-term effects, the latest WHO recommended guidelines as of 2021 ([WHO global air quality guidelines, Table 0.1](#)) provide two threshold levels related to the annual and the 24-hour mean:

- 5 µg/m³ annual mean
- 15 µg/m³ 24-hour mean

Different countries worldwide use different air quality standards, also known as Air Quality Indices (AQI), to communicate current and future air pollution levels to the public. PM2.5 concentration is one of the pollutants considered in the calculation of each AQI. For example, the United States Environmental Protection Agency (EPA) defined a standard to correlate exposure to PM2.5 to air quality.

Table 1 shows PM2.5-specific AQI sub-indices and the relative cautionary statements.

[Table 1: PM2.5-specific AQI sub-indices and cautionary statements]


---

# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## Table 1: PM2.5 specific AQI and cautionary statements defined by the EPA

| PM2.5 breakpoints (µg/m³, 24-hour average) | Air quality index (AQI) category | Air quality index description |
|--------------------------------------------|---------------------------------|-------------------------------|
| 0.0 – 12.0                                 | Good                            | Air quality is satisfactory, and air pollution poses little or no risk. |
| 12.1 – 35.4                                | Moderate                        | Air quality is acceptable. However, there may be a risk for some people, particularly those who are unusually sensitive to air pollution. |
| 35.5 – 55.4                                | Unhealthy for sensitive groups  | Members of sensitive groups may experience health effects. The general public is less likely to be affected. |
| 55.5 – 150.4                               | Unhealthy                       | Some members of the general public may experience health effects; members of sensitive groups may experience more serious health effects. |
| 150.5 – 250.4                              | Very unhealthy                  | Health alert: the risk of health effects is increased for everyone. |
| > 250.4                                    | Hazardous                       | Health warnings of emergency conditions: everyone is more likely to be affected. |

## 1.3 Operating principle

The BMV080 sensor uses a laser-based optical technology to measure particulate matter mass concentration based on particle counts and relative particle velocities in free space, as illustrated in Figure 1. The natural ambient airflow in the proximity of the sensor is utilized in the measurement. Figure 1 shows how light is scattered after colliding with particles in different directions. The light continues at the top of the particle to indicate the light path when there is no collision.

![BMV080 sensor operating principle](#)

*Figure 1: BMV080 sensor operating principle*

The measurement procedure is as follows:

- Laser light is emitted from the sensor and focused by the sensor lens at approximately 5 mm from the top of the sensor’s lens surface.
- Particles traveling in free space due to the natural ambient airflow are detected when passing through the laser focal (sensitive) region.

---


## Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

- Due to the interaction between particles and light, the light scatters in different directions; a fraction is back-scattered towards the sensor, where the integrated photo-detectors detect it.
- The back-scattered signal is processed by unique algorithms (based on particle counts, particle relative velocity, probed air volume during measurement) to derive the particulate matter mass concentration.

The BMV080 consists of hardware and software components.

Figure 2 shows a BMV080 sensor integrated into a host system, where the BMV080 sensor driver (software) runs on the host processing unit (e.g., MCU).

![BMV080 with hardware and software components](#)

*Figure 2: BMV080 with hardware and software components*


---


# Table of contents

## 1 Basic description

1.1 Introduction  
1.2 Particulate matter and health  
1.3 Operating principle  

## 2 Technical specifications

2.1 Standard test conditions  
2.2 Sensor technical specification  
2.3 Storage conditions  
2.4 Measurement modes  
   2.4.1 Continuous measurement mode  
   2.4.2 Duty cycling measurement mode  
2.5 Power consumption  

## 3 Dimensional drawings

3.1 Schematic  
3.2 Flex PCB  

## 4 Hardware integration guidelines

4.1 Mechanical interface  
   4.1.1 Environmental considerations  
   4.1.2 BMV080 footprint  
   4.1.3 Mounting and assembly  
   4.1.4 Handling and mounting guidelines  
4.2 Thermal interface  
4.3 Optical interface  
   4.3.1 Mechanical properties  
   4.3.2 Optical properties  
4.4 Electrical and communication interface  
   4.4.1 Electrical interface  
   4.4.2 Communication interface  
4.5 Maintenance and service  

## 5 Software integration guidelines (Sensor driver)

5.1 Host requirements  
5.2 Application programming interface  
   5.2.1 Typedefs  
   5.2.2 Driver version  
   5.2.3 Sensor management  
   5.2.4 Sensor identification  
   5.2.5 Particulate matter measurement  


---


# 6 Traceability

# 7 Product compliance

## 7.1 Environmental safety

### 7.1.1 RoHS

### 7.1.2 Halogen content

## 7.2 Laser safety

### 7.2.1 Conformity and classification

# 8 Additional material

# 9 Legal disclaimer

## 9.1 Engineering samples

## 9.2 Product use

## 9.3 Application examples and hints

# 10 Document history and modifications


---


# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## List of Figures

- **Figure 1:** BMV080 sensor operating principle ................................................................. 3
- **Figure 2:** BMV080 with hardware and software components ........................................... 4
- **Figure 3:** BMV080 characteristics - correlation to the reference device ........................... 9
- **Figure 4:** Continuous measurement mode integration timing ........................................ 12
- **Figure 5:** Duty cycling measurement mode integration timing ....................................... 12
- **Figure 6:** BMV080 package overview ........................................................................... 14
- **Figure 7:** BMV080 dimensional drawings (dimensions in mm) ....................................... 15
- **Figure 8:** BMV080 flex PCB footprint ........................................................................... 15
- **Figure 9:** Maximum bending angles and minimum bending radius ................................ 16
- **Figure 10:** ZIF connector in detail (dimensions in mm) .................................................. 16
- **Figure 11:** Comparison of pin numbering schemes for BMV080 and ZIF connectors ....... 17
- **Figure 12:** BMV080 hardware design interfaces .......................................................... 18
- **Figure 13:** Placement of BMV080 away from sharp edges ............................................ 19
- **Figure 14:** BMV080 integrated in a host system .......................................................... 19
- **Figure 15:** Concept 1: Case mounting ......................................................................... 20
- **Figure 16:** Placement of PCB for the sensor position ................................................... 21
- **Figure 17:** Process flow for concept 1 - Case mounting ............................................... 21
- **Figure 18:** Concept 2 – PCB mounting ......................................................................... 22
- **Figure 19:** Process flow for concept 2 – PCB mounting ............................................... 22
- **Figure 20:** Maximum forces applied to the LGA package .............................................. 23
- **Figure 21:** Sketch of the thermal integration situation .................................................. 23
- **Figure 22:** Sketch of the optical interface .................................................................... 24
- **Figure 23:** BMV080 pin schematic .............................................................................. 25
- **Figure 24:** Top view of the bottom metal of the flex PCB showing the connector pins numbering ............................................................................................................. 26
- **Figure 25:** Different configurations for protocol selection (SPI / I²C) ............................. 26
- **Figure 26:** Power-supply configuration with a single supply rail .................................... 28
- **Figure 27:** Power-supply configuration with the lowest voltage level ............................ 29
- **Figure 28:** Power-up sequence diagram ...................................................................... 30
- **Figure 29:** Power-supply configuration with separated analog and digital domains ....... 30
- **Figure 30:** SPI 4-wire read mode 0 .............................................................................. 31
- **Figure 31:** SPI 4-wire write mode 0 ............................................................................. 32
- **Figure 32:** I²C read ...................................................................................................... 32
- **Figure 33:** Complete I²C write ..................................................................................... 33
- **Figure 34:** I²C header transfer ..................................................................................... 33
- **Figure 35:** I²C data read .............................................................................................. 33
- **Figure 36:** The sensor driver is the communication channel between the BMV080 and the user application ......................................................................................... 35
- **Figure 37:** Flow diagram of continuous measurement .................................................. 42
- **Figure 38:** Start-up sequence in case of Continuous Measurement Mode .................... 43
- **Figure 39:** Flow diagram of a duty cycling measurement .............................................. 43
- **Figure 40:** Start-up sequence in case of Duty Cycling Measurement Mode .................. 44
- **Figure 41:** Class 1 laser product .................................................................................. 49


---


# List of Tables

| Table | Description                                                                                     | Page |
|-------|-------------------------------------------------------------------------------------------------|------|
| 1     | PM2.5 specific AQI and cautionary statements defined by the EPA                                 | 3    |
| 2     | Standard test conditions                                                                        | 9    |
| 3     | BMV080 technical specification                                                                  | 10   |
| 4     | Absolute minimum and maximum ratings                                                            | 11   |
| 5     | Storage conditions for BMV080                                                                   | 11   |
| 6     | Power Consumption                                                                               | 13   |
| 7     | BMV080 package dimensions                                                                       | 14   |
| 8     | Given parameters for the thermal setup                                                          | 24   |
| 9     | Optical interface mechanical properties                                                         | 24   |
| 10    | Properties of optical cover                                                                     | 25   |
| 11    | BMV080 pin description                                                                          | 27   |
| 12    | Power domains specification and current consumption                                             | 28   |
| 13    | Pin functions depending on selected protocol                                                    | 31   |
| 14    | Host interface - I²C device address selection                                                   | 32   |
| 15    | BMV080 sensor driver technical requirements for embedded systems                                | 35   |
| 16    | BMV080 marking convention                                                                       | 48   |


---


# 2 Technical specifications

## 2.1 Standard test conditions

Table 2 specifies the BMV080 sensor under the laboratory standard test conditions. Deviation from the standard test conditions may impact the sensor performance.

**Table 2: Standard test conditions**

| Parameter                  | Value                                      | Unit  |
|----------------------------|--------------------------------------------|-------|
| Ambient temperature        | 25 ± 2                                     | °C    |
| Relative ambient humidity  | 50 ± 10                                    | %rH   |
| Relative particle velocity | 0.1 – 1.5                                  | m/s   |
| Relative particle flow     | Laminar, plane parallel                    | –     |
| Reference instrument       | Aerosol particle size spectrometer LAP 322 | –     |
| Particle source            | Arizona Road Dust (ARD) Ultrafine A1, ISO 12103-1 | –     |
| Integration time           | 10                                         | s     |
| Vibration suppression      | Disabled                                   | –     |
| Measurement algorithm      | High precision[^1]                         | –     |

To precisely estimate the particle mass concentration, the BMV080 must gather sufficient statistical data. To obtain best results in low PM2.5 concentration situations (i.e., < 12 µg/m³) when few particles are present in ambient air, an integration time (IT) of 10 s has been used for standard test conditions.

The sensor performance is specified using the following parameters:

- **Precision [ε]**: linear regression residual (how much does PM2.5 fluctuate under standard test conditions when test is repeated)[^2]
- **Linearity [R]**: Pearson correlation coefficient (linearity of response to proportional changes)

Figure 3 shows the correlation between a single BMV080 and the reference device under standard test conditions.

![Figure 3: BMV080 characteristics - correlation to the reference device](#)

[^1]: Refer to Section 5.2.1.2.
[^2]: For more details refer to Technical Specification Statement (BST-BMV080-AN002).


---


## 2.2 Sensor Technical Specification

This section describes the technical specification of the BMV080 sensor.

### Table 3: BMV080 Technical Specification

| Parameter                           | Symbol     | Typical Value                              |
|-------------------------------------|------------|--------------------------------------------|
| PM2.5 measurement range<sup>3</sup> | –          | 0 – 1000 µg/m³                             |
| PM2.5 output resolution<sup>3</sup> | –          | 1 µg/m³                                    |
| Minimum detectable particle size<sup>3</sup> | – | 0.5 µm                                     |
| Relative particle velocity<sup>3</sup> | –        | 0.02 – 1.5 m/s                             |
| Precision<sup>3, 4</sup>            | ε          | ± 10 µg/m³ @ 0 – 100 µg/m³                 |
|                                     |            | ± 10 % @ 101 – 1000 µg/m³                  |
| Linearity<sup>3</sup>               | R          | ≥ 0.98 @ 0 – 400 µg/m³                     |
|                                     |            | ≥ 0.95 @ 401 – 1000 µg/m³                  |
| Measurement modes                   | –          | Continuous measurement mode                |
|                                     |            | Duty cycling measurement mode              |
| Measurement algorithm<sup>5</sup>  | –          | High precision                             |
|                                     |            | Balanced                                   |
|                                     |            | Fast response                              |
| Maximum output data rate<sup>6</sup>| ODR        | 0.97 Hz                                    |
| Interface                           | –          | SPI, I²C                                   |
| Average total current<sup>7</sup>   | –          | < 68 mA @ 0.97 Hz ODR                      |
| Sleep current                       | –          | < 30 µA                                    |
| Start-up time<sup>8</sup>           | t<sub>start-up</sub> | 1.9 s – trigger mode: software polling   |
|                                     |            | 2.9 s – trigger mode: IRQ, i.e. hardware interrupt |
| Operating lifetime (MTTF)<sup>9</sup> | –        | 10 years                                   |
| Sensor dimensions<sup>10</sup>      | –          | 4.4 mm x 3.0 mm x 20.0 mm                  |
| Sensor weight                       | –          | 0.092 g                                    |
| Laser class                         | –          | Class 1, according to IEC 60825-1          |

Table 4 shows the absolute minimum and maximum ratings of the sensor BMV080.

Stress above limits, which are stated as “absolute maximum ratings” in Table 4, may cause permanent damage to the device. These are stress ratings only and functional operation of the device under those conditions or any conditions beyond those indicated as “recommended operating conditions” is not implied. Exposure to absolute maximum rating conditions for extended periods may affect device reliability. Hence, it is recommended to perform a qualification according to the intended use-case environment.

---

<sup>3</sup>Specified under the standard test conditions defined in Section 2.1. Deviation from standard test conditions may impact sensor performance. Tolerance intervals cover 99 % of the population (95 % confidence interval).

<sup>4</sup>Precision is defined as variation around average PM2.5 value during stable conditions within a 90 s window after a 30 s stabilization time.

<sup>5</sup>Algorithms “High precision” and “Balanced” are only available in continuous measurement mode.

<sup>6</sup>ODR is configurable, i.e., using duty cycling measurement mode.

<sup>7</sup>During active measurement.

<sup>8</sup>For more details refer to the timing sequence information given in Sections 5.2.5.1.1 and 5.2.5.1.2.

<sup>9</sup>This applies for a sensor in integrated condition as defined in Section 4.1.3 of this datasheet and the Integration Guidelines (BST-BMV080-AN00), assuming continuous 24-hour daily operation under standard test conditions (see Table 2) for an indoor air quality application. Actual sensor lifetime may vary depending on operating conditions.

<sup>10</sup>Refer to Table 7.


---

# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## Table 4: Absolute minimum and maximum ratings

| Parameter                      | Minimum          | Maximum          |
|-------------------------------|------------------|------------------|
| Supply voltages<sup>11</sup>  |                  |                  |
| VDDIO                         | 1.2 V (-5 %)     | 3.3 V (+5 %)     |
| VDDD                          | 2.5 V (-5 %)     | 3.3 V (+5 %)     |
| VDDL                          | 3.3 V (-5 %)     | 3.3 V (+5 %)     |
| VDDA                          | 2.5 V (-5 %)     | 3.3 V (+5 %)     |
| ESD                           |                  |                  |
| Human body model (HMB)        | -2 kV            | 2 kV             |
| Charged device model (CDM)    | -500 V           | 500 V            |
| Sensor operating temperature range<sup>12</sup> | +15 °C           | +65 °C           |
| Operating humidity and condensation range<sup>13</sup> | 0 %rH           | 95 %rH           |

## 2.3 Storage conditions

Table 5 outlines the storage conditions for the BMV080 to ensure its specified lifetime and performance.

### Table 5: Storage conditions for BMV080

| Packing status                        | Storage conditions                  | Remark                      |
|---------------------------------------|-------------------------------------|-----------------------------|
|                                       | Temperature (°C) | Humidity rH (%) | Max Storage Time            |                             |
| BMV080 drypack sealed (as delivered)  | -40 to +70      | not relevant    | 2 years                     | Regular storage             |
| BMV080 drypack opened under air       | +20 to +30      | < 60 (Air)      | 1 week                      | Handling before integration |
|                                       |                 |                 | Equivalent to MSL3          |                             |
| BMV080 integrated<sup>14</sup> and not operated | +10 to +40      | < 60 (non-condensing) | 18 months                   | Handling after integration  |
| BMV080 drypack opened in N<sub>2</sub> cabinet | +20 to +30      | < 30 (N<sub>2</sub>) | 6 months                    | N<sub>2</sub> flow rate: > 3 l/min |

---

<sup>11</sup> Supply pins are described in Table 11.

<sup>12</sup> Given self heating during operation resulting in sensor internal temperature increase of ~15 K in continuous measurement mode with the Power Optimized Configuration (Chapter 4), BMV080 is capable to operate at ambient temperatures <15 °C depending on thermal integration design. For more details, refer to Section 3.3 on thermal integration best practices in BMV080 integration guideline (BST-BMV080-AN000).

<sup>13</sup> No condensation allowed on the sensor, especially on the lens and LGA substrate areas circled below.

[Image: Lens and LGA substrate]

<sup>14</sup> Built into the final product following the guidelines in this document.

---


## 2.4 Measurement modes

It is possible to implement different measurement modes using the BMV080 sensor driver presented in Section 5. Once turned ON, the BMV080 sensor can provide a PM reading every second. Taking this into consideration, the following measurement modes can be implemented to save power consumption and increase operating lifetime.

### 2.4.1 Continuous measurement mode

In this mode, BMV080 delivers particle concentrations with the maximum defined Output Data Rate of 0.97 Hz.

[Figure 4: Continuous measurement mode integration timing]

### 2.4.2 Duty cycling measurement mode

In this mode, BMV080 reports a value periodically based on a configured 'duty cycling period'.

[Figure 5: Duty cycling measurement mode integration timing]

**Note:** Precision target as defined in Table 3 does not apply in case of Duty Cycling Measurement mode. Duty Cycling Measurement mode only supports the fast response measurement algorithm.


---


## 2.5 Power Consumption

Table 6 shows the typical power consumption for the different measurement modes.

| Measurement mode   | Duty cycling period       | Power consumption (mW)<sup>15</sup> |
|--------------------|---------------------------|-------------------------------------|
| **Duty cycling mode** | 1 min                     | 30.4                                |
|                    | 1 measurement in 1 min     |                                     |
|                    | 5 min                      | 6.2                                 |
|                    | 1 measurement in 5 min     |                                     |
|                    | 10 min                     | 3.1                                 |
|                    | 1 measurement in 10 min    |                                     |
|                    | 60 min                     | 0.6                                 |
|                    | 1 measurement in 60 min    |                                     |
| **Continuous mode** | Not applicable             | 181.9                               |
| 1 measurement every 1 s |                       |                                     |

<sup>15</sup>Power consumption estimation is based on electrical integration of the BMV080 based on Power Optimized Configuration as per 4.4.1.3.2.


---


# 3 Dimensional Drawings

## 3.1 Schematic

Figure 6 shows the BMV080 package. The sensor consists of the following components:

- LGA package
- Lens
- Flex-PCB

![Figure 6: BMV080 package overview](image-description)

Table 7 provides the BMV080 package dimensions and is further detailed in Figure 7. A 3D CAD model of the BMV080 design to support the integration in a host system is available on request, see Section 8.

| Parameter                | Nominal dimension [mm]            |
|--------------------------|-----------------------------------|
| **Flex PCB size**        |                                   |
| Width                    | 5.5 (with ears of ZIF connector)  |
|                          | 4.4 (without ears)                |
| Length                   | 20.0                              |
| **Total height**         | 3.005                             |
| **Lens height**          | 1.83                              |
| **LGA package thickness**| 0.94 ... 1.22                     |
| **FPC thickness**        | 0.38                              |


---


# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

![BMV080 dimensional drawings](image-description)

*Figure 7: BMV080 dimensional drawings (dimensions in mm)*

## 3.2 Flex PCB

Bending of the Flex-PCB is only allowed in the bending area highlighted with red rectangle shown in Figure 8 with maximum bending angle of 90° in clockwise direction and 180° in counterclockwise direction. Minimum bending radius is 0.5 mm, as shown in Figure 9.

![BMV080 flex PCB footprint](image-description)

*Figure 8: BMV080 flex PCB footprint*


---

# BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## Maximum Bending Angles and Minimum Bending Radius

![Figure 9: Maximum bending angles and minimum bending radius](#)

The connector area of the BMV080’s flex PCB is compatible with the following ZIF connectors (used in the host system):

- Molex 503566-1302, Easy-On FPC connector, 0.30 mm pitch, 13 circuits, mated height 0.95 mm
- KYOCERA AVX, Series 6844, Part number: 046844713002846+
- Greenconn CFTD104-1302A001C2AD

Details of the connector area of the flex PCB are shown in Figure 10.

![Figure 10: ZIF connector in detail (dimensions in mm)](#)

**Note:**

Please be aware that the pin numbering scheme used for the BMV080 sensor (Figure 24) might differ from the pin numbering schemes of the ZIF connectors which are used in the host system (see list above). For a comparison please refer to Figure 11.

---


# BMV080 Pin Schematic

![BMV080 pin schematic and ZIF connector pin schematic (example)](image-description)

**Figure 11:** Comparison of pin numbering schemes for BMV080 and ZIF connectors

- **BMV080 Pin Schematic**
  - Top View: 01 to 13
  - Bottom View: 13 to 01

- **ZIF Connector Pin Schematic (Example)**
  - Pins: 1, 3, 5, 7, 9, 11, 13 (bottom row)
  - Pins: 2, 4, 6, 8, 10, 12 (top row)


---


# Hardware Integration Guidelines

The BMV080 has 4 hardware design interfaces, shown in Figure 12. Detailed requirements for each interface are specified in the following sections:

- **Mechanical**: contains environmental considerations as well as information about footprint, handling and mounting of the sensor into the host. In addition, important advice with respect to contamination is given.
- **Thermal**: thermal connection to the host for dissipating heat generated by the sensor.
- **Optical**: optical components added by the host to the sensor optical path, e.g., optical cover.
- **Electrical & Communication**: electrical connections for power and data communication between the sensor and host.

![BMV080 Hardware Interfaces](image-description)

*Figure 12: BMV080 hardware design interfaces*

## Mechanical Interface

### Environmental Considerations

The BMV080 measures particulate matter mass concentration in a probing region at approximately 5 mm above the sensor lens surface. To ensure the sensor’s functionality and performance, it is recommended to follow these requirements for sensor placement:

- **Sensor location in the host system**: place the BMV080 minimum 17 mm away from sharp edges to avoid turbulent air flows that could affect the sensor performance, see Figure 13.
- **Objects in front of the sensor (obstruction)**: reflections caused by objects in the optical path can influence the sensor functionality. The BMV080 software detects these events as obstructions. While occasional obstruction (e.g., by waving hands) is filtered out in the BMV080 software and does not influence the sensor performance, static obstruction (i.e., a fixed object in the obstruction-sensitive region, see Figure 14) will influence the sensor functionality. When the BMV080 software detects a static obstruction, the PM2.5 calculation is not available, and an obstruction flag is returned. Therefore, static obstructions caused by the integration into the host shall be avoided.


---


# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

![Figure 13: Placement of BMV080 away from sharp edges](#)

![Figure 14: BMV080 integrated in a host system](#)

The optical properties and the geometry of the object(s) in the optical path of the BMV080 determine the size of the obstruction-sensitive region. For a white reflecting surface perpendicular to the laser light emitted by the BMV080, this distance is ≥ 350 mm from the host surface. This distance reduces for less reflecting objects (e.g., skin).


---


## 4.1.2 BMV080 Footprint

A detailed description of the BMV080 footprint, dimensions, used connectors, and drawings can be found in Chapter 3.

## 4.1.3 Mounting and Assembly

The mounting and assembly concept must fulfill the following requirements to ensure functional integration of the BMV080 into a host system:

- Mechanically fix the BMV080 in the host system
- Protect the BMV080 (e.g., lens) from damage
- Correct positioning to ensure a clear optical path for the sensor optics
- Enable electrical connection to the host system
- Enable thermal connection to the host system
- The mounting position within host has to ensure that
  - no humidity (for example coming from any condensation) covers the lens, optical cover inner surface or any other part of the integrated BMV080,
  - no contamination is applied on the lens and the inner surface of the optical cover of the integrated BMV080 (this could be achieved, e.g., by using a clean room environment for the assembly process. Manufacturing and test of the sensor at Bosch Sensortec is performed in an ISO 7 clean room environment).

The following sections describe two mounting and assembly concept examples.

The BMV080 is placed inside a cavity formed into the housing structure of the host system that includes the optical cover, as shown in Figure 15. The cavity’s shape and dimensions define the sensor’s position inside the housing structure and ensure the required clearance between the BMV080 and the optical cover (Section 4.3). The BMV080 needs to be fixed in the cavity from the backside, and a thermal connection needs to be enabled (Section 4.2). This can be done, for example, with a plastic component (e.g., molded polymer) that includes a metal spring and is attached to the housing structure with a clip structure.

This concept has the following options:

- Precise control of the clearance between the BMV080 lens and the optical cover
- Flexibility to place the PCB for the sensor position (side by side, stacked, etc. – see Figure 16).

### 4.1.3.1 Concept 1: Case Mounting

![Concept 1: Case Mounting](image-url-placeholder)

*Figure 15: Concept 1: Case mounting*


---


# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

![Placement of PCB for the sensor position](image-placeholder)

*Figure 16: Placement of PCB for the sensor position*

Figure 17 shows an example assembly process for Concept 1 – Case mounting.

![Process flow for concept 1 - Case mounting](image-placeholder)

*Figure 17: Process flow for concept 1 - Case mounting*

## 4.1.3.2 Concept 2: PCB mounting

The BMV080 is mounted directly on the host PCB, working simultaneously as a mechanical fixation and thermal connection. For example, BMV080 can be fixed to the host PCB using a cage system (Figure 18). Different options can be used to fix the cage system to the host PCB, for example, screws. Clearance between the BMV080 lens and cover glass has to be ensured by the fixation of the PCB in the host housing (for info about clearance, refer to Section 4.3.1).


---


# PCB Mounting

![Top view without cage and with cage](image-description)

*Figure 18: Concept 2 – PCB mounting*

This concept allows for the following options:

- Use PCB as a heat sink
- Direct mounting on host PCB

Figure 19 shows an assembly process flow example recommended for Concept 2 – PCB mounting.

![Process flow diagram for PCB mounting](image-description)

*Figure 19: Process flow for concept 2 – PCB mounting*


---


# 4.1.4 Handling and Mounting Guidelines

During the assembly process, the following handling guidelines must be considered to avoid any damage to the sensor:

- Maximum forces applied to the LGA package (Figure 20)
  - \( F_{\text{max, x}} = 5 \, \text{N} \)
  - \( F_{\text{max, y}} = 5 \, \text{N} \)
  - \( F_{\text{max, z}} = 3 \, \text{N} \)
- Avoid any force on the lens
- Avoid any contamination on the lens surface (e.g., fingerprints, dust)

![Figure 20: Maximum forces applied to the LGA package](#)

## 4.2 Thermal Interface

The BMV080 sensor needs to be connected to a cooling system to dissipate the heat generated by the sensor.

Figure 21 shows a simplified overview of a thermal setup. The lower surface of the BMV080 Flex-PCB is attached to a cooling element (e.g., a heat sink) via a thermal contact (in this case a tape). The heat sink itself is part of the host system.

![Figure 21: Sketch of the thermal integration situation](#)

When designing the thermal interface from the BMV080 Flex-PCB to the host, the following parameters must be considered, see Table 8.


---

# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## Table 8: Given parameters for the thermal setup

| Parameter                                      | Value   |
|------------------------------------------------|---------|
| Maximum sensor operating temperature           | 65°C    |
| Maximum power (continuous measurement) (P_max) | 181.9 mW|

The maximum sensor operating temperature is 65 °C, the sensor internal temperature increase is 15 K due to power dissipation in the sensor (This value is based on continuous measurement mode).

Please refer to Section 3.3 in BMV080 integration guideline for more details on thermal integration best practices.

## 4.3 Optical interface

In the host system, the BMV080 has to be integrated behind an optical cover to protect the lens from contamination (e.g., fingerprints, dust) and mechanical damage in the application. This section covers the mechanical and optical properties of the optical cover.

### 4.3.1 Mechanical properties

- **Optical cover thickness (d) and clearance (σ) between the lens and optical cover**: the sensor-sensitive region is located approx. 5 mm above the lens surface. It must be ensured that the sensitive region is above the optical cover – outside the housing in free air.
- **Optical window width (φ)**: the optical cover has to be wide enough to transmit the laser beams.
- **Maximum tilt angle (α) between the optical cover and the BMV080**: the lens surface and the optical cover have to be almost parallel to avoid distortion of the optical signal.

[Figure 22: Sketch of the optical interface]

## Table 9: Optical interface mechanical properties

| Parameter                                      | Symbol | Value          | Unit |
|------------------------------------------------|--------|----------------|------|
| Optical cover thickness                        | d      | 0.3 ≤ d ≤ 0.8  | mm   |
| Optical window width                           | φ      | ≥ 1.4          | mm   |
| Tilt angle                                     | α      | ≤ 4            | °    |
| Clearance between the top of the BMV080 lens and the bottom of the optical cover | σ      | 0.2 ± 0.1      | mm   |

---


Scratches and damage on the optical cover can affect the sensor performance. A hard material like glass is recommended (e.g., Corning® Gorilla® Glass 6).

The optical cover must be kept free from fingerprints, dust, and other impurities and contamination.

### 4.3.2 Optical properties

- **Refractive index**: this parameter influences the laser beam shape, and therefore it needs to be specified to avoid affecting the sensor performance.
- **Transmissivity**: the cover glass must allow the transmission of the laser beams. A transmissivity below specifications will decrease the optical signal intensity, thus affecting the sensor functionality.

Optical properties are specified in Table 10.

| Parameter        | Typical value                                           |
|------------------|---------------------------------------------------------|
| Refractive index | 1.45 – 1.77 for λ = 850 nm                              |
| Transmissivity   | ≥ 90 % for an angle of incidence of 30°, P-polarization, λ = 850 nm |

Additional requirements to the optical cover:

- Optical surface roughness needed to avoid any beam distortion
- Avoid any polarization filter

## 4.4 Electrical and communication interface

The BMV080 is connected to the host system by the electrical interface for data communication and power supply.

### 4.4.1 Electrical interface

#### 4.4.1.1 Pin configuration and function

Figure 23 shows a pin schematic of the BMV080. Figure 24 shows the BMV080 flex-PCB. Table 11 shows the functional description of each pin.

![Figure 23: BMV080 pin schematic](#)


---

# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## Top View and Bottom View

![Top and Bottom View of PCB](image-description)

*Figure 24: Top view of the bottom metal of the flex PCB showing the connector pins numbering*

## Protocol Select (PS) Pin

The protocol select (PS) pin is a logic input to configure the type serial interface, SPI, or I²C. Figure 25 shows how the PS pin can be connected to select the SPI or the I²C protocol. The SPI protocol is selected when this pin is connected to a logic low (VSSD). If this pin is connected to a logic high (VDDIO), the I²C protocol is selected. If this pin is not connected (not recommended), the I²C protocol is selected. The pin state is latched during power-up by the digital core.

![Different configurations for protocol selection (SPI / I²C)](image-description)

*Figure 25: Different configurations for protocol selection (SPI / I²C)*

---

© Bosch Sensortec GmbH 2025 | All rights reserved, also regarding any disposal, exploitation, reproduction, editing, distribution, as well as in the event of applications for industrial property rights

Document number: BST-BMV080-DS000-11

---


# Table 11: BMV080 Pin Description

| Label        | Pin no. | Type 16 | Description                                                                 |
|--------------|---------|---------|-----------------------------------------------------------------------------|
| **VDDL**     | 1       | P       | **Laser supply voltage.**<br>The laser supply voltage is 3.3 V and the supply pin should be decoupled from VSSA by >1 µF. |
| **VDDA**     | 3       | P       | **ADC supply voltage.**<br>The ADC supply voltage is 2.5 V– 3.3 V which should be decoupled from VSSA by >1 µF. |
| **VDDD**     | 10      | P       | **Digital supply voltage.**<br>The digital supply voltage is 2.5 V to 3.3 V which should be decoupled from VSSD by >1 µF. |
| **VDDIO**    | 8       | P       | **Interface power supply.**<br>The interface power supply is from 1.2 V (min) to 3.3 V (max), with 1.8 V being the typical value. This pin is typically connected to the same supply of the host interface (e.g., application processor, microcontroller, or FPGA). |
| **PS**       | 7       | DI      | **Protocol select. Logic input.**<br>This pin is used to configure the type of serial interface, SPI or I²C.<br>- The SPI protocol is selected if this pin is connected to a logic low (VSSD).<br>- If this pin is connected to a logic high (VDDIO), the I²C protocol is selected.<br>**Note:**<br>- If this pin is not connected (not recommended), the I²C protocol is selected.<br>- The pin state is latched during power-up by the digital core. |
| **VSSA**     | 2       | GND     | **Analog ground.**<br>This pin is the ground reference for all analog domains, namely VDDL and VDDA. Connecting VSSA and VSSD as close as possible to the BMV080 pin header is recommended. |
| **VSSD**     | 9       | GND     | **Digital ground.**<br>This pin is the ground reference for all digital domains, namely VDDD and VDDIO. Connecting VSSA and VSSD as close as possible to the BMV080 pin header is recommended. |
| **SCK**      | 6       | DI      | **Serial clock. Digital input.**<br>This pin functions as serial input for both serial interface protocols (SPI and I²C). |
| **MOSI**     | 5       | DI/DO   | **SPI:** This pin functions as Master Out Slave In (MOSI).<br>**I²C:** This pin functions as a Serial Data line (SDA). |
| **MISO**     | 11      | DI/DO   | **SPI:** This pin functions as Master In Slave Out (MISO).<br>**I²C:** This pin functions as I²C Address Bit 0 (IA0). IA0 allows adjusting the I²C Address Bit 0 of the slave by applying a logic low (VSSD) or logic high (VDDIO). |
| **CSB**      | 4       | DI      | **SPI:** This pin functions as not Slave Select (nSS).<br>**I²C:** This pin functions as I²C Address Bit 1 (IA1). IA1 allows adjusting the I²C Address Bit 1 of the slave by applying a logic low (VSSD) or logic high (VDDIO). |
| **IRQ**      | 12      | DO      | **Interrupt line. Digital out. Active low.**<br>Internal pull-up is enabled by default for IRQ pin. |
| **Do not connect** | 13 | DO    | **Keep pin floating.**<br>Do not connect to ground or apply voltage. |

## 4.4.1.2 Proposal for Filtering Signal Errors

Strong disturbing signals on the SCK pin may influence the measurement results of the BMV080. In an environment where strong disturbance signals are present, the SCK pin could be protected with a suitable low pass filter, which filters out the disturbance but allows normal communication.

---

16P = power supply, DI = digital in, DO = digital out, GND = ground.


---


### 4.4.1.3 Power domains

The BMV080 has four power domains, listed in Table 12. The passive components specific to the four BMV080 power domains are already included on the flex-PCB.

**Table 12: Power domains specification and current consumption**

| Power domain | Electrical specification Min | Max | Power supply rejection ration | Absolute maximum rating | Current consumption Sleep mode | Measurement mode |
|--------------|------------------------------|-----|------------------------------|-------------------------|-------------------------------|------------------|
| VDDIO¹⁷      | 1.2 V - 5 %                  | 3.3 V + 5 % | Ensure dynamically the listed min. and max. supply values | 3.6 V | < 3 µA | 0.8 mA |
| VDDD         | 2.5 V - 5 %                  | 3.3 V + 5 % | Ensure dynamically the listed min. and max. supply values | 3.6 V | < 15 µA | 21.6 mA |
| VDDL         | 3.3 V - 5 %                  | 3.3 V + 5 % | 100 mV VPP at any frequency | 3.6 V | < 3 µA | 18.29 mA |
| VDDA         | 2.5 V - 5 %                  | 3.3 V + 5 % | 100 mV VPP at any frequency | 3.6 V | < 3 µA | 27.0 mA |

¹⁷Reduced SPI speed for VDDIO < 1.8 V.

### 4.4.1.4 Connection diagrams

The following connection diagrams are examples of how to electrically connect the BMV080 to a host system. Other configurations are possible. Common acronyms used in every connection diagram are Voltage Battery (VBAT) and Power Management Integrated Circuit (PMIC).

#### 4.4.1.4.1 Single supply rail

Figure 26 illustrates the simplest connection diagram possible. All four power domains of the BMV080 sensor, i.e., VDDL, VDDA, VDDD, and VDDIO, are powered by the same rail (3.3 V). The power consumption of the BMV080 is the highest since VDDA and VDDD are supplied at the highest voltage possible.

![Figure 26: Power-supply configuration with a single supply rail](#)


Note: The image description is a placeholder and should be replaced with the actual image if available.


---


### 4.4.1.4.2 Power Optimized Configuration

Figure 27 shows the connection diagram targeting lowest power consumption for each BMV080 power domain while keeping the full SPI speed. Therefore, each power domain is supplied at its lowest allowed voltage (See Section 4.4.1.3):

- VDDL is supplied at 3.3 V
- VDDA and VDDD are supplied at 2.5 V
- VDDIO is supplied by a second PMIC that also supplies the host (e.g., Application Processor, Microcontroller, or FPGA).

![Figure 27: Power-supply configuration with the lowest voltage level](#)

Since VDDD and VDDIO do not share the same power rail, a power-up sequence has to be implemented to ensure the latching of the right information during start-up (see Figure 28). For this purpose, it is possible to use a dedicated PMIC (PMIC #2) controlled by the host.

The sequence is as follows:

1. **PMIC #1 supplies the host and also provides VDDIO to BMV080**
2. **The host boots up. After the required period, a digital output (DO) of the host is used to enable the PMIC #2**
3. **PMIC #2 supplies the remaining domains of BMV080, i.e., VDDL, VDDA, and VDDD**

Whenever the BMV080 is not actively measuring, further energy consumption can be saved by turning completely off the BMV080 sensor instead of putting it into sleep mode; a possible realization of this strategy would consist of disabling PMIC #2 through an enable command generated by the host application processor/microcontroller/FPGA.


---


## 4.4.1.4.3 Separated power supply for analog and digital domains

The separation of analog and digital power domains allows the selection of dedicated PMICs for noise and efficiency. While the low noise PMIC #2 supplies the analog domains VDDL and VDDA, the highly efficient PMIC #1 supplies the digital domains, including the host (See Figure 29). Also, the coupling of digital noise from the digital to the analog domain can be efficiently suppressed.

![Power-up sequence diagram](image-placeholder)

*Figure 28: Power-up sequence diagram*

![Power-supply configuration](image-placeholder)

*Figure 29: Power-supply configuration with separated analog and digital domains*

## 4.4.2 Communication interface

The sensor supports the I²C and SPI digital interfaces, where it acts as a slave for both protocols. The I²C interface supports the Standard, Fast and High Speed modes. The SPI interface supports both SPI mode 0 (CPOL = CPHA = '0') and mode 3 (CPOL = CPHA = '1') in 4-wire configuration.

### 4.4.2.1 Interface selection

Interface selection is done automatically based on PS (protocol select) status. If PS is connected to VDDIO, the I²C interface is active. If PS is pulled down, the SPI interface is activated. After power-up, the level on PS is latched. Hence there cannot be any re-selection of the protocol afterwards. For more details, please refer to Section 4.4.1.1.


---


### 4.4.2.2 Pin Assignment

**Table 13: Pin functions depending on selected protocol**

| Pin no. BMV080 ZIF connector | SPI                                      | I²C                                      |
|------------------------------|------------------------------------------|------------------------------------------|
| 6                            | Serial Clock (SCK)                       | SCL (external pull-up only)              |
| 5                            | Master Out Slave In (MOSI)               | SDA (external pull-up only)              |
| 4                            | Chip Select (CSB), chip-select, low-active | Selection LSB of device address (see 4.4.2.4.1 I²C device address) |
| 11                           | Master In Slave Out (MISO)               | Selection LSB of device address (see 4.4.2.4.1 I²C device address) |
| 7                            | Protocol Selection (PS)                  |                                          |
|                              | high level = I²C                         |                                          |
|                              | low level = SPI                          |                                          |

**Attention:** The MOSI pin has specific usage during serial data communication, depending on the protocol:

- SPI, 4-wire: uni-directional master-out data SPI,
- I²C: bi-directional serial data (external pull-up only)

### 4.4.2.3 SPI Protocol

The SPI interface is compatible with SPI mode 0 (CPOL = CPHA = '0') and mode '3' (CPOL = CPHA = '1'). The automatic selection between mode 0 and 3 is determined by the value of SCK after the CSB falling edge.

- Frequency 1 MHz – 10 MHz[^18]
- 4 wire connection

#### 4.4.2.3.1 SPI 4-wire Read Mode 0

A read transfer consists of 16-bit header information clocked out on the MOSI line followed by reading an arbitrary number of 16-bit words from the MISO line. The Chip Select Signal (CSB) stays low during the whole transfer.

![SPI 4-wire read mode 0](image-description)

*Figure 30: SPI 4-wire read mode 0*

#### 4.4.2.3.2 SPI 4-wire Write Mode 0

A write transfer consists of 16-bit header information followed by an arbitrary number of 16-bit words of payload. Header and payload are clocked out on the MOSI line. The Chip Select Signal (CSB) stays low during the whole transfer.

[^18]: reduced SPI speed for VDDIO < 1.8 V.


---


## 4.4.2.4 I²C Protocol

- **Standard-mode** (100 kHz)
- **Fast-mode** (400 kHz)
- **Fast-mode Plus** (Fm+, 1 MHz, recommended)

The protocol is compliant to the I2C specification UM10204 Rev. 3, with the following restrictions:

- 7-bit device addressing only
- No clock stretching

### 4.4.2.4.1 I²C Address Selection

The I²C device address can be selected depending on the unused CSB and MISO pin. These pins cannot be left floating; if left floating the I²C address will be undefined! This selection is latched after power-up and cannot be altered afterwards.

**Table 14: Host interface - I²C device address selection**

| Bit no. | <6> | <5> | <4> | <3> | <2> | <1> | <0> |
|---------|-----|-----|-----|-----|-----|-----|-----|
|         | 1   | 0   | 1   | 0   | 1   | CSB | MISO |

Below are some other I²C address selection possibilities:

- CSB = 0, MISO = 0, address = 0x54
- CSB = 0, MISO = 1, address = 0x55
- CSB = 1, MISO = 0, address = 0x56
- CSB = 1, MISO = 1, address = 0x57

### 4.4.2.4.2 I²C Read

A read sequence consists of two consecutive I²C transfers: 16 bits of header followed by an arbitrary number of payload data. The payload is always a multiple of 16 bits. For details on the header transfer, see Section 4.4.2.4.4.

![Figure 31: SPI 4-wire write mode 0](#)

![Figure 32: I²C read](#)


---


## 4.4.2.4.3 Complete I²C write

A write sequence consists of two consecutive I²C transfers: 16 bits of header followed by an arbitrary number of payload data. The payload is always a multiple of 16 bits. For details on the header transfer, see Section 4.4.2.4.4.

![Complete I²C write](image-placeholder)
*Figure 33: Complete I²C write*

## 4.4.2.4.4 I²C header transfer

The header is transferred by sending the slave address in write mode (R/ W = '0'), resulting in slave address 10101XX0 ('X' is determined by the state of CSB and MISO pin). Then the master sends the 16 bits of header information MSB first. The reception of a byte is acknowledged by the slave. The transaction is ended by a stop condition.

Figure 34 illustrates the header transmission. The device address is transferred first, followed by the R= W flag set to 0. Depending on the access type, the transfer is continued or followed by another one:

- **Write transfer**: with R/ W flag set to 0, is the header transmission plus following payload data.
- **Read transfer**: with R/ W flag set to 1, assumes a preceding single header transmission without payload data. It is up to the user to either follow-up with a new header transmission or another read access.

![I²C header transfer](image-placeholder)
*Figure 34: I²C header transfer*

## 4.4.2.4.5 I²C data read

After the header is transferred, a read transfer can be issued by sending the slave address in read mode (R/ W = '1'), resulting in slave address 10101XX1 ('X' is determined by state of CSB and MISO pin). Then the master can read an arbitrary number of 16-bit words, MSB first. The master acknowledges the reception of every byte. Data is read until a NACK (issued by the slave) followed by a stop condition occurs.

![I²C data read](image-placeholder)
*Figure 35: I²C data read*

## 4.5 Maintenance and service

Due to its unique measurement principle, the BMV080 particulate matter sensor does not comprise an air inlet or any moving or rotating parts (like, e.g., a fan), i.e., the sensor is designed to be maintenance free. Therefore, there is no need for the user to perform regular maintenance or service tasks.


---


## Optical Cover Maintenance

However, it is possible that dust, fingerprints, or other contamination accumulates on the outer surface of the optical cover of the host system. This might lead to a slight impact on the sensor performance. Hence, it can be beneficial to clean the optical cover surface using a wiping tissue from time to time. A suitable tissue shall be used to avoid scratches on the optical cover.


---


# 5 Software integration guidelines (Sensor driver)

The BMV080 sensor driver is the interface between the sensor and the user application on the host system. Bosch Sensortec provides sensor drivers to run on the host application processor.

![Figure 36: The sensor driver is the communication channel between the BMV080 and the user application](image-description)

The sensor driver includes a complete set of ready-to-use Application Programming Interfaces (APIs) to simplify the development of a host application. Section 5.2 describes these APIs in detail. These functions can be easily used to develop a user application specific to a determined use case.

## 5.1 Host requirements

Table 15 shows the technical requirements for the current version of the BMV080 sensor driver.

**Table 15: BMV080 sensor driver technical requirements for embedded systems**

| Supported platforms     | Compiler               | ROM *               | RAM               |
|-------------------------|------------------------|---------------------|-------------------|
|                         |                        | .text + .rodata     | .bss + .data      | .stack            |
| ARM Cortex-M4F          | arm-none-eabi-gcc      | 64 kB               | 17 kB             | 11 kB             |
| ARM Cortex-M4           | arm-none-eabi-gcc      | 64 kB               | 17 kB             | 11 kB             |
| ARM Cortex-M33F         | arm-none-eabi-gcc      | 63 kB               | 17 kB             | 11 kB             |
| ARM Cortex-M0+          | arm-none-eabi-gcc      | 66 kB               | 17 kB             | 11 kB             |
| ARM Cortex-M7F          | arm-none-eabi-gcc      | 62 kB               | 17 kB             | 11 kB             |
| ESP32                   | xtensa-esp32-elf-gcc   | 74 kB               | 17 kB             | 12 kB             |
| ESP32-S2                | xtensa-esp32s2-elf-gcc | 80 kB               | 17 kB             | 12 kB             |
| ESP32-S3                | xtensa-esp32s3-elf-gcc | 74 kB               | 17 kB             | 12 kB             |
| Raspberry Pi ARMv6 32Bit| arm-linux-gnueabihf-gcc| 89 kB               | 18 kB             | 18 kB             |
| Raspberry Pi ARMv8-A 32Bit| arm-linux-gnueabihf-gcc| 89 kB             | 18 kB             | 18 kB             |
| Raspberry Pi ARMv8-A 64Bit| aarch64-linux-gnu-gcc| 93 kB               | 18 kB             | 19 kB             |

*excluding 20 kB (approx.) for the standard library dependencies for different platforms.

Heap memory allocation is not used.

The compilation has been done in release mode with an -Os optimization flag.

The support for other platforms is being considered case-by-case. To request support for a particular embedded platform, please contact your Bosch Sensortec representative.


---


# 5.2 Application programming interface

## 5.2.1 Typedefs

### 5.2.1.1 Handles

#### 5.2.1.1.1 bmv080_handle_t

| Typedef | typedef void* **bmv080_handle_t**; |
|---------|------------------------------------|
| Summary | Unique handle for a sensor unit    |

#### 5.2.1.1.2 bmv080_sercom_handle_t

| Typedef | typedef void* **bmv080_sercom_handle_t**; |
|---------|-------------------------------------------|
| Summary | Unique handle for serial communication, i.e., the hardware connection to the sensor unit |

### 5.2.1.2 Enumerations

#### 5.2.1.2.1 bmv080_status_code_t

| Typedef | typedef enum { E_BMV080_OK = 0, [...] E_BMV080_WARNING_FIFO_FULL = 215, [...] E_BMV080_ERROR_NULLPTR = 100, [...] } **bmv080_status_code_t**; |
|---------|------------------------------------------------------------------------------------------------------------------------------------------------|
| Summary | Status codes of BMV080 sensor driver                                                                                                           |

#### 5.2.1.2.2 bmv080_measurement_algorithm_t

| Typedef | typedef enum { E_BMV080_MEASUREMENT_ALGORITHM_FAST_RESPONSE = 1, E_BMV080_MEASUREMENT_ALGORITHM_BALANCED = 2, E_BMV080_MEASUREMENT_ALGORITHM_HIGH_PRECISION = 3 } **bmv080_measurement_algorithm_t**; |
|---------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Summary | Possible measurement algorithms for BMV080 sensor driver seen as follows                                                                                                                            |

1. **Fast response**, recommended for use-cases which require BMV080 measurements with best response time (low latency).
2. **Balanced**, recommended for use-cases which require BMV080 measurements with a good balance between precision & fast response time.
3. **High precision**, recommended for use-cases which require BMV080 measurements with optimum precision performance.


---


# 5.2.1.3 Structure Definitions

## 5.2.1.3.1 bmv080_output_t

### Typedef

c
typedef struct
{
    float runtime_in_sec;
    float pm2_5_mass_concentration;
    float pm1_mass_concentration;
    float pm10_mass_concentration;
    float pm2_5_number_concentration;
    float pm1_number_concentration;
    float pm10_number_concentration;
    bool is_obstructed;
    bool is_outside_measurement_range;
    float reserved_0;
    float reserved_1;
    float reserved_2;
    struct bmv080_extended_info_s *extended_info;
} bmv080_output_t;


### Summary

The output structure is updated by `bmv080_serve_interrupt` when sensor output is available.

| **name**                      | **unit**       | **description**                                                                 |
|-------------------------------|----------------|---------------------------------------------------------------------------------|
| runtime_in_sec                | s              | Time passed since the start of the measurement cycle                            |
| pm2_5_mass_concentration      | µg/m³          | PM2.5 mass concentration                                                        |
| pm1_mass_concentration        | µg/m³          | PM1 mass concentration                                                          |
| pm10_mass_concentration       | µg/m³          | PM10 mass concentration                                                         |
| pm2_5_number_concentration    | particles/cm³  | PM2.5 number concentration                                                      |
| pm1_number_concentration      | particles/cm³  | PM1 number concentration                                                        |
| pm10_number_concentration     | particles/cm³  | PM10 number concentration                                                       |
| is_obstructed                 | N/A            | Flag to indicate whether the sensor is obstructed and cannot perform a valid measurement. |
| is_outside_measurement_range  | N/A            | Flag to indicate whether the PM2.5 concentration is outside the specified measurement range (0 – 1000 ug/m³) |
| reserved_0                    | N/A            | For internal use only                                                           |
| reserved_1                    | N/A            | For internal use only                                                           |
| reserved_2                    | N/A            | For internal use only                                                           |
| bmv080_extended_info_s        | N/A            | For internal use only                                                           |


---


# 5.2.1.4 Callbacks

## 5.2.1.4.1 bmv080_callback_read_t

**Callback**

c
typedef int8_t(*bmv080_callback_read_t)
(
    bmv080_sercom_handle_t sercom_handle,
    uint16_t header,
    uint16_t* payload,
    uint16_t payload_length
);


**Summary**

Function pointer for reading an array of *payload_length* words of 16-bit *payload*. All data, *header*, and *payload* are transferred as MSB first.

**Precondition**

Both *header* and *payload* words are 16-bit and combined. A *payload* is only transferred on a complete transmission of 16 bits. Burst transfers, i.e., reading a *header* followed by several *payload* elements, must be supported.

**Postcondition**

N/A

**Arguments**

| Argument       | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| sercom_handle  | Handle for a serial communication interface to a specific sensor unit       |
| header         | Header information for the following payload                                |
| * payload      | Payload to be read consisting of 16-bit words                               |
| payload_length | Number of payload elements to be read                                       |

**Return Value**

E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.

## 5.2.1.4.2 bmv080_callback_write_t

**Callback**

c
typedef int8_t(*bmv080_callback_write_t)
(
    bmv080_sercom_handle_t sercom_handle,
    uint16_t header,
    const uint16_t* payload,
    uint16_t payload_length
);


**Summary**

Function pointer for writing an array of *payload_length* words of 16-bit *payload*. All data, *header*, and *payload* are transferred as MSB first.

**Precondition**

Both *header* and *payload* words are 16-bit and combined. A *payload* is only transferred on a complete transmission of 16 bits. Burst transfers, i.e., reading a *header* followed by several *payload* elements, must be supported.

**Postcondition**

N/A

**Arguments**

| Argument       | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| sercom_handle  | Handle for a serial communication interface to a specific sensor unit       |
| header         | Header information for the following payload                                |
| * payload      | Payload to be written consisting of 16-bit words                            |
| payload_length | Number of payload elements to be read                                       |

**Return Value**

E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.


---

# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## 5.2.1.4.3 bmv080_callback_delay_t

**Callback**

c
typedef int8_t(*bmv080_callback_delay_t)
(
    uint32_t duration_in_ms
);


**Summary**  
Function pointer for executing a software delay operation

**Precondition**  
N/A

**Postcondition**  
N/A

**Arguments**

| Argument      | Description                          |
|---------------|--------------------------------------|
| duration_in_ms | Duration of the delay in milliseconds |

**Return Value**  
E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.

## 5.2.1.4.4 bmv080_callback_data_ready_t

**Callback**

c
typedef void(*bmv080_callback_data_ready_t)
(
    bmv080_output_t bmv080_output,
    void* callback_parameters
);


**Summary**  
Function pointer for handling the sensor’s output information

**Precondition**  
N/A

**Postcondition**  
N/A

**Arguments**

| Argument          | Description                                                      |
|-------------------|------------------------------------------------------------------|
| bmv080_output     | Structure containing sensor output                               |
| *callback_parameters | User-defined parameters to be passed to the callback function. |

**Return Value**  
E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.

## 5.2.2 Driver version

### 5.2.2.1 bmv080_get_driver_version

**Function**

c
bmv080_status_code_t bmv080_get_driver_version
(
    uint16_t* major,
    uint16_t* minor,
    uint16_t* patch,
    char git_hash[12],
    int32_t t num_commits_ahead
);


**Summary**  
Get the version information of this sensor driver

**Precondition**  
No preconditions apply, i.e., no connected sensor unit or sensor driver handle is required.

**Postcondition**  
N/A

**Arguments**

| Argument          | Description                          |
|-------------------|--------------------------------------|
| *major            | Major version number                 |
| *minor            | Minor version number                 |
| *patch            | Patch version number                 |
| git_hash[12]      | Git hash of the build                |
| num_commits_ahead | Number of commits ahead from build   |

**Return Value**  
E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.

---


## 5.2.3 Sensor Management

### 5.2.3.1 bmv080_open

**Function**

c
bmv080_status_code_t bmv080_open
(
    bmv080_handle_t* handle,
    const bmv080_sercom_handle_t sercom_handle,
    const bmv080_callback_read_t read,
    const bmv080_callback_write_t write,
    const bmv080_callback_delay_t delay_ms
);


**Summary**  
Open a sensor unit by initializing a new handle. The handle must be NULL initialized.

**Precondition**  
Must be called first to create the handle required by other functions.

**Postcondition**  
The handle must be destroyed via bmv080_close.

**Arguments**

| Argument   | Description                                         |
|------------|-----------------------------------------------------|
| * handle   | Unique handle for a sensor unit                     |
| sercom_handle | Unique handle for a serial communication interface |
| read       | Function pointer for reading from an endpoint       |
| write      | Function pointer for writing to an endpoint         |
| delay_ms   | Function pointer for a delay in milliseconds        |

**Return Value**  
E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.

### 5.2.3.2 bmv080_reset

**Function**

c
bmv080_status_code_t bmv080_reset
(
    const bmv080_handle_t handle
);


**Summary**  
Reset a sensor unit by performing a reset of the hardware and software.

**Precondition**  
A valid handle generated by bmv080_open is required.

**Postcondition**  
Any parameter changed through bmv080_set_parameter is reverted to its default.

**Arguments**

| Argument | Description                     |
|----------|---------------------------------|
| handle   | Unique handle for a sensor unit |

**Return Value**  
E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.

### 5.2.3.3 bmv080_close

**Function**

c
bmv080_status_code_t bmv080_close
(
    bmv080_handle_t* handle
);


**Summary**  
Close the sensor unit.

**Precondition**  
Must be called last to destroy the handle created by bmv080_open.

**Postcondition**  
N/A

**Arguments**

| Argument | Description                     |
|----------|---------------------------------|
| * handle | Unique handle for a sensor unit |

**Return Value**  
E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.


---


# 5.2.4 Sensor Identification

## 5.2.4.1 bmv080_get_sensor_id

**Function**


bmv080_status_code_t bmv080_get_sensor_id
(
    const bmv080_handle_t handle,
    char id[13]
);


**Summary**  
Get the sensor ID of a sensor unit.

**Precondition**  
A valid handle generated by `bmv080_open` is required. The application must have allocated the char array id with a size of 13 elements.

**Postcondition**  
N/A

**Arguments**

| Argument | Description                           |
|----------|---------------------------------------|
| handle   | Unique handle for a sensor unit       |
| id       | Character array of 13 elements        |

**Return Value**  
E_BMV080_OK if successful. Otherwise, the return value is a BMV080 status code.

# 5.2.5 Particulate Matter Measurement

## 5.2.5.1 User Application Flows

This section introduces two typical types of application flow by means of examples.

### 5.2.5.1.1 Continuous Measurement

[Figure 37 presents an activity diagram illustrating the process of conducting a continuous measurement, which is an unlimited duration measurement. The application is required to execute the sub-programs (highlighted in purple) from the BMV080 library.]

The measurement process begins by establishing a connection with the BMV080. Following this, measurement parameters can be set using the `bmv080_set_parameter()` function.

Initially, the sensor operates in sleep mode, drawing only standby current (as detailed in Table 12). A measurement is initiated by calling `bmv080_start_continuous_measurement()`, which activates the continuous measurement of particle density.

The service function `bmv080_serve_interrupt()` fetches and processes data from the BMV080. Sensor output is provided through the `callback function()`, which is triggered every second and is implemented on application level.

The `bmv080_serve_interrupt()` function can be invoked either at regular intervals (at least once per second) or event-driven, based on an external interrupt.

The measurement process can be halted by calling `bmv080_stop_measurement()`. This action puts the BMV080 back into sleep mode, reducing the current consumption to standby levels.

This setup allows for the implementation of various end-user applications. For instance, PM data can be logged into a database, displayed in real-time, or streamed directly to the cloud.


---


# Bosch Sensortec | BMV080 Ultra-mini Particulate Matter Sensor – Datasheet

## Application BMV080 API

[Flow diagram of continuous measurement]

**Figure 37: Flow diagram of continuous measurement**

A detailed explanation of each sub-program definition is in the API specification above.

### Timing sequence during continuous measurement

Figure 38 depicts the timing sequence for initiating a measurement. After the measurement process is initiated by calling `bmv080_start_continuous_measurement()`, the first measurement will be ready after a delay of 1.9 seconds. The sensor will then provide a new measurement every 1.03 seconds. If the IRQ line is used to trigger the `bmv080_serve_interrupt()` function, the first measurement will be ready after a longer delay of 2.9 seconds. However, subsequent measurements will continue to be available at regular intervals of 1.03 seconds.

---

© Bosch Sensortec GmbH 2025 | All rights reserved, also regarding any disposal, exploitation, reproduction, editing, distribution, as well as in the event of applications for industrial property rights

Document number: BST-BMV080-DS000-11


---


## 5.2.5.1.2 Duty Cycling Measurement

Figure 39 is an activity diagram that shows how to perform a duty cycling measurement – repeating numerous measurements separated by a pause. The main difference from continuous measurement is the duty cycling measurement will pause before repeating the next measurement cycle.

For duty cycling measurement, the service function `bmv080_serve_interrupt()` must be invoked at regular intervals, at least once per second.

**Note:** The event-driven approach using an external interrupt is not compatible with duty cycling measurement.

The period at which new data becomes available is determined by the `duty_cycling_period` parameter (refer to the `bmv080_set_parameter()` function for more details). During the sleep time of the duty cycling period, the sensor will be in sleep mode, limiting current consumption to standby levels. For more details, see Section 2.4.2.

Data availability is signaled through the callback function `bmv080_data_ready_callback()`, which is triggered once every `duty_cycling_period` has elapsed.

This setup allows for the implementation of various end-user applications. For instance, PM data can be logged into a database, displayed in real-time, or streamed directly to the cloud.

![Figure 38: Start-up sequence in case of Continuous Measurement Mode](#)

![Figure 39: Flow diagram of a duty cycling measurement](#)


---


# Timing Sequence During Duty Cycling Measurement

Figure 40 depicts the timing sequence for initiating a measurement. After the measurement process is initiated by calling `bmv080_start_start_duty_cycling_measurement()`, the first measurement will be ready after the Integration time and an additional delay of 1.17 seconds. The sensor will then provide new measurements at the rate of the configured Duty Cycling Period.

![Figure 40: Start-up sequence in case of Duty Cycling Measurement Mode](image-description)

## 5.2.5.2 bmv080_start_continuous_measurement

| Function | `bmv080_status_code_t bmv080_start_continuous_measurement`<br>(<br>&nbsp;&nbsp;const bmv080_handle_t handle<br>); |
|----------|---------------------------------------------------------------------------------------------------------------|
| **Summary** | Start particle measurement in continuous mode. |
| **Precondition** | A valid handle generated by `bmv080_open` is required.<br>Optionally, parameters can be set by previous calls of `bmv080_set_parameter`. |
| **Postcondition** | The measurement mode increases energy consumption.<br>The sensor unit stays in measurement mode until `bmv080_stop_measurement` is called.<br>In measurement mode, `bmv080_serve_interrupt` should be called regularly. |
| **Arguments** | `handle`<br>Unique handle for a sensor unit<br>`id`<br>Character array of 13 elements |
| **Return Value** | `E_BMV080_OK` if successful. Otherwise, the return value is a BMV080 status code. |

## 5.2.5.3 bmv080_start_duty_cycling_measurement

| Function | `bmv080_start_duty_cycling_measurement`<br>(<br>&nbsp;&nbsp;const bmv080_handle_t handle, const bmv080_callback_tick_t get_tick_ms,<br>&nbsp;&nbsp;bmv080_duty_cycling_mode_t duty_cycling_mode<br>); |
|----------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| **Summary** | Start particle measurement in duty cycling mode. |
| **Precondition** | A valid handle generated by `bmv080_open` is required. Optionally, duty cycling parameters (integration_time and duty_cycling_period) can be set by preceding `bmv080_set_parameter` calls. |
| **Postcondition** | The sensor unit stays in duty cycling mode until `bmv080_stop_measurement` is called. In measurement mode, `bmv080_serve_interrupt` should be called regularly. |
| **Arguments** | `handle`<br>Unique handle for a sensor unit<br>`get_tick_ms`<br>Function pointer that provides a tick value in milliseconds (based on the host system clock)<br>`duty_cycling_mode`<br>Mode of performing the duty cycling measurement |
| **Return Value** | `E_BMV080_OK` if successful. Otherwise, the return value is a BMV080 status code. |


---


# 5.2.5.4 bmv080_serve_interrupt

## Function
c
bmv080_status_code_t bmv080_serve_interrupt
(
    const bmv080_handle_t handle,
    bmv080_callback_data_ready_t data_ready,
    void* callback_parameters
);


## Summary
Serve an interrupt using a callback function.

## Precondition
A valid handle generated by `bmv080_open` is required with the sensor unit currently in measurement mode via `bmv080_start_continuous_measurement` or `bmv080_start_duty_cycling_measurement`.

The application can call this function whenever the sensor or the application triggers an interrupt. This interrupt may be a software timeout (e.g., at least once per second) or a hardware interrupt (e.g., FIFO watermark exceeded).

This function tolerates frequent, random, or rare calls to a certain extent. However, not calling `bmv080_serve_interrupt` over longer periods might impair the measurement mode since events could be missed.

In continuous mode, new sensor output is available every second. Hence, `data_ready` is called once every second of the sensor unit uptime. For example, if `bmv080_serve_interrupt` was called 5 s after `bmv080_start_continuous_measurement`, the callback function `data_ready` would subsequently be called five times to report the collected sensor output of each period.

In duty cycling mode, new sensor output is available every duty cycling period. Hence, `data_ready` is called at the end of the integration time, once every duty cycling period. In this case, `bmv080_serve_interrupt` must be called at least once every second.

The recommendation is to call this function based on hardware interrupts. The caller application provides the callback function `bmv080_callback_data_ready_t` and the according `callback_parameter`.

## Postcondition
The interrupt condition is served, e.g., FIFO is fetched, or the ASIC condition is solved.

## Arguments
| Argument           | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| handle             | Unique handle for a sensor unit                                             |
| data_ready         | User-defined callback function, which is called when sensor output is available |
| callback_parameters| User-defined parameters to be passed to the callback function               |

## Return Value
`E_BMV080_OK` if successful. Otherwise, the return value is a BMV080 status code.

# 5.2.5.5 bmv080_stop_measurement

## Function
c
bmv080_status_code_t bmv080_stop_measurement
(
    const bmv080_handle_t handle
);


## Summary
Stop particle measurement.

## Precondition
A valid handle generated by `bmv080_open` is required, and the sensor unit entered measurement mode via `bmv080_start_continuous_measurement` or `bmv080_start_duty_cycling_measurement`. Must be called at the end of a data acquisition cycle to ensure that the sensor unit is ready for the next measurement cycle.

## Postcondition
The sensing mode reduces energy consumption.

## Arguments
| Argument | Description                        |
|----------|------------------------------------|
| handle   | Unique handle for a sensor unit    |

## Return Value
`E_BMV080_OK` if successful. Otherwise, the return value is a BMV080 status code.


---


## 5.2.6 Customization

### 5.2.6.1 bmv080_get_parameter

**Function**

c
bmv080_status_code_t bmv080_get_parameter
(
    const bmv080_handle_t handle,
    const char* key,
    void* value
);


**Summary**

Get a parameter. The table called "Parameters to get" lists the available parameters with their keys and the expected types. This function can be called multiple times and is optional.

**Precondition**

A valid handle generated by `bmv080_open` is required.

**Postcondition**

N/A

**Arguments**

- **handle**: Unique handle for a sensor unit
- **key**: Key of the parameter to get
- **value**: Value of the parameter cast as void-pointer

**Parameters to Get**

| Key                      | Type                        | Unit | Description                                                                                                                                               |
|--------------------------|-----------------------------|------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| path                     | char*                       | N/A  | Path to directory where log files are written. The maximum allowed length is 256 characters, which must be pre-allocated.                                  |
| error_logging            | bool                        | N/A  | Enable/disable logging of error frames reported by the sensor in a CSV file. The filename format is `<yyyymmddTHHMMSS>_<SensorID>_errorFramesOutput.csv`.  |
| meta_data_logging        | bool                        | N/A  | Enable/disable logging of metadata reported by the sensor in a CSV file. The filename format is `<yyyymmddTHHMMSS>_<SensorID>_metaDataOutput.csv`.         |
| pm_logging               | bool                        | N/A  | Enable/disable logging of PM data in a CSV file. The filename format is `<yyyymmddTHHMMSS>_<SensorID>_postProcessorOutput.csv`.                            |
| integration_time         | float                       | s    | Measurement window for computing PM value. In duty cycling mode, this also includes the sensor ON time. The default is 10 s.                               |
| duty_cycling_period      | int                         | s    | Duty cycling period (sum of integration time and sensor OFF / sleep time). Duty cycling period must be greater than integration time by at least 2 s.      |
| do_obstruction_detection | bool                        | N/A  | Enable/disable obstruction notifier.                                                                                                                      |
| do_vibration_filtering   | bool                        | N/A  | Enable/disable vibration filtering.                                                                                                                       |
| measurement_algorithm    | bmv080_measurement_algorithm_t | N/A  | Selection of measurement algorithm based on the use case. Default value is `E_BMV080_MEASUREMENT_ALGORITHM_HIGH_PRECISION`. For a duty cycling measurement, this parameter is fixed to `E_BMV080_MEASUREMENT_ALGORITHM_FAST_RESPONSE`. |

**Return Value**

`E_BMV080_OK` if successful. Otherwise, the return value is a BMV080 status code.


---


### 5.2.6.2 bmv080_set_parameter

#### Function

c
bmv080_status_code_t bmv080_set_parameter
(
    const bmv080_handle_t handle,
    const char* key,
    void* value
);


#### Summary

Set a parameter. The table "Parameters to set" lists the available parameters with their keys and the expected types. This function can be called multiple times and is optional.

#### Precondition

Valid handle generated by `bmv080_open` is required.

This function must be called before `bmv080_start_continuous_measurement` or `bmv080_start_duty_cycling_measurement` in order to apply the parameter in the configuration of particle measurement.

#### Postcondition

N/A

#### Arguments

- **handle**: Unique handle for a sensor unit
- **key**: Key of the parameter to set
- **value**: Value of the parameter cast as void-pointer

#### Parameters to Set

| Key                      | Type                          | Unit | Description                                                                                                                                                                                                 |
|--------------------------|-------------------------------|------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| path                     | char*                         | N/A  | Path to directory where log files are written. The maximum allowed length is 256 characters, which must be pre-allocated.                                                                                   |
| error_logging            | bool                          | N/A  | Enable/disable logging of error frames reported by the sensor in a CSV file. The filename format is `<yyyymmddTHHMMSS>_<SensorID>_errorFramesOutput.csv`.                                                   |
| meta_data_logging        | bool                          | N/A  | Enable/disable logging of metadata reported by the sensor in a CSV file. The filename format is `<yyyymmddTHHMMSS>_<SensorID>_metaDataOutput.csv`.                                                          |
| pm_logging               | bool                          | N/A  | Enable/disable logging of PM data in a CSV file. The filename format is `<yyyymmddTHHMMSS>_<SensorID>_postProcessorOutput.csv`.                                                                             |
| integration_time         | float                         | s    | Measurement window for computing PM value. In duty cycling mode, this also includes the sensor ON time. The default is 10 seconds.                                                                          |
| duty_cycling_period      | int                           | s    | Duty cycling period (sum of integration time and sensor OFF / sleep time). Duty cycling period must be greater than integration time by at least 2 seconds. The default is 30 seconds.                       |
| do_obstruction_detection | bool                          | N/A  | Enable/disable obstruction notifier.                                                                                                                                                                        |
| do_vibration_filtering   | bool                          | N/A  | Enable/disable vibration filtering.                                                                                                                                                                         |
| measurement_algorithm    | bmv080_measurement_algorithm_t| N/A  | Selection of measurement algorithm based on the use case. Default value is `E_BMV080_MEASUREMENT_ALGORITHM_HIGH_PRECISION`. For a duty cycling measurement, this parameter is fixed to `E_BMV080_MEASUREMENT_ALGORITHM_FAST_RESPONSE`. |

#### Return Value

`E_BMV080_OK` if successful. Otherwise, the return value is a BMV080 status code.

---

*File logging is available only for Windows x86/x64 and Raspberry Pi, but not for embedded platforms (e.g., ARM Cortex-M, Xtensa ESP32, etc).*


---


# 6 Traceability

A laser marking (DMC and OCR code) on the sensor is used to identify the single parts and to enable traceability through the production and supply chain.

**Table 16: BMV080 marking convention**

| General                        |                                      |
|--------------------------------|--------------------------------------|
| Marking method                 | Laser (Direct part marking)          |
| Marking position               | Refer to drawing                     |

| Information about DMC          |                                      |
|--------------------------------|--------------------------------------|
| Marking type                   | DMC, ECC 200 (ISO/IEC 16022)         |
| Module size                    | 0.130 ± 0.01 mm                      |
| Symbol size                    | 14 x 14 (Row × column)               |
|                                | nominal 1.82 mm × 1.82 mm            |
| Marking depth                  | < 15 µm                              |
| Marking quality (Grade)        | A-C (ISO/IEC TR 29158)               |
| Information capacity DMC       | 16 (Numeric)                         |
| DMC sequence                   | Digit 1, digit 2, ..., digit 16      |
| Digits 1 – 7                   | Reserved                             |
| Digit 8                        | 0 = 2020                             |
|                                | 1 = 2021                             |
|                                | :                                    |
|                                | 9 = 2029                             |
|                                | Year                                 |
| Digits 9 – 10                  | 01 ~ 53                              |
|                                | Work week                            |
| Digit 11                       | 1 = Sun                              |
|                                | 2 = Mon                              |
|                                | :                                    |
|                                | 7 = Sat                              |
|                                | Day                                  |
| Digits 12 – 16                 | Reserved                             |

| Information about marking text |                                      |
|--------------------------------|--------------------------------------|
| Font type                      | Arial1                               |
| Symbol size                    | 2.15 mm × 0.4 mm                     |
| Information capacity marking text | 6 (Numeric)                     |
| Marking text sequence          | Digit 1, digit 2, ..., digit 6       |
| Digit 1                        | 0 = 2020                             |
|                                | 1 = 2021                             |
|                                | :                                    |
|                                | 9 = 2029                             |
|                                | Year                                 |
| Digits 2 – 3                   | 01 ~ 53                              |
|                                | Work Week                            |
| Digit 4                        | 1 = Sun                              |
|                                | 2 = Mon                              |
|                                | :                                    |
|                                | 7 = Sat                              |
|                                | Day                                  |
| Digits 5 – 6                   | Reserved                             |


---


# 7 Product compliance

## 7.1 Environmental safety

### 7.1.1 RoHS

BMV080 is in compliance with the consolidated RoHS directive 2011/65/EU of the European Parliament and Council regarding the restriction of hazardous substances in electrical and electronic equipment.

### 7.1.2 Halogen content

BMV080 complies with the halogen-free definition of the industry standard IEC 61249 for materials utilized in printed boards and other interconnecting structures.

## 7.2 Laser safety

The design of the BMV080 limits the emitted optical output power to 0.5 mW. The BMV080 is laser class 1 compliant.

### 7.2.1 Conformity and classification

BMV080 is

- laser class 1 compliant according to norm: “Safety of laser products –Part 1: Equipment classification and requirements”, IEC60825-1 Edition 3.0 (2014), respectively, EN 60825-1:2014/A11:2021.
- a consumer product according to norm “Safety of laser products – Particular Requirements for Consumer Laser Products”, EN 50689 (2021).
- compliant with FDA performance standards for laser products except for conformance with IEC 60825-1 Edition 3.0, as described in Laser Notice No. 56, dated May 8, 2019.

This has independently been confirmed by Seibersdorf Laboratories (Test report LE-L176/23, 2024-02-28). The Laser Class 1 classification was achieved by using C-samples on EvalKits as application setup.

![Laser Safety Image](image-description)

*Figure 41: Class 1 laser product*


---


# 8 Additional material

Additional material related to the BMV080 includes the following design files and software packages:

## Sensor integration

3D CAD file of BMV080: BST-BMV080-CAD.stp

## Sensor software

BMV080 Software Development Kit (including support for the BMV080 Shuttle Board 3.1 and Bosch Sensortec Application Board 3.1) : BST-BMV080-SDK


---


# 9 Legal Disclaimer

## 9.1 Engineering Samples

Engineering Samples are marked with an asterisk (*), (E) or (e). Samples may vary from the valid technical specifications of the product series contained in this data sheet. They are therefore not intended or fit for resale to third parties or for use in end products. Their sole purpose is internal client testing. The testing of an engineering sample may in no way replace the testing of a product series. Bosch Sensortec assumes no liability for the use of engineering samples. The Purchaser shall indemnify Bosch Sensortec from all claims arising from the use of engineering samples.

## 9.2 Product Use

Bosch Sensortec products are developed for the consumer goods industry. They may only be used within the parameters of this product data sheet. They are not fit for use in life-sustaining or safety-critical systems. Safety-critical systems are those for which a malfunction is expected to lead to bodily harm, death or severe property damage. In addition, they shall not be used directly or indirectly for military purposes (including but not limited to nuclear, chemical or biological proliferation of weapons or development of missile technology), nuclear power, deep sea or air or space applications (including but not limited to satellite technology) or supercomputers. If customers would like to use Bosch Sensortec products in supercomputers, customers are obligated to get written permissions from Bosch Sensortec.

Bosch Sensortec products are released on the basis of the legal and normative requirements relevant to the Bosch Sensortec product for use in the following geographical target market: BE, BG, DK, DE, EE, FI, FR, GR, IE, IT, HR, LV, LT, LU, MT, NL, AT, PL, PT, RO, SE, SK, SI, ES, CZ, HU, CY, US, CN, JP, KR, TW. If you need further information or have further requirements, please contact your local sales contact.

The resale and/or use of Bosch Sensortec products are at the purchaser’s own risk and his own responsibility. The examination of fitness for the intended use is the sole responsibility of the purchaser.

The purchaser shall indemnify Bosch Sensortec from all third party claims arising from any product use not covered by the parameters of this product data sheet or not approved by Bosch Sensortec and reimburse Bosch Sensortec for all costs in connection with such claims.

The purchaser accepts the responsibility to monitor the market for the purchased products, particularly with regard to product safety, and to inform Bosch Sensortec without delay of all safety-critical incidents.

## 9.3 Application Examples and Hints

With respect to any examples or hints given herein, any typical values stated herein and/or any information regarding the application of the device, Bosch Sensortec hereby disclaims any and all warranties and liabilities of any kind, including without limitation warranties of non-infringement of intellectual property rights or copyrights of any third party. The information given in this document shall in no event be regarded as a guarantee of conditions or characteristics. They are provided for illustrative purposes only and no evaluation regarding infringement of intellectual property rights or copyrights or regarding functionality, performance or error has been made.


---


# Document History and Modifications

| Rev. No. | Chapter | Description of Modification/Changes | Date     |
|----------|---------|-------------------------------------|----------|
| 1.0      | all     | Initial release.                    | Aug 2024 |
| 1.1      | 2.2     | Updated technical specifications and lifetime. | Dec 2024 |
|          | 3.2     | Comparison of pin numbering schemes for BMV080 and ZIF connectors added. |          |
|          | 4.4.1.2 | Proposal for filtering signal errors added. |          |
|          | 4.4.2.4 | Corrected image for complete I²C write. |          |
|          | 5.1     | Host requirements updated. |          |
|          | 5.2     | PM1 definition added. |          |
|          | 6       | Updated content of DMC and laser marking. |          |
|          | 7.2     | Updated information on laser class compliance. |          |
| 1.2      | 1.1     | Update with PM10 and PM1. | Jan 2025 |
|          | 5.1     | Updated host requirements. |          |
|          | 5.2.1.3 | PM10 mass concentration definition added; PM2.5, PM1, PM10 number concentration definition added. |          |
|          | 5.2.6   | Update on error logging, meta data logging and PM logging in get and set parameter definition. |          |
| 1.3      | all     | Editorial work. | May 2025 |
|          | 2.1     | Reference to Technical Specification Statement added. |          |
|          | 2.2     | Updated information on measurement algorithms. Recommendation for integration and use-case specific qualification by customer. Reference to Integration Guideline added. |          |
|          | 2.3     | Update on storage conditions. |          |
|          | 3.1     | LGA package height corrected. |          |
|          | 3.2     | Information added about min. bending radius and max. bending angles of Flex PCB. Bending area defined in drawing. |          |
|          | 4.1.3.1 | Update of mounting and assembly instruction: sealing of cavity added. |          |
|          | 4.4.1.4.1 | Update of figures, ground on pins VSSA, VSSD added. |          |
|          | 4.4.1.4.2 | |          |
|          | 4.4.1.4.3 | |          |
|          | 4.4.2.1 | Table for interface selection removed. |          |
|          | 4.4.2.4 | Section about I²C date write removed. |          |
|          | 5.1     | Host requirements for ARM Cortex-M7F added. |          |
|          | 5.2.1.3 | Correction of unit of PM particle concentration. |          |
|          | 8       | Information on BMV080 EvalKit removed, Update on Sensor Software Development Kit. |          |


---

I'm unable to extract text from the image you provided. Please provide the text content, and I can help you convert it to  format.