# How it works

## 1. Components

- A geostationary satellite (GEO) ~ 22.3k miles above Earth's equator

    __*Notes__: Operating in K<sub>a</sub>-band for narrow spot beam for:
  - higher cap (by reusing bandwith)
  - increase performance

- gateway: ground stations which help receive/transmite data from/to satellite
- antenna with transceiver (transmit + receive)
- Other: Modem
-HUB:a proccesor, in the middle of star topology

## 2. How they interact

- Processed request from gateway server modulated into signal -> Satellite -> subscriber terminal and demodulates and vice versa. (*Insert an diagram :P)

- Antenna dish: must have unobstructed view -> satellite (doable bc its fixed)

## 3. Connectivity

__Ref__: 
- _SATELLITE COMMUNICATION SYSTEMS: Systems, Techniques and Technology (Chap 7.4 and 9.4.5)_ [1]
- _Broadband Satellite Communications for Internet Access (Chap 4.3.3)_ [2]


Depending on the on-board processing capability and the network layer, different techniques are considered for interconnection of coverage:

- transponder hopping (used when there is no on-board processing):
  - what is on-board processing: demodulation + demultiplexing received signal.
  - when to use: low no. of beams (beams are divided band)
  - Filters on satellite separates carriers accordance with sub-band ocupied
  - Output of ea filter -------transponder------> destination beam
  - no. of filters and transponder > no. of beams<sup>2</sup>
- on-board switching (processing) (used when there is transparent and regenerative processing);
  - transaparent processing:
    - when to use: no. of beams is high and satellite payload becomes too complex & heavy
    - 2 types (not going detail since its complicated):
      - analogue transparent switching: DCU + switching maps uplink beam -> downlink beam by magic.
      - digital transparent switching: relying on digital filtering and switching.
  - regenerative processing: baseband switching device routes the packets from a particular uplink beam to the appropriate downlink beam by TST (time-space-time) or T (single stage). 
- beam scanning
  - when to use: both with transparent and regenerative payloads.
    - __with transparent payload__: at least 2 beams are in on-board storage in given instant: to establish uplink & downlink
    - __with regenerative payload__: single beam sequentially scans beam dwell area. Info is extracted and stored for later transmission when beam passed destiation area.

# Satellite broadcast to earth

## 1. Components

- a transmitting hub station (rather very large)
- a number of receive-only earth stations (rather small -> cheap: < 100 Euros)

## 2. Types
__*Ref__: _SATELLITE COMMUNICATION SYSTEMS: Systems, Techniques and Technology (Chap 7.6)_

- __single programmes per satellite channel__: each broadcaster access to diff transponders bandwith, modulated and then broadcasted at full EIRP by satellite.
- __several programmes per satellite channel__: each broadcaster access to 1 transponder within seperated subbands, modulated then broadcasted at reduced ERIP and intermodolation noise.
- __Single uplink with time division multiplex of programmes__: multiple broadcaster access to feeder station (for time division multiplexing) then uplinked to transponder bandwith then broadcasted at full EIRP.
- __Multiple uplink with time division multiplex of programmes__:da fuq mate? look at the image and describe....

[1]: (http://gen.lib.rus.ec/book/index.php?md5=22C07E8AD6898293F92D9E093F94D0C4)
[2]: (http://gen.lib.rus.ec/book/index.php?md5=8F9BC91482E2CFA036306EC62AC8CE8D)
