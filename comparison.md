Comparisons between mitigation techniques

(skip the first 3 sections I note this for myself)

# Ka band, Ku band

- Ka band:  microwave freq 26.5 - 40 gigahertz (GHz)
- Ku band: microwave freq 12 - 18 gigahertz (GHz)

# Phenomena

- attenuation due to precipitation (rain, snow, hail, ice droplets) --> hydrometeor scattering
- gaseous absorption (O2, H2O vapor), small, compared to rain
- cloud attenuation
- melting layer attenuation
- sky noise increase
- signal depolarization (nonspherical scatterers like raindrops), significant for systems reusing freq by transmitting 2 orthogonally polarized sig --> cross-polar interference
- tropospheric scintillations: variation in magnitude and the profile of refractive index of troposphere amplitude fluctuation
- interseystem interference: between satellite and terrestrial systems

# Techniques

- EIRP (Effective Isotropic Radiated Power) control techniques: 
  - uplink/downlink power control (terrestrial/sat)
  - spot beam shaping (beamwidth down = gain up)
- Adaptive transmission techniques
  - hierarchical coding: more error detection code (cons: increase bandwidth)
  - hierarchical modulation: decrease Eb/N0 (what is that?), exchange spectral eff for power requirements, use high order QSK/QAM
  - data rate reduction (don't quite understand this)
- Diversity protection schemes: oriented against rain fades (main factor for > 10GHz)
  - site diversity: take many stations on earth to ensure prob error on both sites low
  - orbital diversity: more satellites
  - freq diversity: high freq (Ka, EHF) during normal operation, lower freq (C, Ku) when high rain attenuation
  - time diversity: retransmission

- Observe/monitor link quality by performing continuous measurements of propagation conditions
- Provide a short-term estimation/prediction of the behavior and the relevant duration of the next state of the satellite channel.
- Set/change the parameters of the system based on the above short-term estimate.

# Comparisons

| FMT   | Availability range | Maximum achievable | Limiting factor  |
|       | of year (%)        | gain (dB)          |                  |
|-------|--------------------|--------------------|------------------|
| ULPC  | 0.01 - 10          | 5 (VSAT)           | Earth station    |
|       |                    | 15 (hubs)          | power range      |
|-------|--------------------|--------------------|------------------|
| DLPC  | 0.01 - 10          | 3 (satellite TWTA) | sat pow range    |
|-------|--------------------|--------------------|------------------|
| SBS   | 0.01 - 10          | 5 (sat attena)     | immature research|
|-------|--------------------|--------------------|------------------|
| HC/HM | 0.01 - 1           | 10 - 15 (Eb/N0     | simultaneous     |
|       |                    |          range)    | fadin in stations|
|-------|--------------------|--------------------|------------------|
| DDR   | 0.01 - 10          | 3-9                | RR intolerant    |
|-------|--------------------|--------------------|------------------|
| SD    | 0.001 - 0.1        | 10-30 (conv rain)  | cost             |
|-------|--------------------|--------------------|------------------|
| OD    | 0.001 - 1          | 3-10               | sat switching    |
|-------|--------------------|--------------------|------------------|
| FD    | 0.001 - 10         | 30 (bwn Ka & Ku)   | cost             |
|-------|--------------------|--------------------|------------------|

- ULPC only adjusts the earth station power --> easy & flexible
- DLPC: same, but limitations of sat amplifier
- SBS: allow mitigation of propagation impairments by stratiform rain over an area of ?00 km
- HC/HM: only a few earth stations at the same time or resource runs out
- DDR does not significantly affect multi-access, but suitable only for appl that tolerate low info rate
- SD, OD: more eff if atmosphere exhibits inhomogeneities (heterogenities?) so alternative path
  which are less affected by rain exist
- FD: can be applied regardless of time percentage, produce large gain, but costly
- TD: not considered