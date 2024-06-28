# Introduction

TPC operation with around 4.1kV (limited but some physics capable performance), with the rest of big partition of silicon, TPOT, and calorimeter detectors. TPC use a gas of 65/25/10 Ar/CF4/N2

The run period contain mix of nonZS ZS data, but **this list focus on the nonZS runs** which is best characterizeation of the detector performance. It limit the triggera rate to 30Hz or so. 

Goal:
- HV stability at the edge of physics capability + get more data for offline to tune to simulation
- Larger TPC performance and joint silicon + tracking + calo study
- High cross section analysis like K0s and photon conversion analysis
- Baseline non ZS data for zero suppression development (noise control, readout stability, threshold scan, and offline reco). 
  - SAMPA baseline correction 3 (BC3) is enabled: https://chat.sdcc.bnl.gov/sphenix/pl/ih7zgjce3fbyjnrgka8i4iggpe 

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

* TPC gas: Ar:CF4: (60:40)

### Runs

* 45888: TPC: GEMs: 4.1 kV, CM: 44.3 kV (all trackers in MVTX, INTT, TPC, TPOT, and all calo). **Trigger prescale and MEB tuning during the run**. Reference: https://chat.sdcc.bnl.gov/sphenix/pl/tfdprph5fiyjzc4x79rc5cz1wo
* 45890: TPC: GEMs: 4.1 kV, CM: 44.3 kV (all trackers in MVTX, INTT, TPC, TPOT, and all calo). Sector 8 FEEs being reset so missing from most of the run. Reference: https://chat.sdcc.bnl.gov/sphenix/pl/entpoxwanbdn8rd77zanjbx4fo 
* 45892: TPC: GEMs: 4.1 kV, CM: 44.3 kV (all trackers in MVTX, INTT, TPC, TPOT, and all calo). Good run. Reference: https://chat.sdcc.bnl.gov/sphenix/pl/c7cxz6q9nj8juyoc37ro3bxxta


## Jun 19, 2024 

### Big partition configuration/ TPC config.

running with nonZS TPC at 30 Hz, with the following gl1 and trigger configurations:
* Multi event buffering off
* tpc ENDAT = 360
* Trigger 10 (MBD >= 1)
* Trigger 25 (Photon 3 GeV + MBD coin.) 
* Trigger 26 (Photon 4 GeV + MBD coin.)  
* Trigger 27 (Photon 5 Gev + MBD coin.) 
* Trigger 29 (Photon 2 GeV) 
* Trigger 30 (Photon 3 GeV) 
* Trigger 31 (Photon 4 Gev)

* TPC gas: Ar:CF4:N2 (65:25:10)
* TPC HV: 4.1 kV, CM: 44.3 kV,
* TPC FEE: 400 samples, 120 pre-samples

### Runs

* Run 46040 [10 , 29, 30, 31] (watch out for transient noise) mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/57hmhkownjy8ufks7i4gwkhrme
* Run 46041 [10, 29, 30, 31] (watch out for transient noise) mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/7ph4gfewujrw7y7o9q7wbb9jee
* Run 46043 [10] mattermost refernce thread: https://chat.sdcc.bnl.gov/sphenix/pl/xty8dftq6bb43yhz6scd63fdyo
* Run 46044 [29, 30, 31] (watch out for transient noise) mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/9os31qzxkirhpy6m1zaohizbgh
* Run 46045 [25, 26, 27] mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/bhnsr7oxepb6fdtzmnfq7jzjie
* Run 46046 [10, 25, 26, 27] mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/mexspb5ef3yadj3gbd6kgsm5da
* Run 46048 [10, 25, 26, 27] mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/xxyc9fc1epgu5jxn1ffouaje9y
* Run 46050 [10, 25, 26, 27] mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/1pouz5iso7g97cp7xznuzzx3be
* Run 46051 [10, 25, 26, 27] mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/7fmezy7h7jdtjria4uhhccjnfe
* Run 46052 [10, 25, 26, 27] mattermost reference thread: https://chat.sdcc.bnl.gov/sphenix/pl/j946ezi6spyf3dymrc3yf13zro

## Jun 25, 2024

### Big partition configuration/ TPC config.

running with nonZS TPC at 30 Hz, with the following gl1 and trigger configurations:
* Multi event buffering off
* tpc ENDAT = 235000
* Trigger 10 (MBD >= 1)
* Trigger 25 (Photon 3 GeV + MBD coin.) 
* Trigger 26 (Photon 4 GeV + MBD coin.)  
* Trigger 27 (Photon 5 Gev + MBD coin.) 

* TPC gas: Ar:CF4:N2 (65:25:10)
* TPC FEE: 400 samples, 120 pre-samples
* Note: This data is mostly rare triggers, MBD coin. only is ~ 4 %

### Runs

* Run 46723 [10 , 25, 26, 27], (all trackers in MVTX, INTT, TPC, TPOT, and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/cu5x617ee7gijnzzdtktxfexwc
* Run 46725 [10 , 25, 26, 27], (INTT, TPC, TPOT, and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/fjsk8w7h3tby3fm6x93zc3r56o
* Run 46726 [10 , 25, 26, 27], (INTT, TPC, TPOT, and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/h5neseckaf8b5rtstcyjpbxouy
* Run 46727 [10 , 25, 26, 27], (INTT, TPC, TPOT, and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/wq8cntqdttd858y5ja4eom7pwh
* Run 46728 [10 , 25, 26, 27], (NTT, TPC, TPOT, and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/91pdmmk4wt898phxmco7xnmi7c
* Run 46729 [10 , 25, 26, 27], (all trackers in MVTX, INTT, TPC, TPOT, and all calo), TPC: GEMs 4.15 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/9d993e7j7trzur5p7age81kbdh
* Run 46730 [10 , 25, 26, 27], (INTT, TPC, TPOT, and all calo), TPC: GEMs 4.2 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/xjokfs9si3dw3jg967u9eyzj9r

## Jun 26, 2024

### Big partition configuration/ TPC config.

TPC running with mixture of ZS and nonZS TPC w/ and w/o diffuse lasers at 40 Hz, with the following detector, gl1 and trigger configurations:

* TPC gas: Ar:CF4:N2 (65:25:10)
* TPC FEE: 400 or 425 samples, 120 pre-samples
* Diffuse Lasers - 4 MIP intensity https://chat.sdcc.bnl.gov/sphenix/pl/ouq5twcm7pg88p6wb1oghok5nw
* Note all voltages are "weather equivalent"

### Runs

* Run 46776 (calib, no laser, nonZS), (all trackers except MVTX and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/5c6yssiqbjgz5mbr36gthsrd3h
* Run 46777 (calib, 7.6 kHz laser, nonZS), (all trackers except MVTX and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/mruipt5shbfgtkxafk4tbr6sar
* Run 46778 (physics, no laser, nonZS), (all trackers except MVTX and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/jii5hdxu47nk9jt73e5hhx3taa
* Run 46781 (physics GL1 sync laser, nonZS), (all trackers except MVTX and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/s5jhipzt4ibq7ygryrot8pfbfe
* Run 46782 (ZS + 40Hz GL1 sync 20Hz laser, **ZS, 10 ADU thresh**), (all trackers except MVTX and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/dnz98fnbmigotpydwrmnim3mwh
* Run 46784 (calib + 45 Hz laser, nonzS) BEAM OFF, TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/zwwszpzhsiry8yqh1k3sco4tae


## Jun 28, 2024

### Big partition configuration/ TPC config.

TPC running with mixture of ZS and nonZS TPC w/ and w/o diffuse lasers at 40 Hz, with the following detector, gl1 and trigger configurations:

* TPC gas: Ar:CF4:N2 (65:25:10)
* TPC FEE: 400 or 425 samples, 120 pre-samples
* Diffuse Lasers - 4 MIP intensity https://chat.sdcc.bnl.gov/sphenix/pl/ouq5twcm7pg88p6wb1oghok5nw
* MBD narrow vertex trigger (approx |z| < 10 cm)
* Note all voltages are "weather equivalent"

### Runs

* Run 46975 (nonZS, laser),(all trackers and all calo, stopped early due to INTT issue) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/tregxbeupfnstm61xw6y6z487y 
* Run 46976 (nonZS, laser),(all trackers and all calo) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/sdeksbbk9jf13m5eqhws46urew
* Run 46977 (nonZS, no laser),(all trackers and all calo, GL1 mismatch in EMCAL) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/jewxfmsg77gszk89k5a9jrincr
* Run 46978 (ZS 15 ADU thresh, no laser),(all trackers and all calo) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/1ni3moyqa7nhuxiak634y353eh
* Run 46979 (ZS 15 ADU thresh, laser),(all trackers and all calo, GL1 mismatch in all ADcs except MBD and ZDC) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/gzxj5rkks3n18yrwtuzwd99dqw
* Run 46980 (ZS 5 ADU thresh, laser),(all trackers and all calo) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/3rqegitomi84mn1ms7c777d1se
* Run 46981 (ZS 5 ADU thresh, no laser), (all trackers and all calo) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/kcm5x81n6pruje44sg9tfbw5wo
* Run 46982 (ZS 25 ADU thresh, no laser), (all trackers and all calo) TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/igm16kft4jgnpb88j9je1g9m6r
* Run 46983 (ZS 25 ADU thresh, laser), (all trackers and all calo, e-link reset isse in TPC), TPC: GEMs 4.1 kV, CM: 44.3 kV https://chat.sdcc.bnl.gov/sphenix/pl/o3pe5mo3fjntfetageg1c6x8hy
* Run 46984 (ZS 20 ADU thresh, laser), (all trackers and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV, https://chat.sdcc.bnl.gov/sphenix/pl/dm41qi8yridwdqc7aj6a68ddha
* Run 46985 (ZS 20 ADU thresh, no laser), (all trackers and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV, https://chat.sdcc.bnl.gov/sphenix/pl/b9qmdg817t88jx1ttfkcbb1gmc
* Run 46986 (ZS 10 ADU thresh, no laser), (all trackers and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV, https://chat.sdcc.bnl.gov/sphenix/pl/fkcnfcwuxpn5ip6qwtr3nphzfw
* Run 46987 (ZS 10 ADU thresh, laser), (all trackers and all calo), TPC: GEMs 4.1 kV, CM: 44.3 kV, https://chat.sdcc.bnl.gov/sphenix/pl/gonzwruhbirojf64i367uq7kyy
