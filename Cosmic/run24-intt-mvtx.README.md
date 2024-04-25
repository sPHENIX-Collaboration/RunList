# INTT and MVTX cosmic runs

## Trigger descriptions

Some of these runs include the TPC and were rate limited to 30 Hz with wide, horizontal cosmics. Some runs excluded the TPC and used vertical narrow triggers which increased the rate to ~75 Hz with significantly improved efficiency, at least a 10x improvement. The MVTX was operated with an 89 microsecond strobe length (readout window)

__NOTE:__ I (Cameron Dean) generated TrkrCluster DSTs with this run list using a _new_ build of the sPHENIX software stack on April 25th 2024. [This was to take advantage of this pull request from Yasser](https://github.com/sPHENIX-Collaboration/coresoftware/pull/2654). I also added two lines of code to the MVTX unpacker in ```offline/packages/mvtx/MvtxCombinedRawDataDecoder.cc``` to reject any events without a L1 trigger in the MVTX. The MVTX ran streamed at 89us so 1 min of data is ~650k events. The cosmic rate in the MVTX is ~ 30 Hz.

The code change is as follows. The bit with ```if (m_writeMvtxEventHeader)``` already exists and is used so people can find where to add the code (line 193).

```c++
//Remove this later
if (l1BCOs.size() == 0) return Fun4AllReturnCodes::ABORTEVENT;
if (mvtx_hit_container->get_nhits() <= 2) return Fun4AllReturnCodes::ABORTEVENT;

  if (m_writeMvtxEventHeader)
  {
    mvtx_event_header =
        findNode::getClass<MvtxEventInfo>(topNode, "MVTXEVENTHEADER");
    assert(mvtx_event_header);
  }
```

| Run   | Trigger                                           |  Comments                          |
|-------|---------------------------------------------------|------------------------------------|
| 38401 | Vertical wide cosmics | Includes TPC. 10 MVTX staves exlcuded |
| 38402 | Vertical wide cosmics | Includes TPC. 10 MVTX staves exlcuded |
| 38934 | Vertical narrow cosmics | |
| 38935 | Vertical narrow cosmics | | 
| 38936 | Vertical narrow cosmics | |
| 38941 | Vertical narrow cosmics | |
| 38943 | Vertical narrow cosmics | |
| 39521 | Vertical narrow cosmics | | 
| 39522 | Vertical narrow cosmics | |
| 39523 | Vertical narrow cosmics | |
| 39611 | Vertical narrow cosmics | |
| 39977 | Horizontal z-cross cosmics | | 
| 39978 | Vertical z-cross cosmics | | 
| 39979 | Unknown, possibly same as 39978 | INTT2 and INTT6 are recording ~2 times more than other INTT servers | 
| 39983 | Vertical narrow cosmics | | 
| 39994 | Vertical narrow cosmics | | 
| 40174 | Vertical narrow cosmics | | 
| 40175 | Vertical narrow cosmics | |
| 40176 | Vertical narrow cosmics | | 
| 40214 | Vertical narrow cosmics | | 
| 40215 | Vertical narrow cosmics | | 
| 40216 | Vertical narrow cosmics | | 
| 40226 | Vertical narrow cosmics | TPC included | 
| 40227 | Unknown, either horizontal or vertical wide | TPC included | 
