
== RunListGen ==
================================================
Dataset      : run3auau (range 66457-78954)
Tag/DST      : pro001_pcdb001_v001 / DST_CALOFITTING
Subsystems   : hcal, emcal, mbd, sepd
================================================
L0 Configuration:
	Runtype in ['physics']
	Require VGTMs: True with requested VGTMs [5, 8, 9, 10]
	Run length >= 300 sec
	Magnet on with current >= 4.5e7: True
	Min bias triggers: ['12']
	Livetime bits: [12] with thresholds [0.7]
	Report level: summary
================================================
L1 Configuration:
	QA columns   : emcal, emcal_auto, ihcal, ihcal_auto, mbd, ohcal, ohcal_auto, sepd
	Offline QA status    : 3 predicates
		emcal_auto == GOLDEN
		ohcal_auto == GOLDEN
		ihcal_auto == GOLDEN
	Triggers     : 12, 12 (including min bias ['12'])
	Reco min events: 1,000,000
================================================

== Inputs ==
FileCatalog  : 3,076 runs
DAQ (base)   : 9,732 runs
DAQ (L0 pass): 3,067 runs
Production   : 4,302 runs

== L0 Cutflow (DAQ cuts; FC-matched events shown) ==
Stage                                            Runs  Removed    Eff         Events MB_scaled_bit0
---------------------------------------------------------------------------------------------------
DAQ base (runnumber range)                      9,732        0      - 57,668,772,074 49,840,899,198
runtype in physics                              4,302    5,430  44.2% 57,668,772,074 46,128,699,180
require_vgtms_all: [5, 8, 9, 10]                4,265       37  99.1% 57,668,772,074 46,128,699,180
magnet_on && current>=4.5e7                     4,237       28  99.3% 57,437,401,271 46,128,699,180
run_length >= 300                               3,171    1,066  74.8% 57,437,401,271 46,128,699,180
require_scaledown_bits != -1: [12, 12]          3,080       91  97.1% 56,888,918,115 46,128,699,180
livetime(bit=12) >= 0.7                         3,067       13  99.6% 56,839,494,785 46,128,699,180

== Merged ==
Common runs  : 2,977 (FC ∩ DAQ(L0) ∩ PROD)
Merged rows  : 2,977

== Cutflow (Merged -> reco_min_events -> QA) ==
Stage                                            Runs  Removed    Eff         Events
------------------------------------------------------------------------------------
Merged: FC ∩ DAQ(L0) ∩ PROD                     2,977        0      - 56,839,494,785
min_reco_events >= 1,000,000                    2,977        0 100.0% 56,839,494,785
offline status predicates                       2,776      201  93.2% 53,007,238,064

== Final Totals ==
Runs         : 2,776
Events       : 53,007,238,064
MB_scaled    : bit 12: 41875724879

== Artifacts ==
Cutflow report JSON: RunList/Physics/Calo/goodRuns/scripts/run3auau/run3auau_pro001_pcdb001_v001_dst_calofitting_cutflow_report.json

== Outputs ==
GRL          : RunList/Physics/Calo/goodRuns/scripts/run3auau/run3auau_pro001_pcdb001_v001_dst_calofitting_grl.list
Run details  : RunList/Physics/Calo/goodRuns/scripts/run3auau/run3auau_pro001_pcdb001_v001_dst_calofitting_run_details.json
