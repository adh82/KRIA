# n.Kria
extensible native norns port of monome's Kria

# changelog
| num | description |
|-|-|
| 0.23
|-| sync groups
|-| temp looping
|-| intense memory optimization
|-| greatly tightened timing accuracy
|-| some fixes to meta sequencer
| 0.19
|-| note, along with overall pitch, as a mod source
|-| retooled stretch and push to be more musical
| 0.18 
|-| lots of internal rewrites
|-| fixed problems introduced in 1.17
| 0.17 | 
|-| added cut functionality 
|-| enabled trigger clocking 
|-| fixed triangle mode 
| 0.16 | fixed neotrellis highlight support, added init message, changed docs slightly |
| 0.15 | fixed odds mod key not working at all. |
|| fixed crash on accessing mod keys from scale page |

# KRIA fork changes

This fork keeps the classic Ansible-style Grid workflow as the single active mode.

- MIDI transport start resets the sequencer before playback.
- MIDI transport stop stops voices, resets the sequencer, and clears playback.
- Note Sync defaults on.
- Note Division Sync defaults off.
- Division Sync defaults to none, so track and parameter divisions are independent.
- Loop Sync defaults to all, sharing loop endpoints without coupling clock divisions.
- Grid Time modifier division writes are scoped to the selected track and parameter.
