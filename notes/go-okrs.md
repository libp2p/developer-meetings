## Attendees
- @diasdavid
- @whyrusleeping
- @jbenet
- @bigs
- @mgoelzer
- @stebalien


## Moved

Moved to https://docs.google.com/spreadsheets/d/1HTXfgR5FyPTFhsTkFPRThkeMvHvCgJOaAs7BSl_vQ_0/edit#gid=1240336497 

That google sheet is the source of truth for OKRs.  Notes in this repo are for historical purposes only.

## Objectives & KRs

- O:  Hiring/Leverage
    
    KR:  Weekly call with {Steb, D#, JB, why, Cole, Mike} occurs at least 75% (=9) weeks of the quarter
    
    KR:  Each engineer sources N high quality candidates
    
    KR:  Hire at least 2 high quality candidates per quarter

- O:  Absolutely critical features/fixes

    KR:  The peerstore not being in memory (P0)
    
    KR:  QUIC (P0)
    
    KR:  Implement connection management (P0)
    
    KR:  Replace multistream select (P1)
    
    KR:  Merge the DHT pipeline (P1)

- O:  go-libp2p is a well-maintained project

    KR:  X% of issues are responded to
    
    KR:  X% of pull requests merged
    
    KR:  Waffle board becomes main interface into projecta

		



---------------

## Everything below here is junk:


#### Roadmap

- Get DHT pipelining merged
- Get peerstore syncing to disk and performant
- [abandoned to discuss thread higher level OKRs instead]


#### OKRs

- O:  Reduce memory usage

   KR:  (something with reducing GC)
    
- O:  Improving connectivity
    
    
    
- O:  Better connection management
   
    KR:  Implement connection suspension
    
    KR:  Better tagging

- O:  Improve DHT performance
    KR:  (Pipeline requests between peers, or ???)
    KR:  Replace Multistream

- O:  Improve Correctness And Security
    KR:  Replace Secio
    KR:  Replace Multistream
    
- O:  go-libp2p is well maintained
    
    KR:  X% of issues are responded to
    
    KR:  X% of pull requests merged

- O:  Our go package manager is easy to use and learn
    
    KR:  Fix https://github.com/whyrusleeping/gx/issues/179



