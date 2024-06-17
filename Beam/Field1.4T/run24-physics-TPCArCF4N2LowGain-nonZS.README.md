# Introduction

TPC operation with around 4.1kV (limited but some physics capable performance), with the rest of big partition of silicon, TPOT, and calorimeter detectors. TPC use a gas of 65/25/10 Ar/CF4/N2

The run period contain mix of nonZS ZS data, but **this list focus on the nonZS runs** which is best characterizeation of the detector performance. It limit the triggera rate to 30Hz or so. 

Goal:
- HV stability at the edge of physics capability + get more data for offline to tune to simulation
- Larger TPC performance and joint silicon + tracking + calo study
- High cross section analysis like K0s and photon conversion analysis
- Baseline non ZS data for zero suppression development (noise control, readout stability, threshold scan, and offline reco)

# Run log

## Jun 17, 2024

### Big partition configuration

running with nonZS TPC at 30 Hz, with the following gl1 and trigger configurations:
* Multi event buffering off
* tpc ENDAT = 100000
* Trigger 10 (MBD >= 1) scaledown = 10000
* Trigger 29 (Photon 2 GeV) = 300
* Trigger 30 (Photon 3 GeV) = 100
* Trigger 31 (Photon 4 Gev) = 100
Reference: https://chat.sdcc.bnl.gov/sphenix/pl/we8tux6ufjyfm86s9tmwszr91h

### Run log

* 45888: TPC: GEMs: 4.1 kV, CM: 44.3 kV (all trackers in MVTX, INTT, TPC, TPOT, and all calo). **Trigger prescale and MEB tuning during the run**. Reference: https://chat.sdcc.bnl.gov/sphenix/pl/tfdprph5fiyjzc4x79rc5cz1wo
* 45890: TPC: GEMs: 4.1 kV, CM: 44.3 kV (all trackers in MVTX, INTT, TPC, TPOT, and all calo). Sector 8 FEEs being reset so missing from most of the run. Reference: https://chat.sdcc.bnl.gov/sphenix/pl/entpoxwanbdn8rd77zanjbx4fo 
* 45892: TPC: GEMs: 4.1 kV, CM: 44.3 kV (all trackers in MVTX, INTT, TPC, TPOT, and all calo). Good run. Reference: https://chat.sdcc.bnl.gov/sphenix/pl/c7cxz6q9nj8juyoc37ro3bxxta
