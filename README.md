# A Doppler, A Misadventure
My prototype CW Doppler Radar. 

### Tech Stack
 - ADALM-Pluto SDR, modified for increased bandwidth and maximum operating frequency + U.FL to SMA connector for injecting clock signal.
 - Leo Bodnar Mini GPSDO to generate perfect 40MHz clock signal
 - 2 of Maarten Baert's open source design 9.4dBi triple-feed patch antennas
 - GNU Radio Companion

### Planned Implementation
The way I will implement this system is still up in the air as I work on fine-tuning the radar and software. Having looked into the various applications of Doppler radar, I'd like to take the project in a biomedical/assistive technology direction. Because my system operates in the 5.8GHz ISM band, it is fairly different than many existing Doppler applications in that the 5.8GHz signal can penetrate materials like wood, plastic, and glass. Because the human body still acts as a reflector at this frequency, I am looking into using the system for machine-learning powered gesture recognition or heartbeat/respiration sensing.

### Changes and Fixes
 [ ] Possible pivot to 2 SDRs instead of 1 to prevent internal TX/RX crosstalk
 [ ] Phase out GPSDO, repurpose for FMCW projects where phase alignment is critical
 [ ] Simulation for calculating ideal setup
