### Instrument Performance
There are several different ways in which we can measure the performance of an instrument:
1) Storage/Transmission of Data
2) Sensitivity or Signal to Noise Ratio
3) Spectral Band
4) Swath Width
5) Field of View
6) Coverage
7) Scanning Modes
8) Resolution
#### Spectral Band
This is just the area of the EM spectrum that the instrument is recording in, e.g. X-Ray, optical etc.
![[Pasted image 20240916143223.png|center|300]]
#### Swath
This is the path that the sensor looks at on the ground. It is measured across the path of the spacecraft, and this is called the 'swath width'. Its width is determined by the height of the orbit and the sensor field of view.
![[Pasted image 20240916143338.png|center]]
#### Field of View
The angular field of view (also field of vision, abb. FOV) is the extent of the observable world that is seen at any given moment. It is usually measured in degrees, radians, arcminutes, or arcseconds. FOV is dependant on focal length and detector size (with a large detector resulting in a wide FOV whilst a long focal length results in a narrow FOV).
![[Pasted image 20240916143536.png|centre]]
#### Coverage
Footprint is defined as the shape of the area of the Earth which the satellite communicate with or observe at **a moment in time**. There is a different footprint for each transponder or communications transmitter. Coverage is defined as the **total geographic area** that the satellite can communicate with. Example: Geostationary Operational Environmental Satellites (GOES) provide continuous imagery and data on atmospheric conditions and solar activity (space weather) from Geostationary orbit. This allows them to be over one point on the Earth continuously.
#### Scanning Modes
There are three primary scanning modes:
![[Pasted image 20240916143750.png|centre]]
1) Whiskbroom – uses rotating mirrors to sweep from side to side across the track and reflect image on to one detector. They are simple but have mechanical (moving) parts which is not a good idea in a vacuum. Dwell time is limited.
2) Pushbroom – uses a line of CCD detectors. These offer more dwell time.
3) Staring – uses a 2D array and offers even more dwell time for fast frame rates. However, they are computationally intensive.

#### The Different Types of Resolution
There are several different types of resolution:
- Spatial resolution
- Angular resolution
- Spectral resolution
- Radiometric resolution
- Temporal resolution
\
**Spatial Resolution** describes the size of the smallest possible feature that can be detected, it is measured in metres along a line.
**Angular Resolution** is similar and describes the smallest feature per unit of angle i.e. degrees or arcminutes.
**Spectral Resolution** describes the ability of a sensor to define fine wavelength intervals and is measured in metres. The finer the spectral resolution, the narrower the wavelength range for a particular channel or band.
**Radiometric Resolution** of an imaging system describes its ability to discriminate very slight differences in energy and is measured in bits. The finer the radiometric resolution of a sensor, the more sensitive it is to detecting small differences in reflected or emitted energy.
**Temporal Resolution** of a sensor is the revisit frequency (the time it takes to return to the same view of Earth) and is measured in units of time.
##### Resolution Calculations
###### Spatial or Ground Resolution
The spatial resolution is the size of the pixel on the ground 's' or ground resolution. $\theta$ is the required angle, $d$ is the range, and $s$ is the size of the object or 'ground resolution element'.
![[Pasted image 20240917154359.png|centre]]
$$s=d\sin\theta \approx d\cdot\theta~~~~~(\text{Due to the SAA.})\\ $$ 