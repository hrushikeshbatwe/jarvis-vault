---
updated: 2026-08-20
---
# Become the Tiger
- 3-minute UE5 psychological horror cinematic for client Dan
- Delivered and paid (~week of Aug 10, 2026), project closed
- Was in revision after Dan requested a compressed human section using only POV shots and an eye-dissolve transformation
- Working through UE5 rendering bugs: MRQ temporal sample issues, PCG memory crashes
- Current rate with Dan is $700 for the 3-minute cinematic (previously $600), far below market
- Next project will be repriced upward toward a $1,500 minimum
- Cannot be used publicly in outreach until cleared for public use; EAGLE leads outreach until then
- Revision replaced the human section with a MetaHuman eye close-up and POV run dissolving into tiger POV; received strong approval
- Full pipeline built in UE5.7 with MetaHuman, spline-based tiger animation, PCG forest, Movie Render Queue
- Suffered a catastrophic ~20GB data loss from a Perforce workspace misconfiguration mid-project; Recuva recovered key files, project rebuilt over a weekend
- Perforce reconfigured correctly afterward with a proper client workspace, .p4ignore file, and strict submit-after-milestone workflow
- UE5.7 MRQ bugs documented and resolved: temporal sample count dropping frames, Flush Grass Streaming OOM crashes, false "not all frames submitted" errors
- MetaHuman facial animation done via offline MetaHuman Animator pipeline after Live Link Face proved too unstable
